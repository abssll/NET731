
Task 1: Azure Monitor Metrics

Azure Monitor was used to collect performance data from the virtual machine.

The Percentage CPU metric was selected to monitor processor usage, while the Network In Total metric was used to observe incoming network traffic.

The CPU usage remained low, indicating minimal workload on the virtual machine. A spike in network activity was observed, showing that data was transmitted to the virtual machine.

These metrics demonstrate how Azure Monitor provides real-time insights into system performance and resource utilisation.


Task 1.1: Enable Monitoring on Virtual Machine

Azure Monitor was accessed through the virtual machine’s monitoring section. Basic monitoring was already active, allowing the collection of performance data such as CPU usage and availability.

The collected data is stored within Azure Monitor metrics and can be visualised directly in the Azure portal. If advanced monitoring is enabled, the data can also be stored in a Log Analytics workspace for deeper analysis.
These metrics demonstrate how Azure Monitor provides real-time visibility into system behaviour and resource utilisation.

Task 2.1: CPU Metrics

The Percentage CPU metric was analysed using Azure Monitor over a 30-minute time range.

The graph shows consistently low CPU usage, indicating that the virtual machine is running with minimal workload. Small fluctuations in CPU usage are visible, which are expected due to background system processes. The values align with expectations for a lightly used or idle virtual machine.
Multiple CPU-related metrics exist because they provide different perspectives of processor performance, such as average usage, maximum usage, and percentage utilisation. These metrics help in understanding system behaviour under different workloads and conditions.
