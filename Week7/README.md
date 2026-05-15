
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


Task 2.2: Network Metrics

The Network In Total and Network Out Total metrics were analysed using Azure Monitor to observe inbound and outbound traffic.

The network usage is relatively low and stable, with occasional spikes in outbound traffic. A noticeable spike in outbound traffic was observed, indicating a moment of increased data transmission. This behaviour is expected in a lab environment with minimal workload.
The network metrics are measured in bytes, typically displayed as kilobytes (KB) or megabytes (MiB). This is expected, as network traffic is measured based on the amount of data transferred.

Yes, both Network In and Network Out can be displayed on the same chart by using the "Add metric" feature in Azure Monitor. This allows multiple metrics to be analysed together for comparison.
The network traffic pattern shows low but consistent activity, with occasional spikes, particularly in outbound traffic. This indicates that the virtual machine is mostly idle but occasionally sends or receives data, which is expected in a lightly used environment.
