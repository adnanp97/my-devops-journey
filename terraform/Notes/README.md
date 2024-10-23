# Terraform and Infrastructure as code
---
# Terraform introduction
## What is Infrastructure as Code ?
- used to deploy resources as code instead of manually in the cloud
## Benefits
- easy to adjust, replicate and scale
- manually is tedious and prone to error
---
# Infrastrcuture as code (IaC)
- terraform is a cloud agnostic tool, which means it can deploy to any cloud and different providers. It can also deploy kubernetes resources. It is a tool that can deploy on many different providers, this is done through terraform registry where it can install certain plugins and certain api call in order to provide two separate providers.
---
# IaC with version control
- can be stored in git, track changes, collaborate and got back to different versions

Collaboration: members of team, deploying to same infrastructure, each pushing different bits of code. This is usually managed by the terraform state file and the terraform lock file.
---
# Infra orchestration vs Config managenment

## config management
### config management tools
- ansible, puppet, chef etc

### orchestration tools
- terraform, cloud formation etc

### how do cofig management tools and orechestration tools work together?
- Assume terraform is used to deploy servers such as EC2 instances
- Ansible will then be used to configure EC2 instances and serves to run certain things such as hosting wordpress server (in AWS module)
---
# what is terraform?
- IaC tool
- cloud agnostic
- practioner -> deployes IaC -> runs a terraform plan (plan - tells you what code is trying to do. compares current IaC attempted to get desired stared compared with current state) -> then run apply (applies IaC code) -> resources deployed in the cloud (includes the creation, updating and versioning of these resources)
---
# Tips for using terraform
- terraform documentation https://developer.hashicorp.com/terraform/tutorials?product_intent=terraform
- testing and validation
- start with a small MVP (minimum viable product) and then iterate (configure resource that you need in order to deploy into cloud and then iterate e.g. add variables, make modules)
- Implement Dry software engineering principle (less duplicates e.g. use modules)
---
# download terraform
