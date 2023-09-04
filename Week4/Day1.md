# Docker
​
## What is containerization, and how does it differ from virtualization?

Containerization and virtualization are two different approaches to managing and deploying applications and services. Each compartment (container) holds an application and its dependencies, but they all share the same underlying system. containerization is more lightweight and efficient because it shares resources between containers, while virtualization provides stronger isolation but is typically heavier on resources because each virtual machine is like a full computer. Virtualization is like having multiple separate boxes (virtual machines) on one physical machine, each with its own complete operating system. These virtual machines don't share the same underlying system.
​

2. Why is containerization important in modern software development and deployment?
​
Containerization is important because it's an efficient resource in terms of packaging and running applications. It aligns with devops principles of organisation and manageable deployment. 

3. What is the difference between an image and a container in Docker?

An image is a lightweight, standalone, and executable package that includes everything needed to run a piece of software, including the code, runtime, libraries, and system tools. A container is a running instance of a Docker image.
​
4. Can you give an example of a situation where you might choose to use Docker containers in a software development project?

Developing and testing a web application


​
5.If you were tasked with explaining Docker to someone who has never heard of it before, how would you describe it in a few sentences?

Docker is a technology that simplifies how we build, package, and run software applications. It bundles everything your app needs, like code, libraries, and settings, into a single, portable unit called a container. These containers are consistent and can run on any system that supports Docker, making it easier to develop, test, and deploy software across different environments. 
​
## Extension
​
Fill in this cheat sheet throughout the day to help and remind you understand how to use Docker commands
​
| Command | Description |
| :-----: | ----------- |
|   ps    |
| images  |
|  pull   |
|  build  |
|   run   |
|  stop   |
​
| Flag | Description  
|:------:|---------------------------------------------------
| -a |
| -d |
| -t |
| -p |
​
Below is an example of a how you might format a docker command. (In documentation having something wrapped in square brackets [] denotes that it is optional to provide this in the command)
​
```bash
docker run [OPTIONS] <IMAGE[:TAG|@DIGEST]> [COMMAND] [ARG...]
```