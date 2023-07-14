# project-documentation

<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/6wj0hh6.jpg" alt="Project logo"></a>
</p>

<h3 align="center">E-commerce Online Shopping</h3>



---

<p align="center"> The E-commerce Online Shopping Project is a web application developed using React JS, Spring Boot, and MySQL. It aims to provide a user-friendly and efficient platform for online shopping. The front-end is built with React JS, ensuring a responsive and interactive user interface. The back-end is powered by Spring Boot, which handles the business logic, data processing, and API integrations. The MySQL database stores product information, user details, and order data, ensuring secure and reliable data storage.
    <br> 
</p>

## 📝 Table of Contents
- [About](#about)
- [Getting Started](#getting_started)
- [Modules](#modules)
- [Deployment](#deployment)
- [Usage](#usage)
- [Built Using](#built_using)
- [Contributing](../CONTRIBUTING.md)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)

## 🧐 About <a name = "about"></a>
In this project, all the main functionalities have been which should be present in any Ecommerce Project or Online Shopping Project. 

When a user visits our application for the first time, he will be able to see all the Products on the Home Page by default, he can also search the products based on the product categories which was added by the Administrator. After that User can log in and add the products to the Cart, and he can add multiple products to Cart with his required quantity, User can also delete the product from the Cart at any time.  

After this, the User can Order the products which are present in his Cart. During the Order placing, the User will be redirected to the Dummy Payment Page for the Order Payment. After the payment, all the products which were present in the Cart will be Ordered and he will get Order Id for the reference, And now he can also see his Orders, Delivery Person Details, and Delivery Status.

After the Customer Orders, Admin can all the Orders made by All the Customers. And now,  Admin can assign a Delivery Person for the Order by using the Customer Order Id. Now, After Assigning the Delivery Person, that particular Customer will be able to see the assigned Delivery Person who will deliver his Orders. And this Delivery Person will update the customer's Order Delivery Status like at what date and time the order is expected to deliver.

## 🏁 Getting Started <a name = "getting_started"></a>
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See [deployment](#deployment) for notes on how to deploy the project on a live system.

### Prerequisites
What things you need to install the software and how to install them.

- JAVA
- STS or ECLIPSE IDE
- MYSQL
- NODE.JS
- VS CODE EDITOR


### Installing
```bash
JAVA
```
- Visit the Oracle Java SE Development Kit (JDK) download page: https://www.oracle.com/java/technologies/javase-jdk11-downloads.html

- Accept the license agreement and choose the appropriate JDK version for your operating system. Click on the download link to start the download.

- Once the download is complete, run the installer executable (.exe file on Windows, .dmg file on macOS, or .tar.gz file on Linux) and follow the on-screen instructions.

- During the installation process, you may be asked to specify the installation directory. Choose an appropriate location on your system and proceed with the installation.

- After the installation is complete, open a command prompt (Windows) or terminal (macOS/Linux) to verify that Java is installed correctly. Run the following command to check the Java version:
        ```
        java -version
        ```

   You should see the installed Java version and other details if the installation was successful.

   Set up the JAVA_HOME environment variable. This variable points to the Java installation directory and is required by many Java-based tools and frameworks. The exact steps for setting     the environment variable depend on your operating system:
 
1. Windows:

- Right-click on "My Computer" or "This PC" and select "Properties".
- Click on "Advanced system settings" or "Advanced" tab.
- Click on "Environment Variables".
- Under "System variables" or "System Variables" section, click on "New".
- Enter JAVA_HOME as the variable name.
- Enter the path to your Java installation directory (e.g., C:\Program Files\Java\jdk1.8.0_221) as the variable value.
- Click "OK" to save the changes.
  
2. macOS/Linux:

- Open a terminal and run the following command to open the environment variable configuration file: ```
        nano ~/.bash_profile
        ```
- Add the following line at the end of the file: ```
        export JAVA_HOME=/path/to/java/installation
        ``` Replace /path/to/java/installation with the actual path to your Java installation directory
        
- Press Ctrl + X, then Y, and Enter to save the changes and exit nano.

```bash
STS
```
- Visit the Spring Tool Suite download page: https://spring.io/tools

- Scroll down to the "Latest Release" section and click on the download link for your operating system (Windows, macOS, or Linux).

- Once the download is complete, run the installer executable (.exe file on Windows, .dmg file on macOS, or .tar.gz file on Linux) and follow the on-screen instructions.

- During the installation process, you may be asked to specify the installation directory. Choose an appropriate location on your system and proceed with the installation.

- After the installation is complete, launch Spring Tool Suite.

- On the initial startup, you may be prompted to select a workspace directory. Choose a directory where you want to store your projects and click "Launch" to proceed.

- Once Spring Tool Suite is open, you can start creating or importing projects. To create a new project, follow these steps:
  
      - Click on "File" in the menu bar and select "New" -> "Spring Starter Project".
      - Enter a project name and choose the desired settings (e.g., Java version, packaging, dependencies).
      - Click "Next" and configure additional project settings if necessary (e.g., project location, build system).
      - Click "Finish" to create the project.
- To import an existing project into Spring Tool Suite, follow these steps:
  
      - Click on "File" in the menu bar and select "Import".
      - Expand the "General" category and select "Existing Projects into Workspace".
      - Click "Next" and browse to the root directory of your existing project.
      - Select the project(s) you want to import and click "Finish".

```bash
MYSQL
```
- Visit the MySQL Community Downloads page: https://dev.mysql.com/downloads/mysql/
- Scroll down to the "MySQL Community Server" section and click on the "Download" button for your operating system (Windows, macOS, or Linux).
- On the next page, you will see a list of available versions. Choose the appropriate version for your operating system and click the "Download" button.
- Once the download is complete, run the installer executable (.exe file on Windows, .dmg file on macOS, or .tar.gz file on Linux) and follow the on-screen instructions.
- During the installation process, you may be prompted to choose an installation type. Select the "Developer Default" or "Server Only" option, which includes the MySQL Server and other necessary components for development.
- Proceed with the installation, and you may be asked to set a root password for the MySQL Server. Choose a strong password and remember it as you will need it to access the database.
- Complete the installation process, and make sure to check the option to start the MySQL Server automatically.
- After the installation is complete, you can verify if the MySQL Server is running by opening a command prompt (Windows) or terminal (macOS/Linux) and running the following command: ```
      mysqladmin version
        ```
  If the server is running, you should see information about the MySQL version and server status.

- To interact with the MySQL Server, you can use the MySQL Command-Line Client or a graphical user interface (GUI) tool like MySQL Workbench.
MySQL Command-Line Client:

       - Open a command prompt (Windows) or terminal (macOS/Linux).
       - Run the following command to start the MySQL Command-Line Client and enter the root password when prompted: mysql -u root -p

MySQL Workbench (optional):

- Download and install MySQL Workbench from the MySQL website: https://www.mysql.com/products/workbench/
Launch MySQL Workbench.
- Click on the "+" icon in the "MySQL Connections" section to create a new connection.
- Enter a connection name and set the connection parameters (hostname, port, username, password) to match your MySQL Server configuration.
- Click "Test Connection" to verify the connection, and then click "OK" to save the connection.
- You can now use MySQL Workbench to manage your databases, execute queries, and perform other database-related tasks.

```
NODE.JS
```

- Visit the official Node.js website: https://nodejs.org
- On the homepage, you will see two download options: LTS (Long-Term Support) and Current. For most users, it is recommended to download the LTS version as it provides stability and long-term support. Click the "LTS" button to download the LTS version.
- Once the download is complete, run the installer executable (.msi file on Windows, .pkg file on macOS, or .tar.gz file on Linux) and follow the on-screen instructions.
- During the installation process, you may be prompted to choose the installation directory. You can keep the default directory or choose a different location as per your preference.
- Proceed with the installation, and you may be asked to accept the license agreement and select additional components. Generally, the default options are sufficient for most users, so you can continue with the default selections.
- Complete the installation process, and make sure to check the option to include Node.js in the system's PATH environment variable. This allows you to run Node.js and npm (Node Package Manager) commands from any directory in the command prompt or terminal.
- To verify if Node.js and npm are installed correctly, open a command prompt (Windows) or terminal (macOS/Linux) and run the following commands:```node -v
npm -v```

```
VS CODE EDITOR
```

- Visit the official Visual Studio Code website: https://code.visualstudio.com/

- On the homepage, you will see a "Download for [Your Operating System]" button. Click on it to start the download.

- Once the download is complete, run the installer executable (.exe file on Windows, .dmg file on macOS, or .deb/.rpm file on Linux) and follow the on-screen instructions.

- During the installation process, you may be prompted to choose the installation directory and select additional components. You can keep the default settings or choose a different location as per your preference.

- Complete the installation process, and Visual Studio Code will launch automatically after the installation is complete.

- When you first launch Visual Studio Code, you will see a welcome screen. You can choose to customize your settings or skip the customization and go straight to the editor.

- Visual Studio Code is now ready to use as a code editor. You can start by opening a folder or creating a new file.

##  Modules <a name = "modules"></a>

User Module:

The project contains 3 Module:

1) Admin

2) Customer

3) Delivery Person

Functional Modules:

1) User Authentication Module
2) Product Module
3) Product Category Module
4) Cart Module
5) Order Module
6) Delivery Module
7) Payment Module

User Role-Wise Functionalities:

```
CUSTOMER ROLE 
```

- Register & Login User :
  Register & Login of User is Role Based. During the Registration & Login, we have to select the Role like Admin, Customer, or Delivery Person.

<div class="separator" style="clear: both; text-align: left;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp;<a href="https://blogger.googleusercontent.com/img/a/AVvXsEjOglqiGoDrYkz1Zp9pp9dPq0dGBA1l1w0FdgPhHaDnkvCjDiGkwlg5zyS4pegt15eLUbLR1zIuDL14jwkJddka-a73w7hBoxHgADyUQlEogz8O28WqONqkfCr6D0RZl_MlqbCY7nPYWvX7l6QQHHEAUEOEgeg9GhgsfPKUVQXvr56gAQBOXnZ7BQNlIg" style="margin-left: 1em; margin-right: 1em;"><img alt="" data-original-height="901" data-original-width="389" height="320" src="https://blogger.googleusercontent.com/img/a/AVvXsEjOglqiGoDrYkz1Zp9pp9dPq0dGBA1l1w0FdgPhHaDnkvCjDiGkwlg5zyS4pegt15eLUbLR1zIuDL14jwkJddka-a73w7hBoxHgADyUQlEogz8O28WqONqkfCr6D0RZl_MlqbCY7nPYWvX7l6QQHHEAUEOEgeg9GhgsfPKUVQXvr56gAQBOXnZ7BQNlIg=w139-h320" width="139"></a>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;<a href="https://blogger.googleusercontent.com/img/a/AVvXsEgkxv80seYNj9LpQsrAGbqOj6BcPoDvYzvdeK9BNAYo9ryeuLEetae6nuAphDEW4mhWJUzNAccF4Rf7OEJFQjjylalc-TKhAC_v5oFI-aD3tHE7s-F75k-BQ_T1w50X4yi2WOInCRBlfsG8SX8uejc1E5SD25pqC56Q14jMvrWpQARNfza_nCjkfQin4g" style="margin-left: 1em; margin-right: 1em; text-align: center;"><img alt="" data-original-height="376" data-original-width="383" height="240" src="https://blogger.googleusercontent.com/img/a/AVvXsEgkxv80seYNj9LpQsrAGbqOj6BcPoDvYzvdeK9BNAYo9ryeuLEetae6nuAphDEW4mhWJUzNAccF4Rf7OEJFQjjylalc-TKhAC_v5oFI-aD3tHE7s-F75k-BQ_T1w50X4yi2WOInCRBlfsG8SX8uejc1E5SD25pqC56Q14jMvrWpQARNfza_nCjkfQin4g" width="244"></a></div>
<hr>

- Customers can view all the Products on the Home Page :-


<p align="center">
  <a href="" rel="noopener">
 <img width=621px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEjoF_c9TnZfcfR1idlqlcJORD8rkb7Bf3ulE9i_Hi5nCe9F48Ni8oiG_ka354SFfxjJqdO5RyESxlcU2OgdbtnpA96-KqkQL-h8qShVRc0yqWjURwkmwDdeNqfmknhSc8NdICT1FxJ2JSwbJFPHTWkdbqcIRHbPQv_XZeLDwQtrTaPX8hdcbHxwUWaN1A" alt="Project logo"></a>
</p>
<hr>

- Customers can Open a Product to View it in Detail.

<p align="center">
  <a href="" rel="noopener">
 <img width=676px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEh773WsEHT8RX321FlSn5ipO9tPD0z_KaN0mqWUvP6G_fuQ8TpbvRUdL72TYA421FYmK5DZZK54QLnZARzH-RxnXnnpG-kqRoOYeSWV9oFK6xPGEbMEq9-27a9ZWhbsijdO9BWcvazUsRnsPP5hyIjH658Yvo1CFKIviK3loxGty7eEbeXQRnshygVFog" alt="Project logo"></a>
</p>
In the above image, we can see, Customer will be able to see the Product in detail and below that, he can also see Related Products.
<hr>

- Customer's Cart :-

 In the above picture, we can see when we open a Product, we get the option to  Add Product Quantity to the Cart.
After adding all the required Products, Now, Customer can see his Cart as shown in the below picture.
<p align="center">
  <a href="" rel="noopener">
 <img width=731px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEj5R1a2H7__r4hlCCF0VYmF6Jd1rsqDtp6ge4dmDSPzKMN8qa6VD3mSWil81LdyVqNO-E9QYff4__Iv-DFiC_PwyjmVSHUEhjPwQTaTSuSvk95z2gR8I4idhXntqAar-Q9rNQI_7m661AflNSl7bztZqoJ8HK48S2fB8aSuxVF5nwJKki1YO3cf7Kr6_w" alt="Project logo"></a>
</p>

  Customers can also delete the Product from the Cart by clicking on the delete button in front of the Product.
Below, the Customer will be able to see the total amount to Pay for the Order.
<hr>

- Payment for the Order :-
  
  In the above pic, below the Total Price for the Order, customers will get the Checkout button, so when the customer will click on it, It will be redirected to the payment page as shown below.

<p align="center">
  <a href="" rel="noopener">
 <img width=297px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEhVpj9hcx-faCQTUxwfSnoSTmxHPPsYLQ-6stOO3xb8yFGITtDUtjhKSpe2_8-BT1TftO3rcg73AV2VzgUDdxiz_f3lEfyO3yrLTW2rW4Dg9dKIfr92mZMXaGPLhnxtLeBpLHDaC_V9oBByEp4s3R7ltZexD7hqUJu9DsvxLci7-pglo75EzEBzSBWftw" alt="Project logo"></a>
</p>

  So after filling in all the details, when the customer will click the Pay button, an Order will be placed for the Customer.
<hr>

```
ADMIN ROLE
```
- View All Customer Orders

  Admin can see all the Customer Orders after the login as shown in the below picture.
<p align="center">
  <a href="" rel="noopener">
 <img width=734px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEh-wkDxXRUDy2V16QDkEtVVT8EuCpkVVmxAOpw8_sGYKo8lBzt7TEJCBLBt2Thm603ilwxV2mQ6SjcfQM5hrMHtwUikkGRcfeBcMQjBuENZNKbH8Z0dE1bwg9Oj_wuFdJ5JplH5MtY-m_nZdc_27D6gLFExDiYJk0LeCKmcLGaYgHDa_9Jndeby1SDnPg" alt="Project logo"></a>
</p>

  Admin can see for the Order, delivery Status is Pending. So from here, the admin can assign the Delivery Person for the Customer Order.
<hr>

- Assign a Delivery Person for Customer Orders

  As seen in the above picture, For all the Customer Orders, the Delivery Status is Pending. So now, Admin can assign a Delivery Person for the Customer Orders by using the Unique Order Id.
<p align="center">
  <a href="" rel="noopener">
 <img width=734px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEifN6gL6SYHP9ROuYAOBVuG76s7pd0qLnS4OJjxSBKN95bCtksEWxSLdonWxlf9r61TJs5wlBb8sI3wfxEjIWIQ_nDBb96PzKJhaGKs1Kx4rW5yom5ndpMdZ2o4tJm0Yf63nz3RVL7HaQqpaMVHEWm7Al6QMhrDFDUXZqlk7gw4CcftFUy3Z1eiLWgD8A" alt="Project logo"></a>
</p>

<hr>

- Add Category

  Admin can add the Product Categories like laptops, Mobile, Shoes, etc.
<p align="center">
  <a href="" rel="noopener">
 <img width=399px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEhPTf_GmUaRSp27uk9IYDlKHO3JLsu6dXceMpeGM08lzU31hY0JwrJg6lGoQ-npoGaXMUav2fQHZYrMHBVrEbn_jFU1-PKJwIYHiL0vgJ1IAtQyLCD2dibg07hmRuRm80Bk8fPNQ0EiMO0f7F9gPdH6_w10dGES-wo3IPvzeDVC6U85Ag84VWr09ByuAQ" alt="Project logo"></a>
</p>
<hr>

- Add Products
  
  Admin can add the Product.

<p align="center">
  <a href="" rel="noopener">
 <img width=203px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEh5_1PWAusFhvX_1c_Sk77b0D2GKce-LTMAK43blSh9R4-z73L46OD_osGbVjIlHtpLBeGM9O7BxWfSjMYzeqxcj3x-GMbw0SSs2BiPlCc_DiNWmm1bFR2JFEqqHGOcMwslp5To4EcshfcQ5jLOBmhtJP6Kc6fQFWVRdP3GnDA8ZRUNAN5pu_RgxnBONw" alt="Project logo"></a>
</p>
<hr>

```
DELIVERY PERSON ROLE
```
- View My Deliveries

  Delivery Person can see all the Orders which are assigned to him by the Admin as shown below.
<p align="center">
  <a href="" rel="noopener">
 <img width=735px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEiyZxYH7GSJqdxDXARmU1s7ri7PMRy9aYdWz8K-fI-6Rihqtje_Ob51r4W3XWKdGEeXwdydCf_iynbdIdy3Z-78AcUTL4TYirDXF__Tt84ytgOqpt1pinO3TJAOIWhkQZ80oHmWPE1iHcdzoJagNK9ljEfApoZggie2ykb0jA9abodhNQs3pGKwhBe32Q" alt="Project logo"></a>
</p>
<hr>

- Update the Delivery Status for the Order.

  In the above picture, the Delivery Person can see the Delivery Status, and Time as Pending. So from here, Delivery Person can update the Delivery Status and Time as per his expectation    as shown below.
<p align="center">
  <a href="" rel="noopener">
 <img width=747px height=348px src="https://blogger.googleusercontent.com/img/a/AVvXsEjoAPIy9hB-V2RQ1pP2uLVy8unywiMSc_AC0EETB64hlbCzTe8B6d72e3TUkfeHkyuDReHmyeB-j7WofGxRG70n0Zt46xOG-ASRN9-ZdklKvf75Q0c_O2daMx7bvRxRc63NQQlVCxo6erNaQi9F1jkjAKpr16uj1_Qap-OenNxbYx2oHCC-l1He86B9sw" alt="Project logo"></a>
</p>



  
  

## 🔧 Running the tests <a name = "tests"></a>
Explain how to run the automated tests for this system.

### Break down into end to end tests
Explain what these tests test and why

```
Give an example
```

### And coding style tests
Explain what these tests test and why

```
Give an example
```

## 🎈 Usage <a name="usage"></a>
Add notes about how to use the system.

## 🚀 Deployment <a name = "deployment"></a>
Add additional notes about how to deploy this on a live system.

## ⛏️ Built Using <a name = "built_using"></a>
- [MongoDB](https://www.mongodb.com/) - Database
- [Express](https://expressjs.com/) - Server Framework
- [VueJs](https://vuejs.org/) - Web Framework
- [NodeJs](https://nodejs.org/en/) - Server Environment

## ✍️ Authors <a name = "authors"></a>
- [@kylelobo](https://github.com/kylelobo) - Idea & Initial work

See also the list of [contributors](https://github.com/kylelobo/The-Documentation-Compendium/contributors) who participated in this project.

## 🎉 Acknowledgements <a name = "acknowledgement"></a>
- Hat tip to anyone whose code was used
- Inspiration
- References
