# Index page

<br>

## 🚀 A series of practical projects    

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
> #### **Some filosophy I wrote when couldn't fell asleep**:
> I prefer learning through hands-on experience rather than just copying numerously-copied tutorials. I like to dive deep into the details understanding how and why things work, comprehending the specifics, and tackling arising challenges head-on. I also niticed that describing in writing of what you've learned helps you structure and remember stuff even better and re-produce easily when needed.
> <br>
> 
> Such approaches obviously take more time, that's why my portfolio is not that extensive. But I believe, following this path, what you've learned stays with you forever.
> 
> This inspired me to launch a series where I took a sample NodeJS web application, thoroughly grasped its workings, and experimented with diverse DevOps and Cloud technologies. The initial design of the app is not mine. I just took the > sample one and modified it slightly.
> <br>
> 
> I began with basic steps, such as simply deploying the application on servers, and then progressively advanced, delving into more complex aspects while exploring current DevOps and Cloud concepts.
> 
> <br><br>
> 
> 
> <p align="center">
>     <img width="500" src="https://github.com/otam-mato/projects_landing_page/assets/113034133/2f4f43e4-583a-440e-b3c1-3f38674417a9">
> </p>
> <p align="center">
>     <img width="500" src="https://github.com/otam-mato/projects_landing_page/assets/113034133/70b881af-a7af-4bb1-a431-2aa23e8905da">
> </p>
> 
> </details>

![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) 
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)

<br>

✍️ **1. [Deploying the app on AWS EC2 and RDS instances](https://github.com/otam-mato/nodejs_mysql_web_app_terraform)** <br>

&nbsp;&nbsp;&nbsp;&nbsp; In the first project I used **Terraform** as an **IaC [Infrastructure as Code]** tool to **Automate** creating the infrastructure on **AWS**. And explored the basic deployment - on **EC2** + **RDS** instances.
 <br><br>
✍️ **2. [Migrating MySQL --> MongoDB with a Python script. Deploying the app on the EC2 instance](https://github.com/otam-mato/nodejs_mongodb_web_app_awscloudformation)** <br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;What if we need using a **NoSQL** database instead of **SQL** while using the existing **SQL** data? Here, I worked out a **Python** script to convert **SQL** data to **JSON**, migrated the database to **MongoDB**, and tweaked the app to talk to **MongoDB** instead of **MySQL**. Finally, I deployed it on two **EC2** instances.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;For the infrastructure provisioning, I opted for **AWS CloudFormation** as the Infrastructure as Code (IaC) tool instead of **Terraform**.<br><br>
✍️ **3. [Docker Container Deployment for Application Portability](https://github.com/otam-mato/nodejs_mysql_web_app_docker)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Embracing **Docker** for its portability advantages, I encapsulated the application within containers, facilitating deployment unburdened by traditional constraints and pushed them to my **DockerHub**. This approach streamlined the journey of the application.<br><br>
✍️ **4. [Kubernetes Deployment and "Canary" Strategy](https://github.com/otam-mato/nodejs_mysql_web_app_kubernetes)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Then, following the logical path I transitioned the Dockerized app into **Kubernetes**, orchestrating the deployment of the application within a **Kubernetes** cluster launched on **AWS EKS**. The follwing introduction of a **"Canary"** deployment strategy deploying ensured a gradual transition to a new version #2, minimizing user impact.

✍️ **5. [ELK Stack Implementation for Log Monitoring and Observability (ElasticSearch, Logstash, Kibana)](https://github.com/otam-mato/nodejs_mysql_web_app_elk)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The next is **Observability**. I used **ELK** stack—**ElasticSearch, Logstash, Kibana**—to set up comprehensive log monitoring capabilities.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; To log every HTTP request sent to the server, I modified the app and involved **"Bunyan logger"** (a JS logging library) <br><br>
✍️ **6. [Prometheus and Grafana Monitoring set up with Docker Compose](https://github.com/otam-mato/nodejs_mysql_web_app_prometheus_grafana)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Observability** again. Here I set up monitoring of the app's metrics with **Prometheus** and **Grafana** to deliver the real-time visual data and watch the application performance. Deployed the stack using **Docker Compose**.<br><br>
✍️ **7. [Ansible-Driven Setup of Prometheus and Grafana](https://github.com/otam-mato/nodejs_mysql_web_app_prometheus_grafana_ansible)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;And again **Observability**. The same stack but setting it up with **Ansible**.<br><br>
✍️ **8. [Jenkins-Based CICD Pipeline to Kubernetes on AWS EKS. Testing with MochaJS+ChaiJS libraries](https://github.com/otam-mato/nodejs_mysql_web_app_jenkins_AWS)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The implementation of a **Continuous Integration/Continuous Deployment (CICD)** pipeline using **Jenkins** facilitated the deployment of the application on **Kubernetes** within **AWS Elastic Kubernetes Service (EKS)**. To be closer to the real-world use cases, the pipeline incorporated testing stages for unit and end-to-end testing. I modified the app to involve **MochaJS** and **ChaiJS** testing libraries<br><br>
✍️ **9. [DevSecOps Integration and CICD Pipeline Refinement for Azure AKS](https://github.com/otam-mato/nodejs_mysql_web_app_jenkins_azure_devsecops)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Next, I switched to **MS Azure** and re-build the **CICD** pipeline and integrating **DevSecOps** stages to scan the app for vulnerabilities using **Trivy, SonarQube** and **OWASP** dependency check which is an important security practice.<br>

✍️ **10. [Deploying with HELM on Azure AKS](https://github.com/otam-mato/nodejs_mysql_web_app_helm_azure_aks_deployment)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Leveraging **HELM** charts, I orchestrated the deployment of the web application again on **Microsoft Azure's AKS**. The introduction of a second version of the app allowed for controlled rollouts and rollbacks, ensuring a seamless and controlled deployment process.


✍️ **11. [Setting up a Service Mesh with Istio. Demo for the Observability and traffic management](https://github.com/otam-mato/istio_nodejsapp_demo.git)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Introducing **Istio** as a service mesh solution, I configured **Observability** features using **Kiali, Jaeger, Prometheus,** and **Grafana**. The implementation showcased a **Blue-Green** and **Canary** deployment strategies, providing fine-grained control over traffic management.

<br><br>

## Various Cloud:

✍️ **1. [Logging and monitoring a user activity on a server with AWS Cloudwatch](https://github.com/otam-mato/AWS_CloudWatch_logging_and_monitoring.git)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Logging and monitoring a user activity on a server with **AWS Cloudwatch**.

✍️ **2. [Deploying a static web-site to AWS S3 with GitHub Actions](https://github.com/otam-mato/otam-mato.github.io.git)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Deploying a static web-site to **AWS S3** and involving **AWS Route53**, **AWS CloudFront** and **AWS CertificateManager** to implement TLS.


<br><br>

## Various Software Development:

✍️ **1. [Front-end experiment with OpenAI API](https://github.com/otam-mato/ChatAI_frontend_app.git)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The frontend experiment to interact with **OpenAI API**. The **JavaScript** code handles the main functionality of your chat interface, including API interactions, updating the UI and managing the question history.

✍️ **2. [Client-Server experiment with OpenAI API](https://github.com/otam-mato/ChatAI_frontend_app.git)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Re-enginering the previous solution (ChatAI) to use the client-server architecture. Involves node.js to set up a backend server<br>

✍️ **2. [Front-end snake game](https://github.com/otam-mato/snake_game.git)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Couldn't sleep well and made a game which I liked when had a Nokia mobilephone.

✍️ **3. [JavaScript code de-obfuscation / re-engineering](https://github.com/otam-mato/JavaScript_de-obfuscation_re-engineering.git)**<br>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;De-obfuscating the heavily obfuscated code to solve the puzzle.
