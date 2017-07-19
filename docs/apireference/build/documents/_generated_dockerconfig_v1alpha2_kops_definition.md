## DockerConfig v1alpha2 kops

Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | DockerConfig





<aside class="notice">
Appears In  <a href="#clusterspec-v1alpha2-kops">ClusterSpec</a> </aside>

Field        | Description
------------ | -----------
bridge <br /> *string*    | 
bridgeIP <br /> *string*    | The bridge cidr (--bip) flag
insecureRegistry <br /> *string*    | 
ipMasq <br /> *boolean*    | 
ipTables <br /> *boolean*    | 
logDriver <br /> *string*    | 
logLevel <br /> *string*    | 
logOpt <br /> *string array*    | 
mtu <br /> *integer*    | 
registryMirrors <br /> *string array*    | Set mirrors for dockerd, benefiting cluster provisioning and image pulling
storage <br /> *string*    | Storage maps to the docker storage flag But nodeup will also process a comma-separate list, selecting the first supported option
version <br /> *string*    | The version of docker to install Be careful if changing this; not all docker versions are validated, and they will break in bad ways.

