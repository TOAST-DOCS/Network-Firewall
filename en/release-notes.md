## July 28, 2026

### Added Features

* Added interface management feature
    * Interfaces can be freely created in the Interface tab and connected to Network Firewall.
* Added source NAT feature
    * NAT can be configured in Network Firewall when instances communicate externally.
        * Can be configured as 1:1 or N:1.

### Feature Updates

* Improved the route add screen
    * Changed to a dropdown format to allow selecting an interface based on the selected Ethernet without manually entering the gateway.
* Improved the ACL policy add screen
    * Improved the screen to allow selecting source/destination interfaces when adding an ACL policy.

### Removed Features

* Removed MTU size configuration option
    * Removed the MTU size configuration option for interfaces used in Network Firewall.

## October 28, 2025

### Feature Updates

* Improved the copy feature
    * Improved to support bidirectional policy copying.

### Removed Features

* Removed vulnerable algorithms
    * Removed encryption and integrity algorithms that are vulnerable to security attacks.
        * Encryption algorithms: DES, MD5, SHA1
        * Integrity algorithms: DH Groups 1, 2, 5

## April 29, 2025

### Added Features

* Added mirroring management feature
    * Traffic passing through Network Firewall can be copied and sent to a specific destination.

## October 15, 2024

### Added Features

* Added route management feature
    * Routes can be configured to branch and manage communication passing through Network Firewall.

### Feature Updates

* Improved the Network Firewall creation process
    * Improved to allow selection of availability zones when creating Network Firewall.

## July 23, 2024

### Feature Updates

* Added Network Firewall deletion feature
    * Added a feature to delete Network Firewall.
* Added Network Firewall configuration change feature
    * Added a feature to select the Network Firewall type as single or redundant.
* Improved traffic logs
    * Added column items displayed in traffic logs.

## June 25, 2024

### Added Features

* Added IPSec VPN management feature
    * Added IPSec VPN feature to enable secure private communication with remote locations.
* Added logging feature
    * Added a feature to configure whether to log per ACL policy.

### Feature Updates

* Improved the policy scheduling feature
    * Improved the UI to check whether a schedule is used or not in the policy page.
    * Improved to arrange schedules in 10-minute increments.
* Improved the monitor screen
    * Displayed internal and external sessions separately in the Sessions graph.
    * Improved the search conditions.

## May 14, 2024

### Added Features

* Added NAT edit feature
    * Added the "Edit" feature on the NAT main page.

## March 26, 2024

### Feature Updates

* Added MTU configuration feature
    * Added the ability to configure the MTU size of interfaces used in Network Firewall.
* Added Syslog port configuration feature
    * Added a feature to configure the port number when configuring Syslog.
* Improved UI
    * Improved the UI to display the protocol in log items as text instead of numbers.

### Removed Features

* Removed NAT configuration feature
    * Removed the NAT activation feature provided in Options and changed it to be automatically activated when Network Firewall is created.

## January 23, 2024

### Added Features

* Added integration with the SKM (Secure Key Manager) service for encrypting confidential information.

### Bug Fixes

* Fixed intermittent slow API responses.

## December 19, 2023

### Feature Updates

* Added quota management
    * Added a quota management feature to check resources by project.
* Added search conditions
    * Added search conditions for bulk policy downloads.
* Improved sensitive information handling
    * Improved to allow masking of sensitive information in logs stored in CloudTrail.

## October 31, 2023

### New Service Launch

Network Firewall is a network security service provided to safely protect the infrastructure assets used in NHN Cloud.