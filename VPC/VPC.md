# Virtual Priavte CLoud(VPC)

Key Notes

---

 - Region Resilent
 - Divided into different subnets in each Availability Zone
 - Default CIDR - 172.31.0.0/16
 - 2 Types of VPC(Default and Custom)


Default VPC Facts

 - By default is private and isolated
 - 1 Default VPC per region per AWS account
 - Available on One per each region. Default VPCs can be deleted/removed and recreated
 - Always using a Default CIDR is 172.31.0.0.1/16
 - Inside a default VPC, /20 gets use Subnet in AZ 
 - By default a Security Group, Internetgateway and a network ACL is created on a default VPC
 - The subnet assign is default to IPV4
 - Default VPCs can be created not from Create VPC button but it is located in Actions button  



 Custom VPC Facts

  - Regional Resilient
  - Isolated Network
  - Supports Hybrid networking( can be pair to on-premise or other cloud services)
  - Uses IPV4 Private CIDR and Public IPs
  - Minimum of /28(16 IPs) and Max of /16 (65, 536 IPs) Allocated
  - IPV6 /56 CIDR Block default use
  - DNS is provided by default by Route 53
      - If <span style="color:red"> enableDNSHostNames </span> is set to true, instances get a public DNS 
      - If <span style="color:red"> enableDNSSupport </span> is set to true, instances can use DNS. 