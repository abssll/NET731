Task 1:

Question 1:
A consistent naming convention is important in an enterprise environment because it improves clarity, accountability, and manageability. It allows administrators to easily identify users, reduces the risk of duplicate or ambiguous accounts, and supports automation and auditing processes. Consistent naming also aligns with security best practices and makes it easier to manage access controls across systems. For example alex.mokoena@novatechsolutions.co.za

Question 2:
Three Security Groups will be created in Microsoft Entra ID, one for each department:

proj-orion-dev
proj-orion-ops
proj-orion-finance

Security Groups are the correct choice because they are specifically designed to control access to Azure resources using role-based access control (RBAC). Unlike Microsoft 365 groups, which are focused on collaboration tools such as Teams and Outlook, Security Groups integrate directly with Azure permissions and subscriptions. This makes them ideal for assigning Azure roles and enforcing access control based on departmental responsibilities.

Question 3:
The principle of least privilege means that users are granted only the minimum level of access required to perform their job functions and nothing more. This principle reduces security risks by limiting the potential damage caused by user error, misuse, or compromised accounts.
Before assigning any roles, access requirements must be carefully analysed so that each department receives only the permissions necessary for their responsibilities. For example, development users should not have access to financial resources, and finance users should not be able to modify infrastructure settings. Applying least privilege ensures a secure, controlled environment and aligns with industry security best practices.

Task 2: Group Membership Allocation
Users were assigned to groups based on their department and job role. Each user belongs to exactly one group to ensure clear access boundaries and to enforce the principle of least privilege.
The group membership structure is as follows:


proj-orion-dev

Alex Mokone
Jordan Nkosi


proj-orion-ops

Sam Patel
Lebo Dlamini


proj-orion-finance

Fatima Khan
Daniel Meyer

This structure ensures that access permissions can be granted at the group level rather than individually, simplifying administration and reducing the risk of incorrect access assignments.
