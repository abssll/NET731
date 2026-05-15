<img width="681" height="729" alt="image" src="https://github.com/user-attachments/assets/c8cc05d3-d8a1-4bb7-a61c-6a86829e93f9" />
Task 1: Azure Budget Alerts

A budget was created in Azure Cost Management to monitor spending. The budget was set to $100 per month and configured with two alert thresholds at 80% and 100%.

Email notifications were added to ensure alerts are received when spending approaches or exceeds the budget. This helps prevent overspending and supports effective cost management.


Task 2: Monitor Usage and Adjust Resource Settings

Cost Analysis:

Azure Cost Analysis was used to review current spending. The data showed that there was minimal or no significant cost recorded during the selected period. This is likely due to limited usage of resources and the short duration of resource activity.

imated Monthly Cost

Based on the current usage pattern, the monthly cost is expected to remain very low and well within the $100 budget. This demonstrates effective cost management and resource control.

# Week 8 – Cost Management Report

Budget Configuration:

A monthly budget was created in Azure Cost Management to monitor spending and prevent overspending.

- Budget Name: week8-budget  
- Scope: Azure Subscription  
- Budget Amount: $100 per month  
- Alerts:
  - 80% (Actual spend) – Early warning  
  - 100% (Forecasted spend) – Predicted overspend alert  
- Notifications: Email alert configured  

The budget ensures that spending is monitored and users are notified before exceeding limits.

 Top 3 Cost Resources

The Cost Analysis tool was used to review resource usage.

Due to the limited usage of resources in this lab environment, no significant cost was recorded during the selected period. However, based on typical Azure usage patterns, the following resources are expected to be the most expensive:

1. Virtual Machine (week3-vm)  
   - Highest cost due to compute usage when running  

2. Storage Account  
   - Small cost associated with data storage  

3. Networking Resources  
   - Minimal cost related to data transfer  

The virtual machine typically represents the highest cost because it continuously uses compute resources when active.

Cost Adjustment (Task 2)

To optimise costs, the virtual machine was stopped when not in use.

Impact of Change:
- Reduced compute charges  
- Prevented unnecessary spending  
- Resource remains available without deletion  

This is an effective cost-saving strategy as compute resources are the primary cost drivers in Azure environments.

Projected Monthly Spend

Based on current usage patterns, the projected monthly spend is expected to remain very low and well within the $100 budget.

Since the virtual machine is not running continuously, the overall cost is significantly reduced.

Recommendations for Cost Management

To manage Azure costs effectively, the following recommendations are suggested:

- Stop unused virtual machines when not needed  
- Use smaller VM sizes for low workloads  
- Monitor spending regularly using Cost Analysis tools  
- Set budgets and alerts to track usage  
- Remove unused resources to avoid unnecessary costs  

By following these practices, users can control cloud spending and maintain efficient use of resources.
