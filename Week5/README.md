
Task 1: Role-Based Access Control (RBAC)

Role-based access control was configured at the resource group level to ensure that users have appropriate permissions based on their job roles while following the principle of least privilege.

The following role assignments were implemented:

- user-ops: Assigned the Contributor role to allow deployment and management of Azure resources.
- user-audit: Assigned the Reader role to provide view-only access for monitoring and auditing purposes.
- user-data: Assigned the Storage Blob Data Contributor role to allow read and write access to blob storage containers without access to other Azure resources.

Roles were assigned at the resource group scope to ensure consistent access across all resources while maintaining a clear boundary and avoiding excessive permissions at the subscription level.


RBAC Scope Justification

Assigning roles at the resource group scope ensures that permissions apply only to the resources within that specific group, reducing security risks and isolating access. If roles were assigned at the subscription level, users such as user-ops would gain access to all resources in the subscription, which could lead to excessive privileges and potential misuse. Therefore, resource group scope provides a balance between accessibility and security.


Storage Account Name: net731storage
Containers: internal-docs, public-assets
Blob Endpoint: https://net731storage.blob.core.windows.net/
