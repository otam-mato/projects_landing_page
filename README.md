# Index page

<br>

## 🚀 A series of practical projects

<br>

Just took the same sample NodeJS web application and juggled it applying diverse DevOps and Cloud technologies.

<br>

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)

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

<br>

## Projects:

✍️ 1. **[Deploying the app on AWS EC2 and RDS instances](https://github.com/otam-mato/nodejs_mysql_web_app_terraform)** <br>
&nbsp;&nbsp;&nbsp;&nbsp; In this setting I automate creating the infrastructure on AWS with Terraform and deploy the app on EC2 + RDS instances.
 <br><br>
✍️ 2. **[Migrating MySQL --> MongoDB with a Python script. Deploying the app on the EC2 instance](https://github.com/otam-mato/nodejs_mongodb_web_app_awscloudformation)** <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In this installment I migrate the MySQL database to MongoDB and launch the app on two EC2 instances within the AWS infrastructure.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;For the infrastructure provisioning, I opted for AWS CloudFormation as the Infrastructure as Code (IaC) tool instead of Terraform.<br><br>
✍️ 3. **[Building and deploying the app on Docker containers](https://github.com/otam-mato/nodejs_mysql_web_app_docker)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The current installment involves deploying the web app in contaners with Docker.<br><br>
✍️ 4. **[Deploying the app on Kubernetes. "Canary" deployment](https://github.com/otam-mato/nodejs_mysql_web_app_kubernetes)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Deploying the Dockerized version of the web application within a Kubernetes cluster. Subsequently, I'm introducing the second version of the app using the "canary" deployment strategy, and routing approximately 33% of incoming traffic to this new version.<br><br>
✍️ 5. **[Monitoring the app's logs with ELK stack (ElasticSearch, Logstash, Kibana)](https://github.com/otam-mato/nodejs_mysql_web_app_elk)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the current installment, I am setting up monitoring of the application logs using 'bunyan' library and ELK stack (Elastic search, Logstash, Kibana).<br><br>
✍️ 6. **[Monitoring the app with Prometheus and Grafana. Deploying with Docker Compose](https://github.com/otam-mato/nodejs_mysql_web_app_prometheus_grafana)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the current installment, I am setting up monitoring of the app with Prometheus and Grafana using Docker Compose.<br><br>
✍️ 7. **[Monitoring the app with Prometheus and Grafana. Deploying with Ansible](https://github.com/otam-mato/nodejs_mysql_web_app_prometheus_grafana_ansible)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the current installment, I am setting up monitoring of the app with Prometheus and Grafana using Ansible.<br><br>
✍️ 8. **[Building CICD pipeline with Jenkins to deploy the app on Kubernetes AWS EKS. Testing with MochaJS+ChaiJS libraries](https://github.com/otam-mato/nodejs_mysql_web_app_jenkins_AWS)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the current installment, I am building CICD pipeline with Jenkins to deploy the app on Kubernetes. Implement testing stages (unit and end-to-end testing) with MochaJS and ChaiJS<br><br>
✍️ 9. **[Implementing DevSecOps stages and re-building the CICD pipeline to deploy the app on Azure AKS](https://github.com/otam-mato/nodejs_mysql_web_app_jenkins_azure_devsecops)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the current installment, I am re-building the CICD pipeline to deploy the app on AKS Azure and integrating DevSecOps stages to scan the app for vulnerabilities using Trivy, SonarQube and OWASP dependency check.<br>

✍️ 10. **[Deploying with HELM on Azure AKS](https://github.com/otam-mato/nodejs_mysql_web_app_helm_azure_aks_deployment)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the current installment, I am deploying the web application on MS Azure AKS using HELM. Subsequently, I am introducing the second version of the app and then rollback to the first version.

✍️ 11. **[Setting up a Service Mesh with Istio. Demo for the Observability and traffic management](https://github.com/otam-mato/istio_nodejsapp_demo.git)**<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;In the current installment, I am setting up the service mesh with Istio and demonstrate observability features with Kiali, Jaeger, Prometheus and Grafana as well as traffic management using "Canary" deployment.
