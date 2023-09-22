class
---
 saclimg is incresing pods


 label is a key pair
    

This is managed service from AWS
EKS is easily created from a tool called as eksctl
Install aws cli and configure authentication for aws iam user
Lets create a config file ekscluster.yaml

--- yaml

---
apiVersion: eksctl.io/v1alpha5
kind: ClusterConfig

metadata:
  name: qteks-cluster
  region: us-east-1

nodeGroups:
  - name: ng-1
    instanceType: t2-micro
    desiredCapacity: 2


    eksctl create cluster -f <clustername>