# Index page

## 🚀 A series of practical projects inspired by the idea to take the same sample NodeJS web application and juggle it applying diverse DevOps technologies.

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)

**Basic functionality**

This sample two-tier web application interfaces with a MySQL database, facilitating CRUD (Create, Read, Update, Delete) operations on the database records.

**<details markdown=1><summary markdown="span">Detailed app description</summary>**

## Summary

The app sets up a web server for a supplier management system. It allows viewing, adding, updating, and deleting suppliers. 

#### **Dependencies and Modules**:
   - **express**: The framework that allows us to set up and run a web server.
   - **body-parser**: A tool that lets the server read and understand data sent in requests.
   - **cors**: Ensures the server can communicate with different web addresses or domains.
   - **mustache-express**: A template engine, letting the server display dynamic web pages using the Mustache format.
   - **serve-favicon**: Provides the small icon seen on browser tabs for the website.
   - **Custom Modules**: 
     - `supplier.controller`: Handles the logic for managing suppliers like fetching, adding, or updating their details.
     - `config.js`: Keeps the server's settings for connectind to the MySQL database.

#### **Configuration**:
   - The server starts on a port taken from a setting (like an environment variable) or uses `3000` as a default.

#### **Middleware**:
   - It's equipped to understand data in JSON format or when it's URL-encoded.
   - It can chat with web pages hosted elsewhere, thanks to CORS.
   - Mustache is the chosen format for web pages, with templates stored in a folder named `views`.
   - There's a public storage (`public`) for things like images or stylesheets, accessible by anyone visiting the site.
   - The site's tiny browser tab icon is fetched using `serve-favicon`.

#### **Routes (Webpage Endpoints)**:
   - **Home**: `GET /`: Serves the home page.
   - **Supplier Operations**: 
     - `GET /suppliers/`: Fetches and displays all suppliers.
     - `GET /supplier-add`: Serves a page to add a new supplier.
     - `POST /supplier-add`: Receives data to add a new supplier.
     - `GET /supplier-update/:id`: Serves a page to update details of a supplier using its ID.
     - `POST /supplier-update`: Receives updated data of a supplier.
     - `POST /supplier-remove/:id`: Removes a supplier using its ID.

#### **Starting Up**:
   - The server comes to life, starts listening for visits, and announces its awakening with a log message.

</details>

### Projects:

✍️ 1. [Deploying the app on AWS EC2 and RDS instances](https://github.com/otam-mato/nodejs_mysql_web_app_terraform) <br>
&nbsp;&nbsp;&nbsp; In this setting I automate creating the infrastructure on AWS with Terraform and deploy the app on EC2 + RDS instances.
 <br>
✍️ 2. [Migrating MySQL --> MongoDB with a Python script. Deploying the app on the EC2 instance](https://github.com/otam-mato/nodejs_mongodb_web_app_awscloudformation)<br>
✍️ 3. [Building and deploying the app on Docker containers](https://github.com/otam-mato/nodejs_mysql_web_app_docker)<br>
✍️ 4. [Deploying the app on Kubernetes. "Canary" deployment](https://github.com/otam-mato/nodejs_mysql_web_app_kubernetes)<br>
✍️ 5. [Monitoring the app's logs with ELK stack (ElasticSearch, Logstash, Kibana)](https://github.com/otam-mato/nodejs_mysql_web_app_elk)<br>
✍️ 6. [Monitoring the app with Prometheus and Grafana. Deploying with Docker Compose](https://github.com/otam-mato/nodejs_mysql_web_app_prometheus_grafana)<br>
✍️ 7. [Monitoring the app with Prometheus and Grafana. Deploying with Ansible](https://github.com/otam-mato/nodejs_mysql_web_app_prometheus_grafana_ansible)<br>
✍️ 8. [Building CICD pipeline with Jenkins to deploy the app on Kubernetes AWS EKS. Testing with MochaJS+ChaiJS libraries](https://github.com/otam-mato/nodejs_mysql_web_app_jenkins_AWS)<br>
✍️ 9. [Implementing DevSecOps stages and re-building the CICD pipeline to deploy the app on Azure AKS](https://github.com/otam-mato/nodejs_mysql_web_app_jenkins_azure_devsecops)<br>
✍️ 10.[Deploying with HELM on Azure AKS](https://github.com/otam-mato/nodejs_mysql_web_app_helm_azure_aks_deployment)<br>

