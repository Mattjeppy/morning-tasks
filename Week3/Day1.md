### Imagine you need to make changes to the configuration of an existing AWS EC2 instance that's being managed by Terraform. How might you go about making those changes while minimizing disruption to your production environment?

- run terraform plan to check the change before applying
- use "lifecycle" within the EC2 to create the resource before destroying old, this will ensure no downtime
- backup / version control incase of a problem
​
### In your own words, what is a module in Terraform?

- a module is a reference to either pre-written or hidden terraform code that can be referenced and have additional data assigned to. They are reusable and allow for neater code to be written.
​
###  What are some advantages of using modules in your Terraform code?

- They are reusable and allow for neater code to be written.
- Encapsulation
- Abstraction
- They can be shared within the community 
​
### What are some instances that you might use an output block?

- to display information such as ip addresses to the developer so they can utalize the information
- Logging and monitoring  
- Use within pipelines
- Use data within scripting
​
### How can you pass arguments to a module? What steps do you need to take to add an argument?

- set a default within a variable
- use a tfvars
- enter values within the command line if not specified. 
​
### Imagine you're creating a Terraform module to deploy an AWS VPC. What are some variables you might define for this module to make it adaptable for different environments?

config for 

- VPC
- EC2 Instances
- Subnets
- Security Groups
- nat / i gws
