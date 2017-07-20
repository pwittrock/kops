# How to update the apirefrence docs

These instructions assume:

- [apiserver-builder](https://github.com/kubernetes-incubator/apiserver-builder/) version v0.1-alpha.6 is installed and on the path.
- The [types repo](https://github.com/kubernetes/api) is vendored as part of the project

## Update the `pkg/openapi/openapi_generated.go`

From the root kops directory run:

```sh
apiserver-boot build generated --generator openapi
```

This will run the openapi-gen code generator and update the openapi definition.

**Note:** If you do not have the types repo installed, this command will fail, but print
out the openapi-gen command it tried to run.  As a workaround, take the failed command
and remove the types repo types from it (and replace them with the client-go types if
you use them).

## Update `docs/apireference`

```sh
mkdir -p bin
go build -o bin/apiserver cmd/kops-server/main.go
apiserver-boot build docs --disable-delegated-auth=false --output-dir docs/apireference
rm docs/apireference/build/runbrodocs.sh
rm docs/apireference/build/node_modules/marked/Makefile
```

This will build the apiserver, get the openapi definitions, and write them to
`docs/apireference/openapi-spec/swagger.json`.  It will then generate the reference
documentation from the openapi.

