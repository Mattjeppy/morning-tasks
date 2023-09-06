1. What is Kubernetes internal DNS, and why is it essential for containerized applications within a cluster?

it's a component of a Kubernetes cluster that specifically provides Domain Name System (DNS) services within a cluster. It is essential for several reasons, such as pod to pod communication, load balancing, abstracting networking and communication.
​
2. Can you explain the concept of a Kubernetes ReplicaSet and why it's useful for maintaining a specified number of pod replicas?

a ReplicaSet is a resource object used to ensure that a specified number of replicas (identical copies) of a pod are running at all times within a cluster.  It simplifies the management of pods, automates the recovery from failures, supports controlled updates, and aligns with Kubernetes' declarative model for infrastructure management.
​
3. In your own words what is the difference between a ClusterIP, NodePort, and LoadBalancer service types?

ClusterIP is for internal cluster communication, NodePort is for external access to services on a specific port, and LoadBalancer is for high-availability external access with traffic distribution and a public IP or DNS name. 
​
4. If you have a front and backend, what service might be best to use to expose the backend to the frontend?

If it's internal, then ClusterIP would be the most appropriate service. 
​
5. What is service discovery in Kubernetes and what is it's purpose?

service discovery in Kubernetes is a key feature that simplifies the way applications find and connect to other services within the cluster. It abstracts network complexities, provides automated load balancing, supports namespace isolation, and ensures that applications can adapt to changes in the cluster's state. 