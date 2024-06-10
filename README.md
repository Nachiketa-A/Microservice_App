

**Create role**

To create role first create yaml file 

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/20ee883e-3264-4e89-8aa0-aeb94afc1791)

Execute te yanl file using command:

Kubectl apply-f rol.yml

after execution of this command role will be created

To assign the role to service account

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/d09885fb-e290-4c61-96f4-170da68feb5b)

To create a token for service account use below yaml file

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/2796401c-6fc7-494b-9ddc-17b67186ee80)


Pipeline creation

GGo to jenkins -> new item ->enter the name -> select pipeline-> click ok

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/d764b10a-5696-43b1-835d-0136fb4e6ded)

Groovy scripting

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/3897850b-b068-4233-90dc-76a1a21db56d)


For git url go to Pipeline syntax->select sample step as git:GIT -> copy git repo url and paste it there -> enerate pipeline script

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/e70a6c78-9d2d-4eee-a8b7-b82df23ac970)


Build Docker Image


command to create kubernetes token

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/b9c93e21-5f95-4ff8-a68f-9d416439ff13)


configuration for k8-token

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/e537b330-f461-432c-a4d8-10cbc88bb11a)

After running pipeline we need to check all the pods are running are not for that

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/ab974bed-bb26-4aff-b73e-e2c333c28794)

Here we can see all the pods are running

To check for services

![image](https://github.com/Nachiketa-A/Microservice_App/assets/157089767/93ebf063-f662-4815-8058-1f754aef184b)



a6c757886c0b04894a1d0cb050e41ce8-1761995302.us-east-1.elb.amazonaws.com 




















 

















































