## EtcdClusterSpec v1alpha2 kops

Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | EtcdClusterSpec





<aside class="notice">
Appears In  <a href="#clusterspec-v1alpha2-kops">ClusterSpec</a> </aside>

Field        | Description
------------ | -----------
etcdMembers <br /> *[EtcdMemberSpec](#etcdmemberspec-v1alpha2-kops) array*    | EtcdMember stores the configurations for each member of the cluster (including the data volume)
name <br /> *string*    | Name is the name of the etcd cluster (main, events etc)

