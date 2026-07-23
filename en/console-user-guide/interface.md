## Interface

**Security > Network Firewall > Console User Guide > Interface**

In the **Interface** tab, you can create and manage interfaces to be used for the Network Firewall.

<br>

## Configure Interface

### Add
* Click **Add** to add an interface.
    * Enter a name and select a VPC and subnet.
![(interface2)](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/5.interface/interface2.png)

### Modify
* Click **Modify** to modify an interface.
    * VPC and subnet cannot be modified.

### Delete
* Click **Delete** to delete an interface.

### Enable/Disable
* You can set the interface to be enabled or disabled from the overflow menu.
![(interface4)](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/5.interface/interface4.png)

!!! tip "Note"

    Only the name and description can be modified.

!!! danger "Caution"
    
    * Interfaces in use cannot be deleted.
        * An interface can only be deleted if it is not used in ACL and route settings and is set to disabled in the Interface tab.
    * Setting an interface currently in use to "Disabled" may affect communication.
    * Information on created interfaces can be viewed in [Network > Network Interface].
        * If a Virtual_IP type interface created in Network Firewall is modified, disabled interfaces will no longer be usable, and interfaces already in use may affect communication.