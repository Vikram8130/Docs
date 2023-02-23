### Attach prevoiusly created IAM role to the Jenkins Server(having eks cluster config file)
For communication between Jenkins server and EKS cluster 


### Jenkins server setup with Helm to deploy into Kubernetes cluster

## Download and Install helm 
```sh
curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
```

## Test with helm command
```sh
helm version
helm list
```

## Copy config file from EKS Management host to Jenkins home directory 
(For connectivity between Jenkins Server and EKS Cluster)
```sh
mkdir /var/lib/jenkins/.kube
copy config file under .kube directory with jenkins ownership

chmod 600 /var/lib/jenkins/.kube/config
helm repo list 
 
```









