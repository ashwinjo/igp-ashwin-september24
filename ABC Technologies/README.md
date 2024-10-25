# Industry Grade Project

This repository demonstrates the skills I have developed during the **Post Graduate Program in DevOps** certification.

---

## Business Challenge/Requirement

**ABC Technologies** is a leading online retail store that has recently acquired a large offline retail business. This business has numerous stores across the globe but is currently following a conventional pattern of development and deployment. As a result, it has incurred significant losses and is facing the following challenges:

- Low availability
- Low scalability
- Low performance
- Hard to build and maintain
- Development and deployment are time-consuming

ABC plans to acquire data from all these storage systems to utilize it for analytics and predictions regarding the firm’s growth and sales prospects. In the first phase, ABC needs to create servlets to add a product and display product details. This includes adding servlet dependencies required to compile the servlets and creating an HTML page for adding products. The team is using **Git** to manage all the source code.

ABC has decided to adopt the **DevOps** model. Once the source code is available on **GitHub**, we will integrate it with **Jenkins** to provide continuous build generation for continuous delivery. Additionally, we will integrate with **Ansible** and **Kubernetes** for deployment and use **Docker Hub** to pull and push images between Ansible and Kubernetes.

---

## The Goal of the Project

Below are some of the high-level goals of this project:

- Implement CI/CD so that ABC Company can achieve:
  1. High availability
  2. High scalability
  3. High performance
  4. Easy build and maintenance
  5. Quick development and deployment
 

## Approach to Solve

### Task 1: Clone the Project

1. Clone the project from the GitHub link shared in resources to your local machine.
2. Build the code using Maven commands.

### Task 2: Set Up Git Repository and Jenkins

1. Set up the Git repository and push the source code.
2. Log in to Jenkins.
   - Create a build pipeline containing a job for each of the following:
     - One for compiling the source code.
     - Second for testing the source code.
     - Third for packing the code.
3. Execute the CI/CD pipeline to run the jobs created in Step 2.
4. Set up a master-slave node to distribute the tasks in the pipeline.

### Task 3: Create Docker Integration

1. Write a Dockerfile.
2. Create an image and container on the Docker host.
3. Integrate the Docker host with Jenkins.
4. Create a CI/CD job on Jenkins to build and deploy in a container.
   - Enhance the package job created in Step 2 of Task 2 to create a Docker image.
   - In the Docker image, add code to move the WAR file to the Tomcat server and build the image.

### Task 4: Integrate Docker Host with Ansible

1. Write an Ansible playbook to create an image and container.
2. Integrate Ansible with Jenkins.
3. Deploy the Ansible playbook.
4. Create a CI/CD job to build code on Ansible and deploy it on the Docker container.
   - Deploy artifacts on Kubernetes.
   - Write pod, service, and deployment manifest files.
   - Integrate Kubernetes with Ansible.
   - Create an Ansible playbook to manage deployment and services.

### Task 5: Monitoring with Prometheus and Grafana

1. Use Prometheus to monitor resources such as:
   - CPU utilization (Total Usage, Usage per core, Usage breakdown)
   - Memory
   - Network on the instance by providing endpoints in localhost.
2. Install the Node Exporter and add the URL to targets in Prometheus.
3. Using this data, log in to Grafana and create a dashboard to show the metrics.
