## Policy

**Security > Network Firewall > Console User Guide > Policy**

In the **Policy** tab, you can use the **ACL** feature to control traffic between VPCs connected to Network Firewall and inbound/outbound traffic, and the **Route** feature to specify the path for communication passing through Network Firewall.

<img src="https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/3.policy/policy1.png" height="65%" />

<br>

## Configure ACL

### Add

* Add policies based on departure, destination, and destination port.
    * Select the departure, destination, and destination port through already created objects.
* Policies can be added by configuring options such as the policy status (enabled/disabled), action (allow/block), schedule, and whether to log per policy.
* The schedule feature operates after the policy status is enabled. (The schedule feature does not apply if the policy is disabled.)

![policy2.PNG](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/3.policy/policy2.png)

### Copy

* Click **Copy** to copy a policy.
    * Copy: Copies the same policy as the one you want to copy.
    * Reverse copy: Copies the policy with the source and destination of the policy being copied swapped.
![policy3.PNG](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/3.policy/policy3.png)
    
### Modify

* Click **modify** to modify a policy.

### Move

* Click **Move** to move a policy.
    * Could not move below the default-deny policy.
![policy4.PNG](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/3.policy/policy4.png)

### Delete

* Click **Delete** to delete a policy.

### Batch Download of Policies

* Download all policies created in the Policy tab at once.

### Batch Register Policies

* You can register policies at once using the downloaded template.

![policy5.PNG](https://static.toastoven.net/prod_nfw/26.07.28/2.console-user-guide/3.policy/policy5.png)

!!! tip "Note"

    Copied policies are disabled. If needed, click **Modify** to enable the policy before use.


Deleted policies cannot be recovered, and the default-deny policy cannot be deleted.

<br>

## Configure Routing

![policy-route.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.09.12/policy-route.png)

### Add

* Click **Add** to select Ethernet, and enter the destination and gateway. 
    * Destination: Enter in subnet format
    * Ethernet: Select an Ethernet from the dropdown list.
    * Gateway: Enter in host format
  
### Modify

* Click **Modify** to modify a route.

### Delete

* Click **Delete** to delete a route.

!!! tip "Note"

    * If Ethernet is set to VPN, a gateway does not need to be specified.
    * For route settings for private IP ranges integrated with IPSec VPN, make sure to set Ethernet to VPN.
    * When entering a destination subnet, if the following validation message appears, check the subnet range in advance and enter the starting IP of the subnet.
        * [Examples]
            * 192.168.199.0/21 (X) → 192.168.192.0/21 (O)
            * 172.16.100.0/20 (X) → 172.16.96.0/20 (O)
            * 10.10.10.130/25 (X) → 10.10.10.128/25 (O)
            ![route_add.PNG](https://kr1-api-object-storage.nhncloudservice.com/v1/AUTH_2acdfabf4efe4efc8a04c00b348110c9/cdn_origin/prod_nfw/24.09.12/route_add.png)

!!! danger "Caution"

    * The default gateway of Network Firewall is the NAT Ethernet, and it cannot be modified or deleted.
    * If route settings are changed, communication issues may occur, so configure with caution. 