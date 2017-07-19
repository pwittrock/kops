## KubeAPIServerConfig v1alpha2 kops

Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | KubeAPIServerConfig





<aside class="notice">
Appears In  <a href="#clusterspec-v1alpha2-kops">ClusterSpec</a> </aside>

Field        | Description
------------ | -----------
address <br /> *string*    | 
admissionControl <br /> *string array*    | 
allowPrivileged <br /> *boolean*    | 
anonymousAuth <br /> *boolean*    | 
apiServerCount <br /> *integer*    | 
auditLogMaxAge <br /> *integer*    | The maximum number of days to retain old audit log files based on the timestamp encoded in their filename.
auditLogMaxBackups <br /> *integer*    | The maximum number of old audit log files to retain.
auditLogMaxSize <br /> *integer*    | The maximum size in megabytes of the audit log file before it gets rotated. Defaults to 100MB.
auditLogPath <br /> *string*    | If set, all requests coming to the apiserver will be logged to this file.
authenticationTokenWebhookCacheTtl <br /> *[Duration](#duration-v1-meta)*    | The duration to cache responses from the webhook token authenticator. Default is 2m. (default 2m0s)
authenticationTokenWebhookConfigFile <br /> *string*    | File with webhook configuration for token authentication in kubeconfig format. The API server will query the remote service to determine authentication for bearer tokens.
authorizationMode <br /> *string*    | 
authorizationRbacSuperUser <br /> *string*    | 
basicAuthFile <br /> *string*    | 
clientCAFile <br /> *string*    | 
cloudProvider <br /> *string*    | 
etcdServers <br /> *string array*    | 
etcdServersOverrides <br /> *string array*    | 
image <br /> *string*    | 
insecurePort <br /> *integer*    | 
kubeletClientCertificate <br /> *string*    | 
kubeletClientKey <br /> *string*    | 
kubeletPreferredAddressTypes <br /> *string array*    | 
logLevel <br /> *integer*    | 
oidcCAFile <br /> *string*    | If set, the OpenID server's certificate will be verified by one of the authorities in the oidc-ca-file otherwise the host's root CA set will be used.
oidcClientID <br /> *string*    | The client ID for the OpenID Connect client, must be set if oidc-issuer-url is set.
oidcGroupsClaim <br /> *string*    | If provided, the name of a custom OpenID Connect claim for specifying user groups. The claim value is expected to be a string or array of strings.
oidcIssuerURL <br /> *string*    | The URL of the OpenID issuer, only HTTPS scheme will be accepted. If set, it will be used to verify the OIDC JSON Web Token (JWT).
oidcUsernameClaim <br /> *string*    | The OpenID claim to use as the user name. Note that claims other than the default ('sub') is not guaranteed to be unique and immutable.
pathSrvKubernetes <br /> *string*    | 
pathSrvSshproxy <br /> *string*    | 
runtimeConfig <br /> *object*    | keys and values in RuntimeConfig are parsed into the `--runtime-config` parameter for KubeAPIServer, concatenated with commas. ex: `--runtime-config=key1=value1,key2=value2`. Use this to enable alpha resources on kube-apiserver
securePort <br /> *integer*    | 
serviceClusterIPRange <br /> *string*    | 
storageBackend <br /> *string*    | 
tlsCertFile <br /> *string*    | 
tlsPrivateKeyFile <br /> *string*    | 
tokenAuthFile <br /> *string*    | 

