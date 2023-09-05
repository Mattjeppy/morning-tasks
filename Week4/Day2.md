# Kubernetes
​
## What is Kubernetes, and how would you explain it to someone who has never heard of it before?

Kubernetes is a powerful open-source platform for managing and orchestrating containerized applications. It is used alongside a containerisation tool (Docker), which simplifies application deployment. 
​
## Can you describe the basic components of a Kubernetes cluster (such as nodes and control plane) and their role?

A Kubernetes cluster is a collection of machines that work together to run containerized applications managed by Kubernetes.

nodes - the nodes are responsible for running containers and ensuring their health. 

control plane - the control plane components manage and control the overall state and configuration of the Kubernetes cluster
​
## How does Kubernetes ensure high availability and fault tolerance of applications within a cluster?

Replication - Kubernetes allows the user to define the desired number of replicas for applications. This ensures multiple copies of the application is running, should one fail, others are available to serve traffic

Self-healing - Kubernetes self-manages the health monitorisation of pods and nodes. It automatically restarts failed containers. 

Load-Balancing - provides a built in load balancer.
​
## What is a Kubernetes Service, and why is it important for networking and communication between Pods?

A service is an essential and powerful abstraction for managing networking and communication between Pods. It acts as a stable endpoint or entry point to a group of one or more Pods, providing a way to access the functionality offered by those Pods. 

​
## What is a Pod in Kubernetes, and why is it a fundamental building block for containerized applications?

A Pod represents a single instance of a running process in a cluster. They simplify the deployment and management of containerized applications by abstracting away many of the complexities of networking, scheduling, and resource allocation. 