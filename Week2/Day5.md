​
### What is remote state in Terraform and why is it important for collaborative projects?

Remote state is storing terraform code remotely as opposed to locally on a machine. This is important for collaboration because it allows moderators to be able to access the most recent version of the code from anywhere rather than just one person working locally. 
​
### What are some advantages to remote state besides being able to work collaboratively?

- Version tracking- similar to Github / conistent source of truth
- Concurrent changes - allows multiple people to make changes to the state data at the same time without overwriting other changes
- Security 
- Scalability - remote state solutions are designed to handle large - scale infrastructures

### What are some options for remote backends and how do they differ?
- Terraform Cloud 
- AWS S3 - part of the AWS platform
- Google Cloud Storage - part of the google platform
- Azure Storage - part of the microsoft platform
​
### Why is it important to not hardcode secrets, like API keys and passwords, directly into your Terraform config?

This poses a security risk to the infrastructure of the network configuration, allowing anybody access / make changes to your AWS configurations.
​
### Provide an example of where using multiple Terraform workspaces would be beneficial

Developing a web application in which a test/development environment could be deployed,  as well as the full scale production environment. This would allow an environment to "test" on before deploying to the main environment. 