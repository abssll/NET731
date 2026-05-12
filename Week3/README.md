Virtual Machine Deployment

A virtual machine was deployed in Microsoft Azure using a low-cost B-series VM size. The virtual machine was created from scratch within a dedicated resource group and deployed in the South Africa North region.

- VM Name:** NET731-VM  
- VM Size:** B2ts_v2  
- Operating System:** Ubuntu Server 22.04 LTS  
- Region:** South Africa North  
- Resource Group:** NET731-RG  

The Standard B1s VM size specified in the task brief was not available in the selected region under the Azure for Students subscription. As an alternative, the B2ts_v2 size was selected as the closest low-cost equivalent.


Network Configuration

A custom virtual network and subnet were created to ensure proper network segregation and control.

- **Virtual Network:** Week3-VNet  
- **Address Space:** 10.20.0.0/16  
- **Subnet:** Week3-Subnet  
- **Subnet CIDR:** 10.20.1.0/24  

The virtual machine was assigned a static public IP address to ensure persistent connectivity. A Network Security Group was automatically created and associated with the network interface, allowing SSH access on port 22.


Auto-Shutdown Configuration

Auto-shutdown was enabled on the virtual machine and scheduled to occur daily at 13:00 (UTC+02:00). This configuration ensures that the virtual machine does not remain running unnecessarily, helping to reduce cloud costs and demonstrate responsible resource management practices.

