
## What is this Application:- 

**Online Boutique** is a demo e-commerce application designed to showcase how different parts of a web-based store can be built using a cloud-first microservices architecture. Microservices mean that the application is divided into smaller, independently deployable services, each handling a specific part of the application's functionality.

The application consists of 11 separate services (or microservices), each written in different programming languages and responsible for different tasks:

1. **frontend** (Go): This is the main web server that shows the website to users. It doesn't need users to sign up or log in; it creates session IDs automatically.

2. **cartservice** (C#): Manages the shopping cart. It saves items in the cart using Redis, a type of database, and retrieves them when needed.

3. **productcatalogservice** (Go): Provides the product list from a JSON file, allows searching for products, and fetching details of individual products.

4. **currencyservice** (Node.js): Converts prices between different currencies using real exchange rates from the European Central Bank. This service handles the highest number of requests per second.

5. **paymentservice** (Node.js): Processes payments by taking credit card information (simulated) and returning a transaction ID.

6. **shippingservice** (Go): Estimates shipping costs based on the items in the shopping cart and provides shipping services (simulated).

7. **emailservice** (Python): Sends order confirmation emails to users (simulated).

8. **checkoutservice** (Go): Manages the checkout process. It collects the items in the cart, prepares the order, processes the payment, handles shipping, and sends the confirmation email.

9. **recommendationservice** (Python): Suggests other products to users based on what's in their shopping cart.

10. **adservice** (Java): Displays text advertisements based on certain keywords.

11. **loadgenerator** (Python/Locust): Simulates real user activity on the website by continuously sending requests to the frontend.

Each of these services is like a small, independent piece of the overall application. They work together to create the full shopping experience for users but can be developed, deployed, and scaled independently.


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






