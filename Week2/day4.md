### What is infrastructure as code (IaC) and why is it important in modern IT operations? What are the advantages?

Infrastructure as code is fairly self-explanatory, it's creating a cloud infrastructure, (VPCs, EC2s) etc using tools such as terraform (using code). Although some time needs to be spent learning the syntax and layout, having IaC means a cloud engineer can quickly whip up an infrastructure in seconds as opposed to using the AWS console, which is a lot more time consuming. Similarly, it can be torn down quickly. This is important because it allows efficient cloud infrastructuring, version control, reducing company time / costs spent on repetitive tasks aswell as reducing human error.
​
### Explain the concept of "Infrastructure as Code" (IaC) and how Terraform fits into this concept.

IaC is another DevOps / cloud methodology, treating cloud infrastructure as software development. Terraform fits into the concept because it allows that exact methodology to take place and TDD is possible within it, just like SD. 
​
### What problems do modules help address, and how do they promote reusability?

As infrastructure code grows, having different modules allows reusable code (similar to functions) to be imported in and used within the main.tf structure of our IaC avoiding repetition. This means managing the infrastructure is made easier, looks cleaner and much more easier to scale.  
​
### Explain in your own words what the following commands achieve;
​
- `terraform init`

Similar to GitHub, terraform init allows us to initialise a terraform working directory.
​
- `terraform plan`
This command is to preview the changes that will be made to your infrastructure before actually applying those changes.
​
- `terraform apply`
This command applys any changes that have been made to the IaC. terraform asks you to confirm you want to apply those changes before doing so.
​
- `terraform destroy`
Destroy tears down any infrastructure that has been created within your current directory. Again, terraform asks you to confirm these changes.
​
- `terraform fmt`
fmt formats your code so it is readable / formatted nicely.
​
- `terraform output`
This command is used to display the values of outputs defined in the configuration of the terraform.
​
- `terraform taint`
This command you give an arguement of a resource which you would like to mark as being "tainted" and destroyed within your cloud infrastructure, before being replaced. 

e.g.
terraform taint aws_instance.example