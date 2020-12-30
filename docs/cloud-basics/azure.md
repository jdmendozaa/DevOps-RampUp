# Cloud Basics - Azure

This challenge aims to set up the cloud environment on which the project will run.

1. **Create a diagram** that reflects the design of the infrastructure you will create in the next steps.  

2. **Create the networking infrastructure** on which your application will live.  

    * Setup a custom VNet.
    * Create the subnets.  
    * Configure security for your subnets (Subnet Security Groups).

    **Note:** Because of constraints with the training Azure account, you may be required to use an existing networking infrastructure. In that case, explain your tutor each the elements involved and how they relate to each other. Make sure you don’t skip this step; networking is an essential part of what we do!

3. **Create the compute infrastructure to support the application.** Is recommended to separate front-end and back-end.

    * Create Virtual Machines and install the applications
    * Capture Images that contains the application and configurations.
    * Create an Scale Set
    * Create a LoadBalancer or and Application Gateway (Read about both and understand the differences, explain why you decided to use the one you deploy)
    * Create LoadBalancer between Front-End and Back-End
    * The expected behavior is: If you destroy one instance (or the application fails), another must be created automatically with the application running again.  

    **Note:** If the application has any external service, like a database or cache system, you can either use a managed service by Azure (as SQL databases, or Azure Database for MySQL, etc.) Or install and manage the service by yourself. In a real production environment, we usually use managed services, but it's a great learning exercise to create all things by yourself. So, if you think you have time, we recommend following the second option, you’ll learn tons of new stuff!

4. **Secure your infrastructure.** Don’t forget to always follow the principle of least privilege.

    * Create security groups for all your resources (Virtual Machines, DBs, etc.). Decide carefully which ports you open and who can access them.

    * Create Service Principals to assign permissions to the applications.

5. **Estimate of the total cost of the infrastructure you created** You can use the [Azure Pricing Calculator](https://azure.microsoft.com/en-us/pricing/calculator) or you can create an Excel sheet.
 

## Recommended readings
