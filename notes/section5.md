# Section 5
## Budget Setup
We can debug our bills using the AWS billing section, you can find the different services that you are using and the carge also with the region
![Alt text](images/budget.png)
![Alt text](images/freetier.png)


To void cost the best practice is to create a budget, you can choose your budget type and use a template


![Alt text](images/budgettype.png)

-----
# EC2 Section
![Alt text](images/EC2intro.png)
![Alt text](images/EC2config.png)


You should select the instance that fit best with your application depending of the demand.

![Alt text](images/EC2types.png)

## Create and EC2 instance with EC2 User Data to have a Website Hands On

![Alt text](images/EC2instance.png)

* Define the name and tag
* Choose a OS system (linux, ubuntu, windows)
* Select Amazon Machine Image (default is free)
* Select Instance type (t2.micro) is free for a month
* Create a Key Pair (RSA and .pem)
* Network 
    * Allow SSH traffic from anywhere
    * Allow HTTP traffic from the internet
* User data: Here we add a script with a command that will execute in the first launch, only once in the hole life cycle of the instance. It is going to update some things and install the **HTTPD** web server on the machine and write an html file to see in the website
![Alt text](images/userdatainstance.png)

**NOTE** Without a server i'm able to create one or a hundred of instances in just a couple of seconds.  


* If you stop and instant and then rerun, aws is going to change de Public IP Address

![Alt text](images/publicaddressEC2.png)

---
## EC2 Instance Types
![Alt text](images/instancetypes.png)

![Alt text](images/instance-generalpurpose.png)