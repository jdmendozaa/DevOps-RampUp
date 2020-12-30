# Cloud Basics - AWS

This challenge aims to set up the cloud environment on which the project will run.

1. **Create a diagram** that reflects the design of the infrastructure you will create in the next steps.  

2. **Create the networking infrastructure** on which your application will live.  

    * Setup a custom VPC.
    * Create the subnets.  
    * Setup route tables for all subnets.
    * Set up a connection to the internet (Internet Gateway and NAT).
    * Configure security for your subnets (Network ACLs).

    **Note:** Because of constraints with the training AWS account, you may be required to use an existing networking infrastructure. In that case, explain your tutor each the elements involved and how they relate to each other. Make sure you don’t skip this step; networking is an essential part of what we do!

3. **Create the ec2 infrastructure to support the application.** If the application has one backend and one fronted, you will need to create one for each.  

    * Create a load balancer.
    * Create a launch configuration or a launch template.
    * Create an auto-scaling group.
    * The expected behavior is: If you destroy one instance (or the application fails), another must be created automatically with the application running again.  

    **Note:** If the application has any external service, like a database or cache system, you can either use a managed service by AWS (as RDS for SQL databases, or Amazon DocumentDB for MongoDB, etc.) Or install and manage the service by yourself. In a real production environment, we usually use managed services, but it's a great learning exercise to create all things by yourself. So, if you think you have time, we recommend following the second option, you’ll learn tons of new stuff!

4. **Secure your infrastructure.** Don’t forget to always follow the principle of least privilege.

    * Create security groups for all your resources (Instances, database, etc.). Decide carefully which ports you open and who can access them.

    * Create IAM policies and roles to assign permissions to the applications.

5. **Create an Excel sheet with an estimate of the total cost**  of the infrastructure you created.