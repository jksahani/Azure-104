**Azure Networking Concepts 1**

1. Azure Virtual Network/ AWS-VPC
2. Subnets
3. Network Security Group
4. Public IPs
5. Private IPs
6. VNET Peering
7. Hub and Spoke Model





VNET1 10.0.0.0/16
Subnet1 10.0.1.0/24 VM2-RG1
Subnet2 10.0.2.0/24
    Peering
VNET2 10.2.0.0/16
Subn1 10.2.1.0/24  VM1-RG1
Subn2 10.2.1.0/22


VNET-Prod-----
VNET-UAT -----VNET-HUB
VNET-Dev------

VNET-HUB

NSG --- Network Security Group 

It is act as firewall, we can add allow or deny network rules. 
We can associate nsg to Subnet or resoures 


VM(NSG)---->Subnet(NSG)--VNET   <-------- traffic

allow rdp any any
deny any any any
