# DB-Monitor

# DragonBall Project Part 7

## Project Objective

For this project, you are to setup a pipeline to deploy Cluster/Application Monitoring tools: Prometheus, and Grafana into the DB cluster using Terraform with the Kubernetes and Helm Providers.

## Prerequisites

- Metrics Enabled in the values files for the following applications to allow Prometheus to track their performance:
  - Jenkins (ref: https://github.com/Ohubabs/DB-Pipeline.git)
  - SonarQube (ref: https://github.com/Ohubabs/DB-Sonarqube.git)
  - MongoDB (ref: https://github.com/Ohubabs/DB-Mongo.git)
  - Nginx-Ingress (ref: https://github.com/Ohubabs/DB-Pipeline.git)
  - Prometheus 
  - Grafana 
  

## Monitoring Pipeline 7

### Step 1: Go to New Item” from the Dashboard, select “Pipeline”, name it “Prometheus_Grafana”.

![Screenshot 2024-06-24 at 2 59 58 PM](https://github.com/user-attachments/assets/71e7db9b-444d-4925-9c7c-473c577cb3ed)

### Step 2: Go to “Configuration”, Select “Poll SCM” and Enter the details for your GitHub repo & Jenkinsfile or copy and paste the Jenkinsfile_Monitor in this repo.

![image](https://github.com/user-attachments/assets/ed435206-da9f-4b69-82c2-6b89448340ea)

#### Notes :-

- Edit the var.tf file with your Grafana credentials to be uploaded into the secret in prince.tf.

![Screenshot 2024-10-08 at 12 41 42 PM](https://github.com/user-attachments/assets/047c20fa-37e6-42e5-8d1f-d664b53c37a9)

![Screenshot 2024-10-08 at 12 35 09 PM](https://github.com/user-attachments/assets/0c3ef7c4-2d61-44b7-b89f-d96ac522342c)

- If you change the name of the secret, it must be edited as well in the graf-values.yml file

![image](https://github.com/user-attachments/assets/2748ca89-fda6-42f9-9e9f-c68f6b0f3979)


### Step 3: Click “Build now” to deploy Cluster/Application Monitoring tools: Prometheus, and Grafana into the DB cluster .

![Screenshot 2024-06-24 at 4 06 53 PM](https://github.com/user-attachments/assets/a92ec669-546d-4f61-ad09-fd5af9e18552)

![Screenshot 2024-06-24 at 3 55 20 PM](https://github.com/user-attachments/assets/a217e032-e192-47e0-802d-05d596f105a8)

![Screenshot 2024-06-24 at 3 55 25 PM](https://github.com/user-attachments/assets/1fb63cac-dcc9-4ba8-8202-59d7019f0200)

![Screenshot 2024-06-24 at 3 55 33 PM](https://github.com/user-attachments/assets/5106bef6-7573-4caa-9e7b-981bb65becd6)

![Screenshot 2024-06-24 at 4 19 02 PM](https://github.com/user-attachments/assets/5ccbf42a-a7bb-48c7-aeff-ea9bda5e6c48)

### Step 4: Once your Prometheus and Grafana sites are live, log into Grafana, set Prometheus as a data source, and gain performance stats from apps running in the cluster e.g Jenkins, SonarQube, etc...

![Screenshot 2024-06-24 at 7 26 34 PM](https://github.com/user-attachments/assets/56d983e4-b8b0-43bc-8df5-f4f92f0f4160)

![Screenshot 2024-06-24 at 7 26 41 PM](https://github.com/user-attachments/assets/9ae5922f-f024-4706-b9d4-ad770557e6ac)

![Screenshot 2024-06-24 at 7 26 44 PM](https://github.com/user-attachments/assets/534cfbf2-5dc4-4924-a92b-f45174f2f1b9)

![Screenshot 2024-06-24 at 7 26 53 PM](https://github.com/user-attachments/assets/748ca682-8e26-42db-9f2f-2d152c03e210)

![Screenshot 2024-06-24 at 7 26 58 PM](https://github.com/user-attachments/assets/d520cf98-eef8-4460-949b-a6b625286f47)

![Screenshot 2024-06-24 at 7 27 03 PM](https://github.com/user-attachments/assets/300c7d32-65e4-4514-acb9-7b296d1682ff)

![Screenshot 2024-06-24 at 7 27 38 PM](https://github.com/user-attachments/assets/a27f447d-9105-4d42-83dd-d68bb36384ff)

![Screenshot 2024-06-24 at 7 31 06 PM](https://github.com/user-attachments/assets/f3b5fc60-366d-4727-82fa-b229329ae5ef)

![Screenshot 2024-06-24 at 7 32 06 PM](https://github.com/user-attachments/assets/bdf6fc8b-3899-48cd-9247-dc0b6aa23b34)

![Screenshot 2024-06-24 at 7 32 47 PM](https://github.com/user-attachments/assets/dce58e49-f562-4d5b-93f4-caf8f18ac085)

![Screenshot 2024-06-25 at 6 40 52 PM](https://github.com/user-attachments/assets/6b9096d6-ef0d-4a9b-a8e4-4598702e86d7)




