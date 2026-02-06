### Cybersecurity Controls and Mitigation Strategies

To counter the cybersecurity threats highlighted in Section 4.1, a set of technical, administrative, and operational security measures is recommended for the booking system of Truelec. These controls are consistent with the network architecture design, and they are aimed at minimising the risk and consequences of widely occurring enterprise threats.

Layered controls such as perimeter firewalls, cloud security groups, and network segmentation are applied to implement network security. The front-end elements do not have direct links to internal application and database layers, so the explicitly authorised traffic is permitted between network segments (Pendyala, 2025). Firewall policies are structured to allow only access to vital services like HTTPS, hence largely limiting the attack surface.

Role-based access control and the principle of least privilege are used in implementing identity and access management. There is limited administrative access to the servers with multi-factor authentication, and only the permissions that users need to carry out their job functions are assigned. This will minimise the chances of compromise of credentials and unauthorised access to the system.

Data protection is used during transmission and at rest. All communications between users, application servers, and databases are carried out with the help of Transport Layer Security (TLS), and stored data is encrypted by cloud-managed mechanisms (Damaraju, 2024). 
