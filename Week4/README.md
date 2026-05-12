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

Question 4:
Assigned membership was selected when creating the security groups. Assigned membership allows administrators to manually control which users belong to each group, reducing the likelihood of unintended access. This approach is suitable for small to medium environments where user roles are stable and administrative oversight is required.
Dynamic membership would be preferable in larger organisations where users frequently change roles or departments and group membership can be automatically managed using user attributes such as department or job title.

Question 5:
Group membership was verified by navigating to Microsoft Entra ID → Groups, opening a security group, and reviewing the Members tab. This verification step ensures that the correct users are assigned to each group and confirms that no user belongs to multiple groups. A screenshot of a group’s members list was captured as evidence.

Question 6:

The Contributor role was assigned to the proj-orion-dev group because members of the development team require the ability to create, modify, and manage Azure resources such as virtual machines, storage accounts, and networking components. This role supports the development lifecycle while preventing access to role assignments, maintaining security boundaries.

The Reader role was assigned to the proj-orion-ops group to allow the operations team to view Azure resources for monitoring, troubleshooting, and auditing purposes without granting permission to make configuration changes. This helps reduce the risk of accidental or unauthorised modifications to production resources.

The proj-orion-finance group was intended to receive the Billing account reader role at the billing scope. This role provides read-only access to cost and billing information without exposing infrastructure resources or configuration settings. Due to limitations of the personal Azure subscription used for this project, group-based role assignment at the billing scope was not available. In an enterprise environment, this role would be assigned to the finance group by a billing administrator.

Question 7:

Roles for this project were assigned at the Subscription scope. Assigning roles at this level ensures that permissions apply consistently across all resources within the subscription and simplifies access management.

Assigning roles at a broader scope, such as a Management Group, could result in excessive permissions being granted beyond what is required for the project. Conversely, assigning roles at narrower scopes, such as Resource Groups or individual resources, would increase administrative complexity and make access management more difficult to maintain. Subscription-level scope provides a balanced approach between security, visibility, and manageability for a project-based environment.

Question 8

Azure built-in roles provide predefined sets of permissions designed to cover common operational responsibilities, such as Contributor and Reader. Built-in roles are generally preferred because they are maintained by Microsoft and reduce the complexity of access management.

A custom role is a role created by an organisation to define a specific set of permissions that are not fully met by built-in roles. An organisation may need to create a custom role when built-in roles grant too many permissions or when strict regulatory, compliance, or operational requirements demand more precise access control. While custom roles offer greater flexibility, they also require additional management and ongoing maintenance.
