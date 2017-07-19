## KubeControllerManagerConfig v1alpha2 kops

Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | KubeControllerManagerConfig





<aside class="notice">
Appears In  <a href="#clusterspec-v1alpha2-kops">ClusterSpec</a> </aside>

Field        | Description
------------ | -----------
allocateNodeCIDRs <br /> *boolean*    | allocateNodeCIDRs enables CIDRs for Pods to be allocated and, if ConfigureCloudRoutes is true, to be set on the cloud provider.
attachDetachReconcileSyncPeriod <br /> *[Duration](#duration-v1-meta)*    | ReconcilerSyncLoopPeriod is the amount of time the reconciler sync states loop wait between successive executions. Is set to 1 min by kops by default
cloudProvider <br /> *string*    | cloudProvider is the provider for cloud services.
clusterCIDR <br /> *string*    | clusterCIDR is CIDR Range for Pods in cluster.
clusterName <br /> *string*    | clusterName is the instance prefix for the cluster.
configureCloudRoutes <br /> *boolean*    | configureCloudRoutes enables CIDRs allocated with allocateNodeCIDRs to be configured on the cloud provider.
image <br /> *string*    | 
leaderElection <br /> *[LeaderElectionConfiguration](#leaderelectionconfiguration-v1alpha2-kops)*    | leaderElection defines the configuration of leader election client.
logLevel <br /> *integer*    | 
master <br /> *string*    | 
pathSrvKubernetes <br /> *string*    | 
rootCAFile <br /> *string*    | rootCAFile is the root certificate authority will be included in service account's token secret. This must be a valid PEM-encoded CA bundle.
serviceAccountPrivateKeyFile <br /> *string*    | 
terminatedPodGCThreshold <br /> *integer*    | terminatedPodGCThreshold is the number of terminated pods that can exist before the terminated pod garbage collector starts deleting terminated pods. If <= 0, the terminated pod garbage collector is disabled.
useServiceAccountCredentials <br /> *boolean*    | UseServiceAccountCredentials controls whether we use individual service account credentials for each controller.

