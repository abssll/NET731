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


Task 6: Requirements and Constraints

The cloud solution was implemented using Microsoft Azure, which was clearly selected and justified in Task 1. All IP addressing makes use of private IPv4 address ranges as defined in RFC 1918, with the virtual network using the 10.10.0.0/16 address space. Subnets are named descriptively based on their function, including Frontend-Subnet, Backend-Subnet, and Database-Subnet, to ensure clarity and ease of management.

Network Security Group rules are documented with justification to explain how traffic is controlled between network segments. All deployed Azure resources remain active and accessible for assessment purposes. The GitHub repository containing the documentation is publicly accessible or shared with the lecturer prior to the submission deadline, in compliance with the module requirements.


7.1 Address Space Design

The virtual network was designed using the private IPv4 address range 10.10.0.0/16, which complies with RFC 1918 for private networks. Each subnet was allocated a /24 address range, providing approximately 251 usable IP addresses per subnet. This allows sufficient capacity for current requirements while also supporting scalability if additional resources or services are added in the futur


7.2 Network Security Groups

Network Security Groups were designed to follow a least-privilege security approach. Public access is restricted to the frontend subnet, while internal subnets are protected from direct internet access. Different security rules apply to each subnet based on its role, ensuring that only necessary traffic is allowed. Both inbound and outbound traffic considerations were taken into account to prevent unnecessary exposure and reduce the attack surface of internal resources


7.3 GitHub and Documentation

The GitHub repository was structured to clearly present the Week 2 practical work, with documentation explaining each task and design decision. The README file provides sufficient detail for someone unfamiliar with the project to understand the network design. Clear and descriptive commit messages were used to reflect progress throughout the practical
