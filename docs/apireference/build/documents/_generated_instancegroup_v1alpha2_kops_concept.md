

-----------
# InstanceGroup v1alpha2 kops

>bdocs-tab:example 

```bdocs-tab:example_yaml

apiVersion: kops/v1alpha2
kind: InstanceGroup
metadata:
  name: instancegroup-example
spec:

```


Group        | Version     | Kind
------------ | ---------- | -----------
kops | v1alpha2 | InstanceGroup







InstanceGroup represents a group of instances (either nodes or masters) with the same configuration

<aside class="notice">
Appears In <a href="#instancegrouplist-v1alpha2-kops">InstanceGroupList</a> </aside>

Field        | Description
------------ | -----------
apiVersion <br /> *string*    | APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/api-conventions.md#resources
kind <br /> *string*    | Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds
metadata <br /> *[ObjectMeta](#objectmeta-v1-meta)*    | 
spec <br /> *[InstanceGroupSpec](#instancegroupspec-v1alpha2-kops)*    | 


### InstanceGroupSpec v1alpha2 kops

<aside class="notice">
Appears In <a href="#instancegroup-v1alpha2-kops">InstanceGroup</a> </aside>

Field        | Description
------------ | -----------
additionalSecurityGroups <br /> *string array*    | AdditionalSecurityGroups attaches additional security groups (e.g. i-123456)
associatePublicIp <br /> *boolean*    | AssociatePublicIP is true if we want instances to have a public IP
cloudLabels <br /> *object*    | CloudLabels indicates the labels for instances in this group, at the AWS level
image <br /> *string*    | 
kubelet <br /> *[KubeletConfigSpec](#kubeletconfigspec-v1alpha2-kops)*    | Kubelet overrides kubelet config from the ClusterSpec
machineType <br /> *string*    | NodeInstancePrefix string `json:",omitempty"` NodeLabels         string `json:",omitempty"`
maxPrice <br /> *string*    | MaxPrice indicates this is a spot-pricing group, with the specified value as our max-price bid
maxSize <br /> *integer*    | 
minSize <br /> *integer*    | 
nodeLabels <br /> *object*    | NodeLabels indicates the kubernetes labels for nodes in this group
role <br /> *string*    | Type determines the role of instances in this group: masters or nodes
rootVolumeOptimization <br /> *boolean*    | RootVolumeOptimization enables EBS optimization for an instance
rootVolumeSize <br /> *integer*    | RootVolumeSize is the size of the EBS root volume to use, in GB
rootVolumeType <br /> *string*    | RootVolumeType is the type of the EBS root volume to use (e.g. gp2)
subnets <br /> *string array*    | Subnets is the names of the Subnets (as specified in the Cluster) where machines in this instance group should be placed
taints <br /> *string array*    | Taints indicates the kubernetes taints for nodes in this group
tenancy <br /> *string*    | Describes the tenancy of the instance group. Can be either default or dedicated. Currently only applies to AWS.

### InstanceGroupList v1alpha2 kops



Field        | Description
------------ | -----------
apiVersion <br /> *string*    | APIVersion defines the versioned schema of this representation of an object. Servers should convert recognized schemas to the latest internal value, and may reject unrecognized values. More info: https://git.k8s.io/community/contributors/devel/api-conventions.md#resources
items <br /> *[InstanceGroup](#instancegroup-v1alpha2-kops) array*    | 
kind <br /> *string*    | Kind is a string value representing the REST resource this object represents. Servers may infer this from the endpoint the client submits requests to. Cannot be updated. In CamelCase. More info: https://git.k8s.io/community/contributors/devel/api-conventions.md#types-kinds
metadata <br /> *[ListMeta](#listmeta-v1-meta)*    | 





