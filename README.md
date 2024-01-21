# Index page

<br>

## 🚀 A series of practical projects    

<br>

I prefer learning through hands-on experience rather than just copying numerously-copied tutorials. I like to dive deep into the details understanding how and why things work, comprehending the specifics, and tackling challenges head-on. 
<br>

Such approach obviously takes more time, probably that's why my portfolio is not that extensive. But I believe, following this path, what you've learned stays with you forever.

This inspired me to launch a series where I took a sample NodeJS web application, thoroughly grasped its workings, and experimented with diverse DevOps and Cloud technologies. The initial design of the app is not mine. I just took the sample one and modified it slightly.
<br>

I began with basic steps, such as simply deploying the application on servers, and then progressively advanced, delving into more complex aspects while exploring current DevOps and Cloud concepts.

<br><br>


<p align="center">
    <img width="500" src="https://github.com/otam-mato/projects_landing_page/assets/113034133/2f4f43e4-583a-440e-b3c1-3f38674417a9">
</p>
<p align="center">
    <img width="500" src="https://github.com/otam-mato/projects_landing_page/assets/113034133/70b881af-a7af-4bb1-a431-2aa23e8905da">
</p>

<br>

> **Basic functionality**
>
> This sample two-tier web application interfaces with a MySQL database, facilitating CRUD (Create, Read, Update, Delete) operations on the database records.
>
> **<details markdown=1><summary markdown="span">Detailed app description</summary>**
>
> ## Summary
>
> The app sets up a web server for a supplier management system. It allows viewing, adding, updating, and deleting suppliers. 
> 
> #### **Dependencies and Modules**:
>   - **express**: The framework that allows us to set up and run a web server.
>   - **body-parser**: A tool that lets the server read and understand data sent in requests.
>   - **cors**: Ensures the server can communicate with different web addresses or domains.
>   - **mustache-express**: A template engine, letting the server display dynamic web pages using the Mustache format.
>   - **serve-favicon**: Provides the small icon seen on browser tabs for the website.
>   - **Custom Modules**: 
>     - `supplier.controller`: Handles the logic for managing suppliers like fetching, adding, or updating their details.
>     - `config.js`: Keeps the server's settings for connectind to the MySQL database.
>
> #### **Configuration**:
>   - The server starts on a port taken from a setting (like an environment variable) or uses `3000` as a default.
>
> #### **Middleware**:
>   - It's equipped to understand data in JSON format or when it's URL-encoded.
>   - It can chat with web pages hosted elsewhere, thanks to CORS.
>   - Mustache is the chosen format for web pages, with templates stored in a folder named `views`.
>   - There's a public storage (`public`) for things like images or stylesheets, accessible by anyone visiting the site.
>   - The site's tiny browser tab icon is fetched using `serve-favicon`.
>
> #### **Routes (Webpage Endpoints)**:
>   - **Home**: `GET /`: Serves the home page.
>   - **Supplier Operations**: 
>     - `GET /suppliers/`: Fetches and displays all suppliers.
>     - `GET /supplier-add`: Serves a page to add a new supplier.
>     - `POST /supplier-add`: Receives data to add a new supplier.
>     - `GET /supplier-update/:id`: Serves a page to update details of a supplier using its ID.
>     - `POST /supplier-update`: Receives updated data of a supplier.
>     - `POST /supplier-remove/:id`: Removes a supplier using its ID.
>
> #### **Starting Up**:
>   - The server comes to life, starts listening for visits, and announces its awakening with a log message.
>
> </details>

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) 
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)

<br>

## Projects:

✍️ **1. [Deploying the app on AWS EC2 and RDS instances](https://github.com/otam-mato/nodejs_mysql_web_app_terraform)** <br>

&nbsp;&nbsp;&nbsp;&nbsp; In the first project I used **Terraform** as an IaC [Infrastructure as Code] tool to automate creating the infrastructure on **AWS**. And then deployed the app on the created **EC2** + **RDS** instances.
 <br><br>
✍️ **2. [Migrating MySQL --> MongoDB with a Python script. Deploying the app on the EC2 instance](https://github.com/otam-mato/nodejs_mongodb_web_app_awscloudformation)** <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;What if the use case suggests using a **NoSQL** database instead of **SQL** and we need to convert the existing **SQL** data? So, I created a **Python** script to convert **SQL** data to **JSON**, migrated it to MongoDB, and tweaked the app to talk to **MongoDB** instead of **MySQL**. Finally, I deployed it on two **EC2** instances.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;For the infrastructure provisioning, I opted for AWS CloudFormation as the Infrastructure as Code (IaC) tool instead of Terraform.<br><br>
✍️ **3. [Building and deploying the app on Docker containers](https://github.com/otam-mato/nodejs_mysql_web_app_docker)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Embracing **Docker** for its portability advantages, I encapsulated the application within containers, facilitating deployment unburdened by traditional constraints and pushed them to my **DockerHub**. This approach streamlined the journey of the application.<br><br>
✍️ **4. [Deploying the app on Kubernetes. "Canary" deployment](https://github.com/otam-mato/nodejs_mysql_web_app_kubernetes)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Then, following the logical path I transitioned the Dockerized app into **Kubernetes**, orchestrating the deployment of the application within a **Kubernetes** cluster launched on **AWS EKS**. The follwing introduction of a **"Canary"** deployment strategy deploying ensured a gradual transition to a new version #2, minimizing user impact.

✍️ **5. [Monitoring the app's logs with ELK stack (ElasticSearch, Logstash, Kibana)](https://github.com/otam-mato/nodejs_mysql_web_app_elk)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Setting up monitoring of the application logs using 'bunyan' library and ELK stack (Elastic search, Logstash, Kibana).<br><br>
✍️ **6. [Monitoring the app with Prometheus and Grafana. Deploying with Docker Compose](https://github.com/otam-mato/nodejs_mysql_web_app_prometheus_grafana)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Setting up monitoring of the app with Prometheus and Grafana using Docker Compose.<br><br>
✍️ **7. [Monitoring the app with Prometheus and Grafana. Deploying with Ansible](https://github.com/otam-mato/nodejs_mysql_web_app_prometheus_grafana_ansible)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Setting up monitoring of the app with Prometheus and Grafana using Ansible.<br><br>
✍️ **8. [Building CICD pipeline with Jenkins to deploy the app on Kubernetes AWS EKS. Testing with MochaJS+ChaiJS libraries](https://github.com/otam-mato/nodejs_mysql_web_app_jenkins_AWS)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Building CICD pipeline with Jenkins to deploy the app on Kubernetes. Implement testing stages (unit and end-to-end testing) with MochaJS and ChaiJS<br><br>
✍️ **9. [Implementing DevSecOps stages and re-building the CICD pipeline to deploy the app on Azure AKS](https://github.com/otam-mato/nodejs_mysql_web_app_jenkins_azure_devsecops)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Re-building the CICD pipeline to deploy the app on AKS Azure and integrating DevSecOps stages to scan the app for vulnerabilities using Trivy, SonarQube and OWASP dependency check.<br>

✍️ **10. [Deploying with HELM on Azure AKS](https://github.com/otam-mato/nodejs_mysql_web_app_helm_azure_aks_deployment)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Deploying the web application on MS Azure AKS using HELM. Subsequently, I am introducing the second version of the app and then rollback to the first version.

✍️ **11. [Setting up a Service Mesh with Istio. Demo for the Observability and traffic management](https://github.com/otam-mato/istio_nodejsapp_demo.git)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Setting up the service mesh with Istio and demonstrate observability features with Kiali, Jaeger, Prometheus and Grafana as well as traffic management using "Canary" deployment.
