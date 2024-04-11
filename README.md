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

## Delete the cluster

```
eksctl delete cluster --name demo-cluster --region us-east-1
```
