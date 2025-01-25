<h1>Effortless-Website-Hosting-With-AWS</h1>

Launching a website using AWS EC2 involves several steps, from creating an EC2 instance to setting up a web server and connecting it to a domain. Here’s a step-by-step guide
Sign up for an AWS account and log in to the AWS Management Console.

<h2> Step-1</h2>

When configuring an AWS VPC (Virtual Private Cloud), there are a few key steps to follow.

Create a VPC:

Open the VPC dashboard in the AWS Management Console.
Select Create VPC and provide a name, CIDR block (e.g., 10.0.0.0/20), and select the default settings for the other options, unless you need custom configurations.
A VPC provides a logically isolated network environment in the AWS cloud.
It enables you to define and control your network's IP address range, subnets, and routing.

![ans](https://github.com/user-attachments/assets/e6af9134-cc67-4d87-a25f-5013541125e9)

<h2> Step-2</h2>
Subnets:

You need at least one public subnet and one private subnet.
For each subnet, define:
Public subnets: Resources (e.g., EC2 instances) that need to be accessible from the internet.
Private subnets: Resources (e.g., databases) that shouldn't be accessible directly from the internet.
The CIDR block (e.g., 10.0.1.0/24 for public and 10.0.2.0/24 for private).
The Availability Zone (AZ).

![ans-2](https://github.com/user-attachments/assets/47321513-b381-4383-b33c-21453eccc96d)

<h2> Step-3</h2>
Internet Gateway (IGW):

For public subnets to access the internet, you'll need to create an Internet Gateway and attach it to your VPC.
Update the route table to route internet-bound traffic (0.0.0.0/0) to the Internet Gateway.

![ans-3](https://github.com/user-attachments/assets/ed15350a-93c9-4ffe-81c9-ddda06720819)

<h2> Step-4</h2>
Route Tables:

AWS creates a default route table when you create a VPC.
Add custom routes if necessary, especially for public internet access (via an Internet Gateway).
![ans-4](https://github.com/user-attachments/assets/08685588-8328-4922-b715-8fc595f329f2)

<h2> Step-5</h2>

Launch an EC2 Instance
Navigate to EC2 Dashboard:

Search for "EC2" in the AWS Console and open it.
Create an Instance:

Click Launch Instances.
Choose an Amazon Machine Image (AMI):
Select an appropriate Linux-based AMI like Amazon Linux 2, Ubuntu, or another OS.
Select an instance type (e.g., t2.micro for free-tier eligibility).
Configure instance details:
Use the default VPC and subnet or customize as needed.
Enable public IP for the instance.
Add storage:
Stick with the default or increase the size if necessary.
Add tags (optional):
Add a key-value tag like Name: MyWebsite.
Configure the security group:
Open ports such as:
Port 22 for SSH.
Port 80 for HTTP (for web traffic).
Port 443 for HTTPS (optional for SSL/TLS).
Review and launch the instance.
Download the Key Pair:

When prompted, create or use an existing key pair and download the .pem file. This is needed for SSH access.

![ans-5](https://github.com/user-attachments/assets/2df60ba4-b312-4cbe-9ce8-de74f5478037)
![ans-6](https://github.com/user-attachments/assets/f868f792-be1c-4133-93ba-301b50be03c5)

<h2> Step-6</h2>
Copy the public instance ID and paste it in kitty terminal.
KiTTY and PuTTY are both popular terminal emulators used to establish SSH (Secure Shell) connections to remote servers, typically in a Linux environment. They are widely used in the IT and development communities for managing remote servers. Here's why they're so commonly used:
SSH and Remote Server Management
Secure Connections.
Cross-Platform Compatibility.
Simple, Lightweight Interface.

![ans-7](https://github.com/user-attachments/assets/7a2bf9ea-36cd-4a1c-9433-63fc1661bf39)


<h2> Step-7</h2>
I'm in the process of launching an online bakery store, where customers will be able to browse and order a wide variety of freshly baked goods, all from the convenience of their homes. This e-commerce site will offer everything from artisan breads to decadent cakes and pastries, making it easier than ever to satisfy sweet cravings and enjoy homemade treats.
which i took it from the online templates.

![ans-9](https://github.com/user-attachments/assets/30e6726f-7d54-4e11-bb12-98f553c32684)


<h2> Step-8</h2>
These are the list of commands which are used to launch my website successfully.

![ans-8](https://github.com/user-attachments/assets/5f35e75f-6479-4b8d-94d8-7e6352e76f1e)

<h2> Step-9</h2>
After the successful launch of the bakery e-commerce site, customers can now easily explore and order a delectable range of freshly baked goods from the comfort of their homes.


https://github.com/user-attachments/assets/7c93dd1d-7bd9-44b6-8aff-a6c0489bb12c








