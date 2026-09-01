<!-- pre-align:aligned sig=f90308ef9ace -->

<a id="network-firewall-release-notes"></a>
## Network Firewall Release Notes { #network-firewall-release-notes }

**Security > Network Firewall > Release Notes**

<a id="july-28-2026"></a>
## July 28, 2026 { #july-28-2026 }

<a id="added-features"></a>
### Added Features { #added-features }

* Added interface management feature
    * Interfaces can be freely created in the Interface tab and connected to Network Firewall.
* Added source NAT feature
    * NAT can be configured in Network Firewall when instances communicate externally.
        * Can be configured as 1:1 or N:1.

<a id="feature-updates"></a>
### Feature Updates { #feature-updates }

* Improved the route add screen
    * Changed to a dropdown format to allow selecting an interface based on the selected Ethernet without manually entering the gateway.
* Improved the ACL policy add screen
    * Improved the screen to allow selecting source/destination interfaces when adding an ACL policy.

<a id="removed-features"></a>
### Removed Features { #removed-features }

* Removed MTU size configuration option
    * Removed the MTU size configuration option for interfaces used in Network Firewall.

<a id="october-28-2025"></a>
## October 28, 2025 { #october-28-2025 }

<a id="october-28-2025-feature-updates"></a>
### Feature Updates { #october-28-2025-feature-updates }

* Improved the copy feature
    * Improved to support bidirectional policy copying.

<a id="october-28-2025-removed-features"></a>
### Removed Features { #october-28-2025-removed-features }

* Removed vulnerable algorithms
    * Removed encryption and integrity algorithms that are vulnerable to security attacks.
        * Encryption algorithms: DES, MD5, SHA1
        * Integrity algorithms: DH Groups 1, 2, 5

<a id="april-29-2025"></a>
## April 29, 2025 { #april-29-2025 }

<a id="april-29-2025-added-features"></a>
### Added Features { #april-29-2025-added-features }

* Added mirroring management feature
    * Traffic passing through Network Firewall can be copied and sent to a specific destination.

<a id="october-15-2024"></a>
## October 15, 2024 { #october-15-2024 }

<a id="october-15-2024-added-features"></a>
### Added Features { #october-15-2024-added-features }

* Added route management feature
    * Routes can be configured to branch and manage communication passing through Network Firewall.

<a id="october-15-2024-feature-updates"></a>
### Feature Updates { #october-15-2024-feature-updates }

* Improved the Network Firewall creation process
    * Improved to allow selection of availability zones when creating Network Firewall.

<a id="july-23-2024"></a>
## July 23, 2024 { #july-23-2024 }

<a id="july-23-2024-feature-updates"></a>
### Feature Updates { #july-23-2024-feature-updates }

* Added Network Firewall deletion feature
    * Added a feature to delete Network Firewall.
* Added Network Firewall configuration change feature
    * Added a feature to select the Network Firewall type as single or redundant.
* Improved traffic logs
    * Added column items displayed in traffic logs.

<a id="june-25-2024"></a>
## June 25, 2024 { #june-25-2024 }

<a id="june-25-2024-added-features"></a>
### Added Features { #june-25-2024-added-features }

* Added IPSec VPN management feature
    * Added IPSec VPN feature to enable secure private communication with remote locations.
* Added logging feature
    * Added a feature to configure whether to log per ACL policy.

<a id="june-25-2024-feature-updates"></a>
### Feature Updates { #june-25-2024-feature-updates }

* Improved the policy scheduling feature
    * Improved the UI to check whether a schedule is used or not in the policy page.
    * Improved to arrange schedules in 10-minute increments.
* Improved the monitor screen
    * Displayed internal and external sessions separately in the Sessions graph.
    * Improved the search conditions.

<a id="may-14-2024"></a>
## May 14, 2024 { #may-14-2024 }

<a id="may-14-2024-added-features"></a>
### Added Features { #may-14-2024-added-features }

* Added NAT edit feature
    * Added the "Edit" feature on the NAT main page.

<a id="march-26-2024"></a>
## March 26, 2024 { #march-26-2024 }

<a id="march-26-2024-feature-updates"></a>
### Feature Updates { #march-26-2024-feature-updates }

* Added MTU configuration feature
    * Added the ability to configure the MTU size of interfaces used in Network Firewall.
* Added Syslog port configuration feature
    * Added a feature to configure the port number when configuring Syslog.
* Improved UI
    * Improved the UI to display the protocol in log items as text instead of numbers.

<a id="march-26-2024-removed-features"></a>
### Removed Features { #march-26-2024-removed-features }

* Removed NAT configuration feature
    * Removed the NAT activation feature provided in Options and changed it to be automatically activated when Network Firewall is created.

<a id="january-23-2024"></a>
## January 23, 2024 { #january-23-2024 }

<a id="january-23-2024-added-features"></a>
### Added Features { #january-23-2024-added-features }

* Added integration with the SKM (Secure Key Manager) service for encrypting confidential information.

<a id="bug-fixes"></a>
### Bug Fixes { #bug-fixes }

* Fixed intermittent slow API responses.

<a id="december-19-2023"></a>
## December 19, 2023 { #december-19-2023 }

<a id="december-19-2023-feature-updates"></a>
### Feature Updates { #december-19-2023-feature-updates }

* Added quota management
    * Added a quota management feature to check resources by project.
* Added search conditions
    * Added search conditions for bulk policy downloads.
* Improved sensitive information handling
    * Improved to allow masking of sensitive information in logs stored in CloudTrail.

<a id="october-31-2023"></a>
## October 31, 2023 { #october-31-2023 }

<a id="new-service-launch"></a>
### New Service Launch { #new-service-launch }

Network Firewall is a network security service provided to safely protect the infrastructure assets used in NHN Cloud.