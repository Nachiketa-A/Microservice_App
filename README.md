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

eksctl create cluster --name=my-eks92 \
                      --region=us-east-1 \
                      --zones=us-east-1a,us-east-1b \
                      --version=1.30 \
                      --without-nodegroup



![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/ccb0417d-fda9-43fd-a89d-c808ec2fdee0)



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

Credentials of jenkins

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/ff770f0f-26b0-4092-a309-ebfed77323da)


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

command to check container is created or not

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/a68323ee-f4e7-4630-9064-11a3cb08b7bc)

To access sonarqube copy te public ip address and open it on port 9000

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/2733db19-184d-45f1-84c2-fc6da25cd2d7)

sonarqube credentials

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/1504417b-6bec-4e60-a323-b902809979ab)


After execution of EKS Cluster command

To setup worker node

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/86429c03-ab6a-4bd6-a187-7b9cb9848f29)


![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/0370218a-6a6d-4bbb-9615-9af8a116f2a9)


Meanwhhile we will manage jenkins

**Steps**

Go to **manage Jenkins**

click **Plugins**

click on **Available Plugins**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/3f4e1429-937c-4781-b105-195126bb875a)

For docker Plugins

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/0cd60108-c6ec-4fcb-93ac-f91aea392a2d)

For kubernetes plugins

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/238cdf38-0b7e-44f9-a78b-8d6b6bcf6820)

Click **Install**

For conifuration of Jenkins

Go to **Manage Jenkins**

Click on **Tools**

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/ac8543a0-43ff-46d0-9cb8-ed709b976c69)

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/89de3cc7-9b21-4bda-949d-05a3adaed0c4)

Click on **Apply**

To configure Sonarqube server

Go to Sonarqube -> Administartion -> security -> users -> token

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/a79251d0-f192-402d-81a3-014e0fcde940)

Copy token 

Go to Jenkins -> manage jenkins -> credentials-> system -> global credentials -> add credentials

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/c5730c06-d3f1-4f0d-b591-53c83e519e71)

To add sonarqube server to the jenkins

MAnage jenkins -> system

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/1e992fd4-0079-4102-8f2e-27273acd4926)


To check the status of worker node

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/92480573-56e2-403a-a5f9-01787fc738d9)

Open the EKS in AWS -

Click on **Cluster name** -> security -> inbound rules

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/e1a5ace8-fc08-4ed0-8bc1-7db65261d70c)

To check namespace

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/6e994428-42e2-4232-9eb6-088447054c32)

To create new namespace

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/51af6b0d-bee2-46ee-b19b-c2890d668d47)

**Creatin Service Account**

Firstly create one yaml file usin command 

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/017edfa5-9076-4246-949e-01701d24f34d)

To execute te service account code

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/aed79d1a-903f-4159-9417-112ca8cbbcb7)










 

















































