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
# terraform state file
- terraform starte file is the blueprint (a record of existing infrastructure)
- idempotency - means your terraform configuration no matter how many times you run it, it will produce the same result. If you make a particular change it won't cause a complete change (will just apply that particular change)

- "Allow idempotency" means that an operation or system is designed to handle repeated requests or actions without causing unintended side effects or changes. If idempotency is allowed, running the same operation multiple times will always produce the same result as running it once.

For example, if an API allows idempotency for a "delete" request, you can send the same request multiple times, but the outcome will remain the same—the item will be deleted once, and subsequent requests won’t change anything further. This prevents errors from accidental duplicate requests.

## Desired vs current state
.tf (desired state) - what you want
.tfstate (current state) - what you have

The terraform state file compares your desired state to your current state (actual infrastructure). (Then you need to deploy again)

---
# Deploying infrastructure

## How is infrastructure deployed by terraform?
## How are the connections established for your deployments?
## How do I make sure to deploy things safely and not break anything?

---
# Terraform providers
- A plugin that allows you to interact with the cloud platforms, services and other technologies.
- Enables terraform to manage resources in the cloud.
---
# Terraform provider code
![Screenshot 2024-10-24 at 18 49 59](https://github.com/user-attachments/assets/36c3c54c-3e5f-495b-b743-1156cd7adc10)

---
# Terraform init (initialise)
- first command you run in any new or existing terraform project
- initialise the backend (stores the state of your infrastructure), can be stored locally or remote such as S3
- initial provider plugins - downloads provider (terraform looks at your configuration and identifies the providers you need, then downloads providers from terraform registry or other sources. Providers are like plugin which lets terrafrom communicate with the cloud ). 


