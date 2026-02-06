## Cloud and Security Analysis
### Cloud Services and Cost Evaluation 
Cloud computing allows organisations to acquire computing resources using the on-demand model without being compelled to invest in and support physical infrastructure. In the case of Truelec, whose business-critical service is the booking system used in multiple locations, cloud services provide a possibility to enhance the availability, scalability, and resilience and decrease the overhead of maintenance of the infrastructure in the long term (Kezron., 2025). This part analyses the aptness of cloud infrastructure over on-premises deployment and provides a cost-benefit analysis of Amazon Web Services (AWS) and Microsoft Azure.

An on-premises deployment would necessitate Truelec to buy new physical servers, which have become obsolete, and have other related storage, networking devices, power, cooling, and maintenance. This model comes with a huge initial investment and leaves the availability, fault tolerance and recovery of disasters fully on the organisation. Upgrading the system would require further hardware investment and possible service outage during upgrades to scale the system to serve more branch offices or even more users.

Contrary to this, the virtual machines associated with clouds are run on an operational expenditure model, meaning the resources are charged on a per-use basis. Cloud providers are provided with an in-built redundancy, distributed geographically dispersed data centres, and scalability. To have a customer-facing booking system that is still available at any time, cloud infrastructure ensures that there are no long outages and less complex capacity planning (Joel, Chibunna and Daraojimba, 2024). Thus, the deployment of the cloud is more appropriate to the operational and growth needs of Truelec than a solution based on on-premises.

To compare the opportunities of cloud providers, AWS and Azure have been chosen because they are mature, available in Australia, and widely used by enterprises. To make a fair comparison, the specifications of the virtual machine of the two providers were kept the same. Each setup will include a Linux-based virtual machine that has two virtual CPUs, eight gigabytes of memory, and about 100 gigabytes of solid-state storage, and it will run 24 hrs a month (Hasani et al., 2023). The official provider calculators were used to generate the pricing estimates, and the resulting Excel files have been provided as supporting evidence.

The AWS estimation is made using an EC2 t3.large with deployment in the Asia Pacific (Sydney) region. The monthly cost will be computed as USD 42.92, and the annual cost will be USD 515.04. The total expenses incurred in 5 years will amount to USD 2,575.20, as indicated in the AWS pricing export and 5-year cost comparison spreadsheet.
The estimate used in the Azure is an instance of a D2as v5 virtual machine in the Australia East region with one 128-gigabyte Standard SSD attached. It is estimated that the monthly cost will be USD 91.90, which will translate to annual USD 1,102.80 and a total of USD 5,514.00 in five years. The Azure pricing export supports these values and is summarised in the spreadsheet of the five-year comparison.

Cost-wise, AWS is much cheaper than Azure to support the chosen workload, and the total cost over five years is lower than that of Azure. The two platforms offer similar performance, reliability, and security, identity and access management, network isolation, and encryption support, as well as monitoring services (Akinade et al., 2025). Although Azure has good integration with Microsoft enterprise ecosystems, the same is not true with the Linux-based booking application of Truelec. AWS also has a wider service ecosystem and reduced prices of general-purpose workload computers.

Although both providers have free-tier or promotional credits, these are still short-term and are not suitable for long-term production systems. This is why the pay-as-you-go pricing was chosen in the first place to ensure the realistic operation costs of the pay-as-you-go pricing and to facilitate the correct comparison.

### Cybersecurity Controls and Mitigation Strategies

To counter the cybersecurity threats highlighted in Section 4.1, a set of technical, administrative, and operational security measures is recommended for the booking system of Truelec. These controls are consistent with the network architecture design, and they are aimed at minimising the risk and consequences of widely occurring enterprise threats.

Layered controls such as perimeter firewalls, cloud security groups, and network segmentation are applied to implement network security. The front-end elements do not have direct links to internal application and database layers, so the explicitly authorised traffic is permitted between network segments (Pendyala, 2025). Firewall policies are structured to allow only access to vital services like HTTPS, hence largely limiting the attack surface.

Role-based access control and the principle of least privilege are used in implementing identity and access management. There is limited administrative access to the servers with multi-factor authentication, and only the permissions that users need to carry out their job functions are assigned. This will minimise the chances of compromise of credentials and unauthorised access to the system.

Data protection is used during transmission and at rest. All communications between users, application servers, and databases are carried out with the help of Transport Layer Security (TLS), and stored data is encrypted by cloud-managed mechanisms (Damaraju, 2024). 

## Cloud Pricing Evidence

The following pricing exports were generated using official cloud provider calculators and are included in this repository:

- **AWS pricing export:**  
  [aws_vm_pricing.csv](cloud-pricing/aws_vm_pricing.csv)

- **Azure pricing export:**  
  [ExportedEstimate.xlsx](cloud-pricing/ExportedEstimate.xlsx)

- **Five-year cost comparison:**  
  [cloud_cost_5_years.xlsx](cloud-pricing/cloud_cost_5_years.xlsx)

