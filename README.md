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
- SPRING TOOL SUITE (STS)
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

<hr>

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

<hr>

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

<hr>

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

<hr>

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
<hr>

## 🎈 Usage <a name="usage"></a>

```
BACKEND PART  :- 
```
  
<h3> STEP 1 :- Import the backend part of project to sts</h3>

- Launch Spring Tool Suite.
- In the main menu, click on "File" and select "Import" to open the import wizard.
- In the import wizard, expand the "Maven" category and select "Existing Maven Projects". Click "Next".
- On the next screen, click the "Browse" button next to the "Root Directory" field and navigate to the location of your Maven project.
- Select the project folder and click "Finish". STS will start scanning the project directory for the Maven project structure and dependencies.
- Once the project is detected, you will see it listed in the import wizard. Make sure the project checkbox is selected, and click "Finish".
- STS will import the Maven project and start building it. This process may take some time.

<h3>STEP 2 :- Open application.properties file </h3>

- Write your root password after equals on the line : ```spring.datasource.password = ```
- Create a images folder in the system .
- Give the correct path of the images folder under : ```disk.uplaod.basepath = ```
  
<h3>STEP 3 :- Run Mavin Build</h3>

- Click on the project .
- Select run as maven build
- In the goals write : clean install
- Check the skip test box 
- Click on apply 
- The console will open and it will run the tests and after completion it will show  'BHUILD SUCCESS'

<h4>STEP 3 :- Run the Project </h3>

- Click on the Project 
- Select run as Spring Boot App

<hr>

```
FRONT-END PART  :-
```

<h3> STEP 1 :- Import the front-end part of project to vs code </h3>

- Launch Visual Studio Code.
- Open the folder where your existing React project is located by either selecting "Open Folder" from the "File" menu or using the keyboard shortcut Ctrl+K Ctrl+O (Windows/Linux) or Cmd+K - Cmd+O (macOS).
- Once the folder is open in VS Code, you should see the project files in the Explorer sidebar.
- Open an integrated terminal in VS Code by selecting "View" from the menu, then "Terminal" or using the keyboard shortcut Ctrl+ backtick (`). This will open a new terminal pane at the bottom of the editor.
- In the terminal, navigate to the root directory of your React project.
- Once you're in the root directory of your React project and have Node.js and npm installed, run the following command to install the project dependencies listed in the package.json file:```npm install```

<h3> STEP 2 :- Run the Project  </h3>

- After the installation is complete, run the following command to start the React development server:```npm start```
- Open a web browser and navigate to the URL provided in the terminal (e.g., http://localhost:3000). You should now see your React application running in the browser.
- 
```
NOTE:- Initially the admin need to add products and category as shown in modules section of the readme . 
```


## 🚀 Deployment <a name = "deployment"></a>

<h2> STEP 1 :- Set up the Live System:</h2>

- Obtain a server or hosting provider where you can deploy your project.
- Ensure the server meets the system requirements for running React JS, Spring Boot, and MySQL.
- Install the necessary software dependencies on the server, including Node.js, Java (for Spring Boot), and MySQL.

<h2>STEP 2 :- Build the React JS Frontend:</h2>

- In the root directory of your React project, run the following command to build the optimized production-ready version of your frontend:```npm run build```
- This will create a build folder containing the compiled and minified assets of your React project.

<h2> STEP 3 :-Configure and Serve the Frontend (React JS):</h2>

- Set up a web server (e.g., Apache or Nginx) on the server to serve the static files of your React JS frontend.
- Configure the web server to point to the build folder generated in Step 2.
- Set up appropriate routing rules and configurations to handle frontend routes.

<h2>STEP 4 :-Test and Verify the Deployment:</h2>

- Access the live system URL in a web browser to ensure that the React JS frontend and Spring Boot backend are functioning correctly.
- Perform end-to-end testing on the live system to validate the complete functionality of the E-commerce Online Shopping Project.
- Monitor the logs and error reports to identify and resolve any issues that may arise during the live deployment.

<h2>STEP 5 :-Set up Continuous Integration/Continuous Deployment (CI/CD) (Optional):</h2>

- Consider implementing CI/CD pipelines using tools like Jenkins, Travis CI, or GitLab CI/CD to automate the deployment process, allowing for continuous integration and deployment of updates to the live system.

## ⛏️ Built Using <a name = "built_using"></a>
- [MySQL](https://www.mysql.com/) - Database
- [Spring-Boot](https://spring.io/projects/spring-boot) - Server Framework
- [React.js](https://react.dev/) - Web Framework
- [NodeJs](https://nodejs.org/en/) - Server Environment

## ✍️ Authors <a name = "authors"></a>
- [@yashraj](https://github.com/Yashraj05) - Idea & Initial work


## 🎉 Acknowledgements <a name = "acknowledgement"></a>
 <h2>Inspiration :-</h2>
 
- Full-stack Development: Developing an E-commerce project with React JS, Spring Boot, and MySQL allows you to showcase your skills in both frontend and backend development. It offers an opportunity to work with modern JavaScript frameworks, build efficient APIs, and handle data persistence.
- React JS - Rich User Interface: React JS is a popular JavaScript library for building user interfaces. It offers a component-based architecture, allowing you to create reusable UI components, manage state efficiently, and provide a seamless and responsive user experience.
- Spring Boot - Powerful Backend Framework: Spring Boot is a robust Java framework that simplifies backend development. It provides features like dependency injection, easy configuration, and a wide range of libraries for building RESTful APIs, handling security, and integrating with databases.
- MySQL - Reliable Database Management: MySQL is a widely used open-source relational database management system. It offers stability, performance, and scalability, making it a suitable choice for handling product data, user information, and order management in an e-commerce application.
- E-commerce Demand: E-commerce is a rapidly growing industry with increasing demand. Developing an E-commerce Online Shopping Project allows you to explore real-world scenarios, such as product listing, searching, filtering, user authentication, shopping cart management, and order processing.
- Learning Opportunities: Building an E-commerce project using these technologies provides an excellent learning experience. You can gain expertise in frontend development with React JS, backend development with Spring Boot, API integration, database management with MySQL, and the overall development workflow.
- Portfolio and Career Growth: Completing an E-commerce project using React JS, Spring Boot, and MySQL adds a valuable project to your portfolio, showcasing your skills and capabilities as a full-stack developer. It can attract potential employers, clients, or collaborators and open doors to new career opportunities.
- Customizability and Scalability: By building your own E-commerce project, you have the freedom to customize and tailor it to specific business requirements. You can implement custom features, integrate payment gateways, optimize performance, and scale the application as the business grows.
  
<h2> References </h2> 

<h4>React JS:</h4>

- React documentation: https://reactjs.org/docs/
- React Router: For handling client-side routing within the React application. Documentation: https://reactrouter.com/
- React Bootstrap or Material-UI: UI component libraries for building responsive and visually appealing user interfaces. Documentation: https://react-bootstrap.github.io/ or https://mui.com/
  
<h4>Spring Boot:</h4>

- Spring Boot documentation: https://spring.io/projects/spring-boot
- Spring Data JPA: Simplifies database operations and provides repositories for interacting with MySQL. Documentation: https://spring.io/projects/spring-data-jpa
- Spring Security: For implementing authentication and authorization in your application. Documentation: https://spring.io/projects/spring-security

<h4>MySQL:</h4>

- MySQL documentation: https://dev.mysql.com/doc/
- Spring Data JPA: As mentioned above, it simplifies database interactions and provides convenient methods for querying and manipulating data in MySQL.
