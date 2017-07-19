## KubeProxyConfig v1alpha2 kops

Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | KubeProxyConfig





<aside class="notice">
Appears In  <a href="#clusterspec-v1alpha2-kops">ClusterSpec</a> </aside>

Field        | Description
------------ | -----------
clusterCIDR <br /> *string*    | clusterCIDR is the CIDR range of the pods in the cluster. It is used to bridge traffic coming from outside of the cluster. If not provided, no off-cluster bridging will be performed.
cpuRequest <br /> *string*    | 
hostnameOverride <br /> *string*    | hostnameOverride, if non-empty, will be used as the identity instead of the actual hostname. Note: We recognize some additional values:  @aws uses the hostname from the AWS metadata service
image <br /> *string*    | 
logLevel <br /> *integer*    | 
master <br /> *string*    | master is the address of the Kubernetes API server (overrides any value in kubeconfig)

