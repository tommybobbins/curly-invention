# EKS Managed Node Group Example

```
$ aws eks --region eu-west-2 update-kubeconfig --name $(aws eks list-clusters --region=eu-west-2 --query 'clusters[]' --output text)
Added new context arn:aws:eks:eu-west-2:1234567789:cluster/ex-curly-invention to ~/.kube/config
$ kubectl get nodes
NAME                                         STATUS   ROLES    AGE   VERSION
ip-10-123-34-34.eu-west-2.compute.internal   Ready    <none>   19m   v1.28.2-eks-a5df82a
ip-10-123-43-32.eu-west-2.compute.internal   Ready    <none>   26m   v1.28.2-eks-a5df82a
```

