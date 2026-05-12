Task 1: Cloud Platform Selection

Microsoft Azure was selected as the cloud platform for this practical because it provides robust virtual networking features such as Virtual Networks (VNets), subnets, and Network Security Groups (NSGs). Azure is widely used in enterprise environments and aligns with the learning objectives of the NET731 module.


Task 2: Virtual Network Creation

A Virtual Network (VNet) named NET731-VNet was created in Microsoft Azure using the private IPv4 address space 10.10.0.0/16. This address range was selected to allow sufficient capacity for subnet segmentation while supporting future network expansion. No subnets were created at this stage, as subnet configuration is addressed in a later task


Task 3: Subnet Configuration

Three subnets were created within the virtual network to logically separate network traffic based on function. The frontend subnet (10.10.1.0/24) is intended for public-facing resources such as web servers. The backend subnet (10.10.2.0/24) hosts application services, while the database subnet (10.10.3.0/24) is reserved for database resources. This design improves security, scalability, and network management through logical segmentation.

