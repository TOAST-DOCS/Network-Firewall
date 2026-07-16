## Object

**Security > Network Firewall > Console User Guide > Object**

In the **Object** tab, you can create and manage the IPs and ports to be used when creating policies.

![(object1)](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/4.object/object1.png)

<br>

## Configure Objects

### Add

* Create an object by entering the required fields.
    * Objects can be added in two forms: IP and port.
![(object2)](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/4.object/object2.png)

### Modify

* Click **Modify** to modify an object.
    * Types cannot be modified.

### Delete

* Click **Delete** to delete an object.
    * Objects automatically created by Network Firewall cannot be modified or deleted.

### Add Instance Object
* Add objects by leveraging the instances that exist within the project where Network Firewall was created.
![(object3)](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/4.object/object3.png)

### Batch Download of Objects

* You can download all IP and port objects created in the **Object** tab at once.

!!! tip "Note"
\* Group objects cannot be added when creating a group object (only individual or range objects can be selected and added).
\* Objects are created by simply referencing the instance name and private IP address, regardless of the instance itself. Created objects are managed in the **Object** tab.

!!! danger "Caution"
Objects in use by a policy will be changed to ALL objects after deletion.