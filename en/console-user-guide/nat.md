<!-- machine_translated: true -->

<!-- pre-align:aligned sig=b5a6dd9155ad -->

<a id="nat"></a>
## NAT { #nat }

**Security > Network Firewall > Console User Guide > NAT**

The Network Address Translation (**NAT**) tab allows you to configure source NAT, which sets the public IP exposed externally when an instance communicates with the outside, and destination NAT, which connects a public IP dedicated to an instance that is to be accessed from the outside.

<br>

<a id="configure-source-nat"></a>
## Configure Source NAT { #configure-source-nat }

<a id="add"></a>
### Add { #add }

* Click **Add** to create a source NAT.
    * Objects to be selected in Pre-NAT IP must be created in advance in the **Object** tab before clicking **Add**.
    * For Post-NAT IP, select one of the IPs created in advance in **Network > Floating IP**. 

![nat_add.PNG](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/6.nat/nat2-pub.png)

<a id="modify"></a>
### Modify { #modify }

* Click **Modify** to modify the created source NAT.
    * You can modify both public and private IPs.

<a id="delete"></a>
### Delete { #delete }

* Click **Delete** to delete the created source NAT.

<br>

<a id="configure-destination-nat"></a>
## Configure Destination NAT { #configure-destination-nat }

<a id="configure-destination-nat-add"></a>
### Add { #configure-destination-nat-add }

* Click **Add** to create a destination NAT.
    * For Pre-NAT IP, select one of the IPs created in advance in **Network > Floating IP**.  
    * Objects to be selected in Post-NAT IP must be created in advance in the **Object** tab before clicking **Add**.

![nat_add.PNG](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/6.nat/nat3-pub.png)

<a id="configure-destination-nat-modify"></a>
### Modify { #configure-destination-nat-modify }

* Click **Modify** to modify the created destination NAT.
    * You can modify both public and private IPs.

<a id="configure-destination-nat-delete"></a>
### Delete { #configure-destination-nat-delete }

* Click **Delete** to delete the created destination NAT.

!!! tip "Note"

!!! danger "Caution"
    * When you add a source or destination NAT, the private IP before/after NAT that you select displays the objects created with **Type-Subnet** on the **Objects** tab at the time of addition.
        * Even if a selected object is modified or deleted on the **Objects** tab after adding NAT, it does not affect the NAT configuration (objects and NAT are not linked to each other).
        For example, if you select an object created with 10.10.10.10/32 when adding a destination NAT and then go to the **Objects** tab to modify that object from 10.10.10.10/32 to 10.10.10.20/32, the NAT configuration remains unchanged.