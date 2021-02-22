# terraform-eks-deploy
I will create a ekscluster using Ansible, here I will speicify the size of this cluster to scale up deppending on my computing needs
Main.tf is the terraform configuration script that will automate the build spec of eks clusters and node specification, as well as, policys and permissions. It will create the build based on vpc needs, private/public subnets etc. All the necessary componets needed for this build.
Deployment.yml is the kubernetes container that will be deployed
Also, added an ingress.yml which serves as a Application load balancer for these clusters, this os opitional and if you do not need this then you could remove line 74 and 76-81. 
