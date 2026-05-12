 1: Cloud Platform Selection

Microsoft Azure was selected as the cloud platform for this practical because it provides robust virtual networking features such as Virtual Networks (VNets), subnets, and Network Security Groups (NSGs). Azure is widely used in enterprise environments and aligns with the learning objectives of the NET731 module.


Task 2: Virtual Network Creation

A Virtual Network (VNet) named NET731-VNet was created in Microsoft Azure using the private IPv4 address space 10.10.0.0/16. This address range was selected to allow sufficient capacity for subnet segmentation while supporting future network expansion. No subnets were created at this stage, as subnet configuration is addressed in a later task


Task 3: Subnet Configuration

Three subnets were created within the virtual network to logically separate network traffic based on function. The frontend subnet (10.10.1.0/24) is intended for public-facing resources such as web servers. The backend subnet (10.10.2.0/24) hosts application services, while the database subnet (10.10.3.0/24) is reserved for database resources. This design improves security, scalability, and network management through logical segmentation.


Task 4: IP Addressing Validation

The IP addressing scheme was reviewed to ensure correctness and consistency. All subnet address ranges fall within the virtual network address space of 10.10.0.0/16. Each subnet uses a unique /24 CIDR block, ensuring there is no overlap between subnets. This design supports efficient network segmentation while allowing sufficient IP capacity and scalability for future expansion.


Task 5: Network Security Groups

Network Security Groups (NSGs) were created to control network traffic within the virtual network. Three NSGs were provisioned: Frontend-NSG, Backend-NSG, and Database-NSG. Each NSG is intended to be associated with its respective subnet in order to enforce security controls based on the role of the network segment. Security rules are configured in subsequent tasks

