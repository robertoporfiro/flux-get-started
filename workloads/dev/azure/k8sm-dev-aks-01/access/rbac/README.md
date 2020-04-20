# RBAC overview

Role-based access control (RBAC) objects determine whether a user is allowed to perform a given action within a project.

Cluster administrators can use the cluster roles and bindings to control who has various access levels to the platform itself and all projects.

Developers can use local roles and bindings to control who has access to their projects. 
Note that authorization is a separate step from authentication, which is more about determining the identity of who is taking the action.

Authorization is managed using:

| Rules 	| Sets of permitted verbs on a set of objects. For example, whether a user or service account can create pods.
| Roles 	| Collections of rules. You can associate, or bind, users and groups to multiple roles.
| Bindings  | Associations between users and/or groups with a role.

There are two levels of RBAC roles and bindings that control authorization:

| Cluster RBAC | Roles and bindings that are applicable across all projects. Cluster roles exist cluster-wide, and cluster role bindings can reference only cluster roles.

| Local RBAC | Roles and bindings that are scoped to a given project. While local roles exist only in a single project, local role bindings can reference both cluster and local roles.