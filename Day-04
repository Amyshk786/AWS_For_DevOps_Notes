
Day 4 - | Best VPC explanation| VPC explained in 30 mins
========================================================


Virtual Private Cloud (VPC) - 


Imagine you want to set up a private, secure, and isolated area in the cloud where you can run your applications and store your data. This is where a VPC comes into play.


A VPC is a virtual network that you create in the cloud. It allows you to have your own private section of the internet, just like having your own network within a larger network. Within this VPC, you can create and manage various resources, such as servers, databases, and storage.


Think of it as having your own little "internet" within the bigger internet. This virtual network is completely isolated from other users' networks, so your data and applications are secure and protected.


Just like a physical network, a VPC has its own set of rules and configurations. You can define the IP address range for your VPC and create smaller subnetworks within it called subnets. These subnets help you organize your resources and control how they communicate with each other.


To connect your VPC to the internet or other networks, you can set up gateways or routers. These act as entry and exit points for traffic going in and out of your VPC. You can control the flow of traffic and set up security measures to protect your resources from unauthorized access.


With a VPC, you have control over your network environment. You can define access rules, set up firewalls, and configure security groups to regulate who can access your resources and how they can communicate.
 




---------------------------------------------------------------------------------------------------------------------------------------------------------------------




VPC Components - 
==================


1) Virtual private clouds (VPC) - A VPC is a virtual network that closely resembles a traditional network that you'd operate in your own data center. After you create a VPC, you can add subnets.



2) Subnets - A subnet is a range of IP addresses in your VPC. A subnet must reside in a single Availability Zone. After you add subnets, you can deploy AWS resources in your VPC.



3) IP addressing - You can assign IP addresses, both IPv4 and IPv6, to your VPCs and subnets. You can also bring your public IPv4 and IPv6 GUA addresses to AWS and allocate them to resources in your VPC, such as EC2 instances, NAT gateways, and Network Load Balancers.



4) Network Access Control List (NACL) - A Network Access Control List is a Stateless Firewall that controls Inbound and Outbound traffic at the Subnet Level. It operates at the IP address level and can allow or deny traffic based on rules that you define. NACLs provide an additional layer of network security for your VPC.



5) Security Group - A security group acts as a virtual firewall for instances (EC2 instances or other resources) within a VPC. It controls inbound and outbound traffic at the instance level. Security groups allow you to define rules that permit or restrict traffic based on protocols, ports, and IP addresses.  



6) Routing - Use route tables to determine where network traffic from your subnet or gateway is directed.



7) Gateways and Endpoints - A gateway connects your VPC to another network. For example, use an internet gateway to connect your VPC to the internet. Use a VPC endpoint to connect to AWS services privately, without the use of an internet gateway or NAT device.



8) Peering connections - Use a VPC peering connection to route traffic between the resources in two VPCs.



9) Traffic Mirroring - Copy network traffic from network interfaces and send it to security and monitoring appliances for deep packet inspection.



10) Transit Gateways - Use a transit gateway, which acts as a central hub, to route traffic between your VPCs, VPN connections, and AWS Direct Connect connections.



11) VPC Flow Logs - A flow log captures information about the IP traffic going to and from network interfaces in your VPC.



12) VPN connections - Connect your VPCs to your on-premises networks using AWS Virtual Private Network (AWS VPN).




Resources For VPC with servers in private subnets and NAT - https://docs.aws.amazon.com/vpc/latest/userguide/vpc-example-private-subnets-nat.html





--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

CA



A Virtual Private Cloud (VPC) is a private, logically isolated network environment within a public cloud provider's infrastructure. It enables users to create virtualized networks, subnets, and other networking components, similar to an on-premises data center, but within the cloud provider's infrastructure.

In a VPC, users have control over network settings, such as IP address ranges, subnets, routing tables, and security groups. This level of control allows them to design and manage their network architecture in a secure and scalable manner.


Features of Virtual Private Cloud (VPC) - (VPISSRNN)

1. VPC

2. Peering Connection

3. Internet Gateway (IGW)

4. Subnet

5. Security Groups

6. Route Tables

7. Network Access Control Lists (NACL's)

8. Network Address Translation Gateway (NAT Gateway)



 --> Note - Internet gateway per request aayegi toh round table per request jyegi then NACL fir waha se Public Subnet and NAT per request jyegi toh public subnet se private subnet se connect hoga. 
 
 
 
 
 Things to remember: 

--> Each subnet exists within 1 availability zone.

--> Security groups are stateful, ACL’s are stateless

--> Transitive peering is not allowed, meaning you can't hop from one VPC to another, via another VPC. You must have direct access.

--> VPC’s can be peered within the same account and across AWS accounts 


 
 

The main benefits of using a Virtual Private Cloud include:

--> Isolation: VPC's offer logical isolation from other customers and the public internet, enhancing security and privacy.

--> Scalability: Users can easily scale their network resources up or down based on their requirements.

--> Security: Users have control over network access and security configurations, allowing them to implement robust security measures.

--> Cost-Efficiency: VPC's provide the benefits of cloud computing while offering a level of control and isolation similar to traditional data centers, helping organizations optimize costs.





--> Availability Zones (AZ's)  are  Physically isolated data centers. Data is flowing at the speed of light from A to B and B to A. And ek se dusre Datacenter ke beech ka max distance  100km hona chahiye due to latency issue q ki agar zyada dur rahega toh latency badegi

-->  A CIDR is basically a combination of IP Address and Subnet Masks that allows you to define a range of IP Addresses. CIDR stands for Classless Inter-Domain Routing.
For example, in the CIDR notation "192.168.1.0/24," the first 24 bits represent the network portion, leaving 8 bits for the host portion.
 {Uper k eg me phle 3 octet block ho jyege and last wala octet rahega host k pas.}
 
 
 
 
 Subnet
A subnet is a range of IP addresses in your VPC. You can launch AWS resources, such as EC2 instances,into a specific subnet. When you create a subnet, you specify the IPv4 CIDR block for the subnet, which is a subset of the VPC CIDR block. Each subnet must reside entirely within one Availability Zone and cannot span zones. By launching instances in separate Availability Zones, you can protect your applications from the failure of a single zone.



--> Subnet is a collection or Range of IP Addresses 

Subnets are of Three types  -
A)Public Subnet
B) Private Subnet
C) VPN only Subnet but ye use nhi hota hai organisation me and sirf interview perspective se yad rkhna h third wala.

-->  Public Subnet  ki connectivity Internet Gateway and Local dono se rehti hai 

-->  A private subnet is any subnet which is connected to NAT Gateway
Private Subnet ki connectivity local router tuk hi rehti hai 





Internet Gateway
An Internet Gateway is how your VPC accesses the internet. Internet gateway allows communication between resources such as EC2 and RDS instances in your VPC and the Internet. It is highly available, redundant, and horizontally scalable; that is, you do not need to attach more than one internet gateway to your VPC in order to support an increase in traffic.

If a VPC does not have an Internet Gateway, then the resources in the VPC cannot be accessed from the Internet. It allows resources within your VPC to access the internet, and vice versa.






NAT Gateway
You will often have resources in your VPC that will reside in private subnets that are not accessible from the internet. However, these resources will need to access the internet occasionally for patch update, software upgrade, and so on. A NAT device is used exactly for this purpose, allowing resources in private subnet to connect with either the internet or other AWS services securely. NAT devices support only IPv4 traffic.


-->  Functions Of NAT Gateway - 

A) Internal request jab aayegi toh usko private IP address se Public IP address pe translate kur ke aage bada dena.

B) Agar andar se request aa rahi hai toh uska response allow kurna chahiye but agar bahar se request aa rahi hai toh usko deny karega. 



AWS recommends a NAT gateway over a NAT instance as it is a managed service that requires little or no administration, is highly available, and highly scalable.

Things to remember:

1. Scale automatically up to 10Gbps
2. Automatically assigned a public IP
3. Security Groups cannot be associated with a NAT Gateway.





VPC Endpoints
A VPC endpoints is a secure way to communicate with other AWS services without using the internet, Direct Connect, VPN Connection, or a NAT device. This communication happens within the Amazon network internally so your traffic never goes out of Amazon network. At present, endpoints are supported only for Simple Storage Service (S3). These endpoints are virtual devices supporting IPv4-only traffic.

VPC endpoints support IPv4 traffic only.
Endpoints are supported within the same Region only.
Endpoints cannot transfer an endpoint from one VPC to another, or from one service to another.



--> How to Calculate CIDR range manually

2(³² minus 16 )



====================================================================================================================


   --> How to Deploy VPC - 
   

 Step 1 VPC create 

 Step 2 Create Subnet (1a public subnet)  (1b private subnet)

 Step 3 Create Route table (public rt)  (private rt)

 Step 4 internet gateway me ja k usko attach krne ka 

 Step 5 Subnet association take public and save in public

 Step 6 Take private and save in private

 Step 7 Add internet gateway to public 

 Step 8 Create Instance for public and private both
 Select public VPC and grp the. Enable security group common.

 Step 9 For private bas private select Krna h and disable
 

 Note -  NAT is required for connecting private &and NAT ko private me add krne ka 
 
 
========================================= For Clean Up =============================================================

•	Terminate instances
•	Release Elastic IP
•	Detach & Delete NAT Gateway
•	Detach & Delete Internet Gateway
•	Delete VPC






---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



VPC Peering - 
===================



Peering Connection
A VPC peering connection is a networking connection between two VPCs that enables routing using each VPC’s private IP addresses as if they were in the same network. This is the AWS recommended method for connecting VPCs.VPC peering connections can be created between your own VPCs or with a VPC in another AWS account. VPC peering also supports inter-region peering. Traffic using inter-region VPC Peering always stays on the global AWS backbone and never traverses the public internet, thereby reducing threat vectors, such as common exploits and DDoS attacks.




Create vpc 1 (Demo) 

Create vpc 2 (Project)

Create 1 public instance in workspace and 1 private instance in ubuntu for Demo VPC

Create 1 public instance in workspace and 1 private instance in ubuntu for Project VPC

Go to Peering connection and create a peering request and once the request is created then go to Actions and Accept the peering request.

Go to Route Table and Demo k route table me Project ke vpc ka CIDR dalna hai 
Project k route table me Demo ke vpc ka CIDR dalna hai


Setup Workspace for Demo and Project Both 

Demo workspace me ja k powershell se demo k private instance ko connect krne ka 

Project workspace me ja k powershell se project k private instance ko connect krne ka 

Then Demo k security group me jane ka and project ke Subnet ka CIDR copy kr ke waha paste krne ka
(Vpc then subnet me jyege toh CIDR milega)

Same project ke security group me jane ka and demo ke Subnet ka CIDR dalne ka 

Dono k Security group me yahi hona chahiye
A) ICMP {Subnet ka CIDR}
B) ALL TRAFFIC (SG GRP)
C) SSH MY IP

At Last demo k workspace me ja k powershell se project ke pvt ip ko ping krne ka toh ho jyega and  same for project ke isme demo k private IP ko dal k ping krne ka 


For deleting

1) Terminate instance
2) Delete peering 
3) Delete VPC 






---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



Transit Gateway -
====================

Create VPC 1  (public)
1 Az  lena h 10.0.0.0/16

Create VPC 2  (private)
1 Az lena h  10.2.0.0/16

Create VPC 3  (private)
1 Az lena h 10.3.0.0/16 



Go to Transit Gateway 
Select ASN 420000000000

Transit Gateway Attachment in left side list and Create Transit Gateway (VPC1) 
 Select Transit Gateway
VPC

VPC I'd me 1 Lena h private subnet


Create Transit Gateway (VPC2) 
 Select Transit Gateway
VPC

VPC I'd me 2 Lena h private subnet



Create Transit Gateway (VPC3) 
 Select Transit Gateway
VPC

VPC I'd me 3 Lena h private subnet


Launch 4 Instances 
1 with vpc 1  Public
1 with vpc 1 Private
1 with vpc 2 Private
1 with vpc 3 Private 

Change the hostnames of all the machines 
And send key to the public instance

VPC 1 k pvt k route me VPC 2 ka CIDR and VPC 3 ka (transit gateway)

VPC 2 pvt  me 1 and 3 k VPC ka CIDR range dalne ka (transit gateway)

VPC 3 pvt  me 1 and 2 ka Vpc ka CIDR range dalne ka (transit gateway)



Security group -
All traffic sg
Ssh anywhere 
All traffic anywhere
