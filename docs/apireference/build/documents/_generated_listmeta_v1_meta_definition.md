## ListMeta v1 meta

Group        | Version     | Kind
------------ | ---------- | -----------
meta | v1 | ListMeta



ListMeta describes metadata that synthetic resources must have, including lists and various status objects. A resource may have only one of {ObjectMeta, ListMeta}.

<aside class="notice">
Appears In  <a href="#clusterlist-v1alpha2-kops">ClusterList</a>  <a href="#instancegrouplist-v1alpha2-kops">InstanceGroupList</a>  <a href="#status-v1-meta">Status</a> </aside>

Field        | Description
------------ | -----------
resourceVersion <br /> *string*    | String that identifies the server's internal version of this object that can be used by clients to determine when objects have changed. Value must be treated as opaque by clients and passed unmodified back to the server. Populated by the system. Read-only. More info: https://git.k8s.io/community/contributors/devel/api-conventions.md#concurrency-control-and-consistency
selfLink <br /> *string*    | SelfLink is a URL representing this object. Populated by the system. Read-only.

