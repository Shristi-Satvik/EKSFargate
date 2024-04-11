### Prerequisites: 

> kubectl – A command line tool for working with Kubernetes clusters. For more information, see Installing or updating kubectl.

> eksctl – A command line tool for working with EKS clusters that automates many individual tasks. For more information, see Installing or updating.

### Install AWS CLI 

As the first step, you need to install AWS CLI as we will use the AWS CLI (`aws configure`) command to connect Terraform with AWS in the next steps.

Follow the below link to Install AWS CLI.
```
https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
```

### create a EKS cluster
### Install using Fargate

```
eksctl create cluster --name demo-cluster --region us-east-1 --fargate
```


### Install Terraform

Next, Install Terraform using the below link.
```
https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli
```

### Connect Terraform with AWS

Its very easy to connect Terraform with AWS. Run `aws configure` command and provide the AWS Security credentials as shown in the video.

### Initialize Terraform

Clone the repository and Run `terraform init`. This will intialize the terraform environment for you and download the modules, providers and other configuration required.

### Optionally review the terraform configuration

Run `terraform plan` to see the configuration it creates when executed.

### Finally, Apply terraform configuation to create EKS cluster with VPC 

`terraform apply`



## Delete the cluster

```
eksctl delete cluster --name demo-cluster --region us-east-1
```