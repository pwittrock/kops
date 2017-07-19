## KubeletConfigSpec v1alpha2 kops

Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | KubeletConfigSpec





<aside class="notice">
Appears In  <a href="#clusterspec-v1alpha2-kops">ClusterSpec</a>  <a href="#instancegroupspec-v1alpha2-kops">InstanceGroupSpec</a> </aside>

Field        | Description
------------ | -----------
allowPrivileged <br /> *boolean*    | allowPrivileged enables containers to request privileged mode. Defaults to false.
anonymousAuth <br /> *boolean*    | AnonymousAuth chooses if you want anonymous auth on the kubelet api
apiServers <br /> *string*    | not used for clusters version 1.6 and later
babysitDaemons <br /> *boolean*    | The node has babysitter process monitoring docker and kubelet. Removed as of 1.7
cgroupRoot <br /> *string*    | cgroupRoot is the root cgroup to use for pods. This is handled by the container runtime on a best effort basis.
clientCaFile <br /> *string*    | The client CA which the requestes for the above must be signed by
cloudProvider <br /> *string*    | cloudProvider is the provider for cloud services.
clusterDNS <br /> *string*    | clusterDNS is the IP address for a cluster DNS server.  If set, kubelet will configure all containers to use this for DNS resolution in addition to the host's DNS servers
clusterDomain <br /> *string*    | clusterDomain is the DNS domain for this cluster. If set, kubelet will configure all containers to search this domain in addition to the host's search domains.
configureCbr0 <br /> *boolean*    | configureCBR0 enables the kublet to configure cbr0 based on Node.Spec.PodCIDR.
enableCustomMetrics <br /> *boolean*    | enable gathering custom metrics.
enableDebuggingHandlers <br /> *boolean*    | enableDebuggingHandlers enables server endpoints for log collection and local running of containers and commands
enforceNodeAllocatable <br /> *string*    | Enforce Allocatable across pods whenever the overall usage across all pods exceeds Allocatable.
evictionHard <br /> *string*    | Comma-delimited list of hard eviction expressions.  For example, 'memory.available<300Mi'.
evictionMaxPodGracePeriod <br /> *integer*    | Maximum allowed grace period (in seconds) to use when terminating pods in response to a soft eviction threshold being met.
evictionMinimumReclaim <br /> *string*    | Comma-delimited list of minimum reclaims (e.g. imagefs.available=2Gi) that describes the minimum amount of resource the kubelet will reclaim when performing a pod eviction if that resource is under pressure.
evictionPressureTransitionPeriod <br /> *[Duration](#duration-v1-meta)*    | Duration for which the kubelet has to wait before transitioning out of an eviction pressure condition.
evictionSoft <br /> *string*    | Comma-delimited list of soft eviction expressions.  For example, 'memory.available<300Mi'.
evictionSoftGracePeriod <br /> *string*    | Comma-delimited list of grace periods for each soft eviction signal.  For example, 'memory.available=30s'.
featureGates <br /> *object*    | FeatureGates is set of key=value pairs that describe feature gates for alpha/experimental features.
hairpinMode <br /> *string*    | How should the kubelet configure the container bridge for hairpin packets. Setting this flag allows endpoints in a Service to loadbalance back to themselves if they should try to access their own Service. Values:   "promiscuous-bridge": make the container bridge promiscuous.   "hairpin-veth":       set the hairpin flag on container veth interfaces.   "none":               do nothing. Setting --configure-cbr0 to false implies that to achieve hairpin NAT one must set --hairpin-mode=veth-flag, because bridge assumes the existence of a container bridge named cbr0.
hostnameOverride <br /> *string*    | hostnameOverride is the hostname used to identify the kubelet instead of the actual hostname. Note: We recognize some additional values:  @aws uses the hostname from the AWS metadata service
imageGCHighThresholdPercent <br /> *integer*    | imageGCHighThresholdPercent is the percent of disk usage after which image garbage collection is always run.
imageGCLowThresholdPercent <br /> *integer*    | imageGCLowThresholdPercent is the percent of disk usage before which image garbage collection is never run. Lowest disk usage to garbage collect to.
kubeReserved <br /> *object*    | Resource reservation for kubernetes system daemons like the kubelet, container runtime, node problem detector, etc.
kubeReservedCgroup <br /> *string*    | Control group for kube daemons.
kubeconfigPath <br /> *string*    | kubeconfigPath is the path to the kubeconfig file with authorization information and API server location kops will only use this for clusters version 1.6 and later
kubeletCgroups <br /> *string*    | KubeletCgroups is the absolute name of cgroups to isolate the kubelet in.
logLevel <br /> *integer*    | 
maxPods <br /> *integer*    | maxPods is the number of pods that can run on this Kubelet.
networkPluginMTU <br /> *integer*    | networkPluginMTU is the MTU to be passed to the network plugin, and overrides the default MTU for cases where it cannot be automatically computed (such as IPSEC).
networkPluginName <br /> *string*    | networkPluginName is the name of the network plugin to be invoked for various events in kubelet/pod lifecycle
nodeLabels <br /> *object*    | nodeLabels to add when registering the node in the cluster.
nonMasqueradeCIDR <br /> *string*    | nonMasqueradeCIDR configures masquerading: traffic to IPs outside this range will use IP masquerade.
nvidiaGPUs <br /> *integer*    | nvidiaGPUs is the number of NVIDIA GPU devices on this node.
podCIDR <br /> *string*    | The CIDR to use for pod IP addresses, only used in standalone mode. In cluster mode, this is obtained from the master.
podManifestPath <br /> *string*    | 
reconcileCIDR <br /> *boolean*    | reconcileCIDR is Reconcile node CIDR with the CIDR specified by the API server. No-op if register-node or configure-cbr0 is false.
registerSchedulable <br /> *boolean*    | registerSchedulable tells the kubelet to register the node as schedulable. No-op if register-node is false.
requireKubeconfig <br /> *boolean*    | 
resolvConf <br /> *string*    | ResolverConfig is the resolver configuration file used as the basis for the container DNS resolution configuration."), []
runtimeCgroups <br /> *string*    | Cgroups that container runtime is expected to be isolated in.
systemCgroups <br /> *string*    | SystemCgroups is absolute name of cgroups in which to place all non-kernel processes that are not already in a container. Empty for no container. Rolling back the flag requires a reboot.
systemReserved <br /> *object*    | Capture resource reservation for OS system daemons like sshd, udev, etc.
systemReservedCgroup <br /> *string*    | Parent control group for OS system daemons.
taints <br /> *string array*    | Taints to add when registering a node in the cluster
volumePluginDirectory <br /> *string*    | The full path of the directory in which to search for additional third party volume plugins

