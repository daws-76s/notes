HD, Cloud drives

HD sits near to computer, as near as possible
Cloud drives are network drives like NFS..

storage is very crucial

static provisioning
---------------------
EBS, EFS
Elastic block store --> HD
Elastic file system --> NFS

static
-----------
1. first we need to create storage, either storage admin or k8 admin will create the storage
2. we need to make this volume available to k8 cluster. we should install drivers. aws-ebs-csi drivers should be installed
3. a proper role should be attached to ec2 instance to access EBS.

kubernetes volume objects/resources
------------------------------
persistant volume --> it represents the external storage.
persistant volume claim --> pods should request volume through pvc.

1. when you apply, where your pod is getting created? any worker node

kubectl label nodes ip-192-168-53-69.ec2.internal zone=1b

dynamic provisioning
---------------------
1. volume should be created automatically.
2. there is another object called storageClass that can create storage dynamically based on the request.

here external volume and pv would be created automatically by storageClass...


since storageClass is cluster level resource, admins should create this.

EBS will have one storageclass cluster wide.

EFS static
--------------------
1. create EFS filesystem
2. edit the security group, so that it will allow port 2049 from worker nodes.
3. we should have drivers installed

kubectl kustomize \
    "github.com/kubernetes-sigs/aws-efs-csi-driver/deploy/kubernetes/overlays/stable/ecr/?ref=release-1.7" > private-ecr-driver.yaml
	give ec2 roles efs full access
4. create pv
5. create pvc
6. use pvc in the pod