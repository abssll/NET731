
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

Task 3: Resources Monitoring

Monitoring was enabled on multiple Azure resources using Azure Monitor. The primary resource monitored was the virtual machine (week3-vm), where metrics such as CPU usage and network activity were collected using Azure Monitor Metrics.

Additionally, diagnostic settings were configured on the Network Security Group (NSG) and the Virtual Network (VNet). NSG logs included NetworkSecurityGroupEvent and NetworkSecurityGroupRuleCounter, which provide visibility into allowed and denied network traffic. VNet diagnostics captured network-level metrics and logs.

All diagnostic data from the NSG and VNet was sent to a central Log Analytics Workspace (week7-law) for aggregation, storage, and analysis.
The alert triggers when CPU usage exceeds 80% for 5 minutes. An email notification is sent to inform the administrator so that corrective action can be taken.


Monitoring is critical in a cloud environment because it provides real-time visibility into system performance, availability, and security. It helps detect issues early, such as high CPU usage or unusual network traffic, allowing administrators to respond quickly and prevent system failures.

In cloud environments, monitoring is highly automated and scalable, with built-in tools like Azure Monitor that can track resources across multiple regions and services. In contrast, on-premises monitoring is often limited to local infrastructure and requires manual setup, making it less flexible and harder to scale.


A metric is a numerical value collected at regular intervals, such as CPU usage or network traffic, used for monitoring performance and trends over time.

A log is a detailed record of events, such as system actions, errors, or security events, used for troubleshooting and auditing.

Metrics are typically used for performance monitoring and alerts, while logs are used for in-depth analysis and investigating specific issues.


If a virtual machine shows consistently high CPU usage at 2am, the first step would be to check scheduled tasks or background processes that may be running at that time. This could include system updates, backups, or automated scripts.

Next, logs and metrics would be reviewed to identify abnormal activity, such as unexpected spikes or repeated processes. Security should also be considered, as high CPU usage could indicate malicious activity such as unauthorized access or attacks.

Finally, performance monitoring tools would be used to determine if the workload is expected or if resources need to be scaled to handle demand.

Monitoring data can be used to identify underutilized resources and reduce unnecessary costs. For example, if CPU and network usage remain consistently low, the virtual machine size can be reduced to a smaller, more cost-effective option.

Monitoring can also detect inefficient workloads, excessive data transfer, or unused services, allowing administrators to optimize resource allocation.

By analysing usage patterns over time, organizations can make informed decisions about scaling resources up or down, improving both performance and cost efficiency.
