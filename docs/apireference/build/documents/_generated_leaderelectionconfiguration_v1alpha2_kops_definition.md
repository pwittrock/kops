## LeaderElectionConfiguration v1alpha2 kops

Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | LeaderElectionConfiguration



LeaderElectionConfiguration defines the configuration of leader election clients for components that can run with leader election enabled.

<aside class="notice">
Appears In  <a href="#kubecontrollermanagerconfig-v1alpha2-kops">KubeControllerManagerConfig</a>  <a href="#kubeschedulerconfig-v1alpha2-kops">KubeSchedulerConfig</a> </aside>

Field        | Description
------------ | -----------
leaderElect <br /> *boolean*    | leaderElect enables a leader election client to gain leadership before executing the main loop. Enable this when running replicated components for high availability.

