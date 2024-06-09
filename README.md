# Connecting Instance with MobaXterm

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/4881d1bf-e259-4d2f-8465-1ee496e67a1d)

Click on **session**
click on **SSH**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/aa15c01f-b2c9-48f8-969b-a7314a213cdf)


After clickin on **ok** you will get on error

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/1d375f07-e5f4-458e-8638-4e6f04afddf5)

To resolve this error 

Go to **EC2 instance**

Click on **SEcurity Group**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/2aaa4cb9-7be3-4719-86bf-4276d7baaf25)

Click on **Edit inbound rules**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/8bea75fd-d1dd-42fc-a01f-f611a27fd80d)

**Add rules**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/66db0f4c-5687-41eb-9544-67517662935b)

Click on **Save Rules**

Again go to MobaXterm and Press **R** to restart the session

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/b053feed-93c2-4a59-8e96-78e0689f3327)

coneection successfull


![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/6bdfa9ab-7f53-4789-b624-072dcd8745d8)

Command to **install AWSCLI & install Unzip**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/1ee0355d-de28-4d7c-bff4-ccde222b7d9a)

Command to unzip

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/a4058fab-7aca-4a98-8418-dc3df6f5e6ac)

Command to install AWS


![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/c8994951-f36e-4ea7-a7f0-638c4797fcf7)

Command to Configure AWS

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/1569bea4-3f45-4714-a657-db5e50f6703a)

For access Id 

Go to **IAM user**

click on **SECurity Credentials**


click on **create access key**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/01ffa759-2db7-470f-b129-974a6a800a67)

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/9c6b77e5-bf5b-40fc-b5b1-d9193a9ab0a2)

we created the key successfully

Download the csv fil for the credentials

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/c0bfa3ee-c3cb-4aed-82fc-6b36672a62f8)

steps to configure AWS

Write the region name according to your region
and keep default output format as blank

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/d903af9a-559f-4fb0-8778-39ca310f68ca)

To check it is configure or not 

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/7c54d45f-74ef-47c3-a84a-fe69aae89ac2)


Command to install kubectl

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/1a8c6dc7-3337-4c82-9212-407ec2d3fb13)


Command to install eksctl

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/8ba11cd7-7cf2-4bbb-b366-6946becbb40d)


Creation of EKS Cluster

eksctl create cluster --name=my-eks924 \
                      --region=ap-south-1 \
                      --zones=ap-south-1a,ap-south-1b \
                      --version=1.30 \
                      --without-nodegroup



![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/8d29171d-c89e-40eb-a181-19facdd34a3a)



Till execution of this command we will setup jenkins in anothr tab using the same session

For that just double click on user

First step **Installation of Java**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/8df7e31e-3d27-461e-a45d-e5051a324c92)

**installation oif jenkins**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/f2537ec8-1009-472e-83cb-930844a2b5ba)

To access Jenkins copy te public ip address and open it on port 8080

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/b6800bb8-2286-4333-a0c7-8bf8ffd79f09)

To get the password of jenkins use below command


![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/a6411405-a062-45b5-b4f2-86ba374c45f7)

One pop up is coming click on **Install sugested Plugin**

**installation of sonarqube**

installation of docker

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/50bb3fa6-e5fc-4768-8003-284f7eef0f5e)

command to access all docker permissions

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/813b4e0c-b8b7-4a4d-8f84-91db780dadad)

Command to set up sonarqube

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/dc5e970e-986b-4862-83d2-12f0a3ac1475)

-d : Detached mode (it will run the logs in background)

-p : mention te port range

eg: 9000:9001 (9000 is a host port ; 9001 is  container port)

lts: latest versuion of sonarqube image



























