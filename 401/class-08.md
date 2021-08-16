# role-based access control 
* RBAC: is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

* role-based access control (RBAC): is an approach to restricting system access to authorized users, and  it's a policy-neutral access-control mechanism defined around roles and privileges
* The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments.
* RBAC can be used to facilitate administration of security in large organizations with hundreds of users and thousands of permissions.
* Although RBAC is different from MAC and DAC access control frameworks, it can enforce these policies without any complication.

## 5 steps to simple role-based access control (RBAC)
1. **Inventory your systems**
Figure out what resources you have for which you need to control access

2. **Analyze your workforce and create roles**
You need to group your workforce members into roles with common access needs.  

3. **Assign people to roles**
Now that you have a list of roles and their access rights, figure out which role(s) each employee belongs in, and set their access accordingly. 

4. **Never make one-off changes**
Resist any temptation to make a one-off change for an employee with unusual needs. If you begin doing this, your RBAC system will quickly begin to unravel. Change the roles as required or add new ones when really necessary. 

5. **Audit**
Periodically review your roles, the employees assigned to them, and the access permitted for each. If you discover, for example, that a role has unnecessary access to a particular system, change the role and adjust the access level for all employees in that role. 




# Q
1. When is Basic Authorization used vs. Bearer Authorization?
* The Basic authentication schemes are dedicated to the authentication using a username and a secret 
* The Bearer authentication scheme is dedicated to the authentication using a token

2. What does the JSON Web Token package do?
* defines a compact and self-contained way for securely transmitting information between parties as a JSON object. 
3. What considerations should we make when creating and storing a SECRET?
* Use encryption to store secrets within .git repositories
* Use environment variables
* Use “Secrets as a service” solutions




# Terms
* **Encryption** is the process of taking plain text, like a text message or email, and scrambling it into an unreadable format — called “cipher text.” This helps protect the confidentiality of digital data either stored on computer systems or transmitted through a network like the internet.
* **token** is a piece of a two-factor authentication security device that may be used to authorize the use of computer services. 
* **Bearer authentication**  (also called token authentication) is an HTTP authentication scheme that involves security , Bearer authentication is a security scheme with type: http and scheme: bearer . 
* **secret** These non-human privileged credentials are often called “secrets” and refer to a private piece of information that acts as a key to unlock protected resources or sensitive information in tools, applications, containers, DevOps and cloud-native environments.
* **JSON Web Token** is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. The tokens are signed either using a private secret or a public/private key

