# Event Driven Applications

* **Event-Driven Programming** is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.

* **Event-Driven Programming concepts**
    1. An Event Handler is a callback function that will be called when an event is triggered.
    2. A Main Loop listens for event triggers and calls the associated event handler for that event.
* **EventEmitter** is a module provides from *node.js* allows us to get started incorporating Event-Driven Programming in our project right away.
 
 ``const EventEmitter = require('events').EventEmitter;``

``const myEventEmitter = new EventEmitter;``

* To **remove event** listeners in EventEmitter we can use the ``removeListener`` or ``removeAllListeners`` method


# Q 
1. Why is access control important?
- limit access to information and information processing systems
- Reduce the risk of information being accessed without the appropriate authorisation, unlawfully and the risk of a data breach. 

2. Describe an application that would need access control.
- They apply anywhere access is required to perform a business activity and should be adhered to when accessing information in any format, on any device.

3. What is a role used for?
- facilitate administration of security in large organizations with hundreds of users and thousands of permissions.because not every employee needs a starring role and access to every thing 

4. 
- **RBAC** takes more of a real world approach to structuring access control. Access under RBAC is based on a user's job function within the organization to which the computer system belongs
- Once implemented **MAC** also imposes a high system management overhead due to the need to constantly update object and account labels to accommodate new data, new users and changes in the categorization and classification of existing users.
- **Discretionary Access Control** increases the risk that data will be made accessible to users that should not necessarily be given access.


# Terms 
* **Authorization** :is the function of specifying access rights/privileges to resource
* **Role Based Access Control:** (RBAC) is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.
* **capability** (known in some systems as a key) is a *communicable, unforgeable token of authority*. It refers to a value that references an object along with an associated set of access rights. A *user program on a capability-based operating system must use a capability to access an object*.
