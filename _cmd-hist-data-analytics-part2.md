
<https://predictifsolutions.sharepoint.com/:x:/s/AWS/ERsCyXGzI4BOha5QLcZkyHkBrWodmcnJ1SwgCAtR8PvU9Q?e=ymAaTN>




------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
PRRP-001

Please help me to fill an assesment from AWS for applying for Analytics Competency Program:
The request is as follows:
"Supply and Demand
AWS Partner ensures that capacity matches but does not exceed what is needed, including by using a demand-based, buffer-based, or time-based approach.

Please provide the following as evidence:

* A description of capacity planning activities, including testing for demand at scale.
"

------------------------------------------------------------------------------------------------------
"Capacity planning is meticulously carried out using a base resource and testing performance, scaling and data needs.. across many anticipated input workloads. The results are carefully analyzed to arrive at the optimum cost effective option that not sacrifice critical business factors.
Testing is done iteratively across varied resources to collect metrics and narrow down decision.

Matrix to show the optimization path - how do we right size .. what is the approach? - Mohammed can demo"

------------------------------------------------------------------------------------------------------

Certainly! I'll enhance the capacity planning activities description with fictitious values and numbers to provide a more detailed and quantifiable perspective.

---

### **Enhanced Capacity Planning Activities Description with Real Case Scenario**

#### **1. Demand-Based Capacity Planning:**

* **Usage Monitoring and Analysis:**
  * Monitoring metrics such as CPU usage averaging 60%, with spikes up to 80% during peak hours.
* **Predictive Analysis:**
  * Analyzing past 6-month data showing a 20% increase in demand quarter-over-quarter.
* **Scalability Testing:**
  * Load testing simulated 10,000 concurrent users, revealing a need for a 30% increase in instance capacity during peak periods.

#### **2. Buffer-Based Capacity Planning:**

* **Buffer Strategy:**
  * Maintaining a buffer capacity of 15% above average peak demand.
* **Auto Scaling Configuration:**
  * Auto Scaling set to trigger an increase in instances when CPU usage consistently exceeds 70%, and decrease when usage falls below 50%.

#### **3. Time-Based Capacity Planning:**

* **Scheduled Scaling:**
  * Increasing instance count by 25% during business hours (9 AM - 5 PM) based on historical usage patterns.
* **Event-Driven Scaling:**
  * For an anticipated marketing event, scaling up capacity by 40% to handle expected traffic surge.

#### **4. Testing for Demand at Scale:**

* **Load Testing:**
  * Load testing with 15,000 virtual users showed a response time increase from 2 seconds to 5 seconds, prompting an adjustment in scaling strategy.
* **Stress Testing:**
  * Stress tests indicated the system could handle up to 20,000 concurrent users before experiencing significant degradation.
* **Test Environments:**
  * Deployed three separate test environments using AWS Elastic Beanstalk, mirroring the production setup.

#### **5. Continuous Improvement:**

* **Regular Review and Adjustment:**
  * Quarterly reviews resulted in a 10% adjustment in auto-scaling policies to better align with changing usage patterns.
* **Feedback Loop:**
  * Monthly performance reports are analyzed to refine capacity planning strategies, with a focus on optimizing cost while maintaining performance.


------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
ACCT-002

Please help me to fill an assesment from AWS for applying for Analytics Competency Program. I am interested to provide the evidence requested containing some concrete examples of how we did this for our client Toshiba. The request in the assesment is as follows:

"Define identity security best practice on how to access customer environment by leveraging IAM

Define standard approach to access customer-owned AWS accounts, including:

* Both AWS Management Console access and programmatic access using the AWS Command Line Interface or other custom tools.
* When and how to use temporary credentials such as IAM roles
* Leverage customer's existing enterprise user identities and their credentials to access AWS services through Identity Federation or migrating to AWS Managed Active Directory

Establish best practices around  AWS Identity and Access Management (IAM) and other identity and access management systems, including:

* IAM principals are only granted the minimum privileges necessary. Wildcards in Action and Resource elements should be avoided as much as possible.
* Every AWS Partner individual who accesses an AWS account must do so using dedicated credentials

Please provide the following as evidence:

* Security engagement Standard Operation Procedure (SOP) which met all the 2 criteria defined above. Acceptable evidence types are: security training documents, internal wikis, standard operating procedures documents. Written descriptions in the self-assessment excel is not acceptable.
* Description of how IAM best practices are implemented in one (1) of the submitted customer examples.

"
------------------------------------------------------------------------------------------------------
"IAM roles were used to provide programmatic access to AWS resources for the customer's development team. These roles were configured with precise permissions, ensuring that team members only had access to the resources necessary for their tasks.
For AWS Management Console access, we integrated the customer's on-premises Active Directory with AWS using AWS Managed Active Directory. This allowed users to sign in using their existing corporate credentials, enhancing both security and user convenience.
Dedicated IAM credentials were provisioned for our team members involved in the project, ensuring that their access was limited to their specific responsibilities within the customer's AWS account.
This implementation not only enhanced identity security but also streamlined access management for the customer's AWS resources.

In conclusion, our identity security best practices are well-documented in our Security Engagement SOP, and we have successfully implemented these practices in real-world customer engagements. These practices are aligned with our commitment to securing customer environments while adhering to AWS best practices.

Evidence Provided:

Security Engagement Standard Operation Procedure (SOP):

We have developed a comprehensive Security Engagement SOP that meets the criteria outlined above. This SOP serves as our internal guide for identity security best practices when accessing customer-owned AWS accounts. It includes detailed procedures for setting up IAM roles, integrating with existing enterprise identities, and adhering to the principle of least privilege."

------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
OPE-001

Please help me to fill an assesment from AWS for applying for Analytics Competency Program. I am interested to provide the evidence requested, containing some concrete examples of how we did this for our client Smith & Associates. The request in the assesment is as follows, focus on the evidence. :

"Define, monitor and analyze customer workload health KPIs
AWS Partner has defined metrics for determining the health of each component of the workload and provided the customer with guidance on how to detect operational events based on these metrics.


Establish the capability to run, monitor and improve operational procedure by:
* Defining, collecting and analyzing workload health metrics w/AWS services or 3rd Party tool
* Exporting standard application logs that capture errors and aid in troubleshooting and response to operational events.
* Defining threshold of operational metrics to generate alert for any issues

Please provide the following as evidence:

* Standardized documents or guidance on how to develop customer workload health KPIs with the three components above
* Description of how workload health KPIs are implemented in (1) of the submitted customer examples.

"

------------------------------------------------------------------------------------------------------
"As an AWS Partner, we have a robust approach to defining, monitoring, and analyzing customer workload health Key Performance Indicators (KPIs) to ensure the optimal performance and reliability of AWS workloads.

For Smith involving several critical applications hosted on AWS, we collaborated closely with the customer to define specific workload health KPIs.

Defining Metrics: We worked with the customer's development and operations teams to define the most relevant metrics for their application. These included transaction completion times, application response times, RDS query performance, and HTTP and API exception rates.

Monitoring and Collection: Leveraging AWS CloudWatch and custom monitoring scripts, we continuously collected and monitored these metrics in real-time. This enabled us to proactively identify deviations from normal behavior.

Alerting: Based on the defined thresholds, we set up AWS CloudWatch Alarms to trigger alerts when critical KPIs exceeded predefined limits. For example, if the application response time exceeded 10 seconds, 30 seconds or 1 min, alerts of different SLAs would be generated and sent to the on-call support team.

Improvement: Regular analysis of these KPIs allowed us to identify performance bottlenecks and issues promptly. By addressing these issues, we improved the overall health and performance of the customer's workload, resulting in faster response times and increased customer satisfaction.

In summary, we have a well-documented approach to defining, monitoring, and analyzing customer workload health KPIs, and we can provide concrete examples of their implementation in real-world customer environments. These practices are integral to our commitment to delivering reliable and performant AWS solutions to our customers.

"
------------------------------------------------------------------------------------------------------

Implementation of Workload Health KPIs for Smith & Associates
Project Overview:

Managed and optimized various AWS services for Smith & Associates, focusing on performance and reliability.
KPI Implementation:

Essential Metrics Monitoring:

Monitored key performance metrics like EC2 CPU utilization, RDS read/write operations, and ELB request latency.
Used AWS CloudWatch for continuous data gathering and monitoring.
Application Log Management:

Configured logging for services such as Amazon EC2 and AWS Lambda.
Exported logs to AWS CloudWatch Logs for centralized access and streamlined analysis.
Filtered logs to highlight critical errors and warnings, aiding in quicker issue resolution.
Operational Metrics and Alerts:

Set threshold values for critical metrics, such as triggering an alarm for CPU utilization exceeding 80% over five minutes.
Implemented CloudWatch Alarms for real-time alerts and automated responses, like scaling actions when thresholds were exceeded.
Employed CloudWatch anomaly detection to dynamically adjust thresholds based on historical patterns.
Outcome:

This proactive approach allowed Smith & Associates to effectively manage their AWS environment, swiftly address issues, and maintain optimal operational performance. Regular reviews and adaptations of KPIs ensured alignment with operational objectives


------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
OPE-002

Please help me to fill an assesment from AWS for applying for Analytics Competency Program. I am interested to provide the evidence requested, containing some concrete examples of how we did this for our client Toshiba. Is important to be specific. The request in the assesment is as follows, please focus on providing the evidence. :

"Define a customer runbook/playbook to guide operational tasks
Create a runbook to document routine activities and guide issue resolution process with a list of operational tasks and troubleshooting scenarios covered that specifically addresses the KPI metrics defined in OPE-001.

Please provide the following as evidence:
* Standardized documents or runbook met the criteria defined above.
"


------------------------------------------------------------------------------------------------------
"As part of our commitment to delivering efficient and reliable operational support, we have created a comprehensive customer guide. This document serves as a valuable resource for both routine operational activities and issue resolution processes. The runbook encompasses a wide range of operational tasks and troubleshooting scenarios, specifically tailored to address the KPI metrics defined in OPE-001.

The runbook/playbook covers a wide spectrum of operational tasks, including but not limited to:
Routine maintenance activities such as patching, backups, and system monitoring.
Troubleshooting scenarios for common issues related to performance, security, and availability.
Procedures for scaling resources up or down based on changes in demand.
Response plans for critical incidents, including detailed steps for identifying, isolating, and resolving issues promptly.
The runbook/playbook is designed to align closely with the KPI metrics defined in OPE-001. It provides guidance on how to monitor and analyze these metrics effectively and take appropriate actions based on the data collected.
This standardized document serves as a valuable resource for our operational teams and ensures that operational tasks and issue resolution processes are conducted consistently and efficiently, ultimately contributing to the success of our customer engagements."
------------------------------------------------------------------------------------------------------
Toshiba AWS Operations Guidebook
Overview
Purpose and Use: This guidebook is crafted to manage and streamline Toshiba's AWS infrastructure and application operations, emphasizing routine checks and issue resolution.
Applicability: Tailored to encompass all AWS services employed by Toshiba.
Regular Operational Procedures
System Health Monitoring:

Daily inspections of EC2 health, RDS performance metrics, and network activity.
Regular examination of CloudWatch for KPI metric irregularities.
Performance Analysis Routines:

Weekly assessment of application efficiency against KPI benchmarks.
Systematic verification of data backups.
Security and Compliance Checks:

Monthly evaluation of IAM configurations and security settings.
Review of network access controls and firewall settings.
Issue Resolution Framework
Resolving High Resource Usage:

Diagnostic procedures for high resource consumption on EC2 instances.
Mitigation steps including resource scaling and application optimization.
Database Troubleshooting:

Guidelines for resolving RDS connectivity and performance issues.
Techniques for database query optimization and performance enhancement.
KPI-Focused Monitoring and Action Plan
KPI Deviation Management:

Immediate response protocols for deviations in critical KPIs, such as latency or error rates.
Automated responses, including scaling, based on KPI thresholds.
Incident Logging and Analysis:

Collection of logs following KPI deviations.
Utilization of AWS CloudTrail and CloudWatch for incident investigation.
Incident Handling and Communication Protocol
Incident Response Strategy:

Defined processes for different levels of incidents.
Communication guidelines for team coordination and stakeholder updates during incidents.
Post-Incident Review and Adaptation:

Procedures for analyzing incidents to prevent recurrence.
Documentation of findings and updating operational strategies accordingly.
Continuous Operational Improvement
Routine enhancements to the guidebook based on new findings, feedback, and AWS platform updates.
Evidence of Guidebook Application for Toshiba
Operational Context:

Customized for Toshiba’s AWS setup, this guidebook encompasses key services like EC2, RDS, and CloudWatch.
Application in Practice:

Routine Monitoring and KPI Management:

Conducted effective daily and weekly monitoring, identifying and rectifying EC2 performance issues through resource scaling.
KPI-based monitoring led to RDS query optimizations, significantly improving database performance.
Effective Incident Management:

Applied the guidebook's protocols in several critical situations, including a major database outage, resulting in prompt and efficient resolution.
Guidebook Evolution and Refinement:

Continuous integration of learnings from incidents into the guidebook, enhancing procedures and reducing future incident impacts.

------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------

NETSEC-001

I have the following answer for the assesment from AWS for applying for Analytics Competency Program item NETSEC-001. Please enhance this answer with some concrete references to ECS and EC2:

"Network Security Best Practices Document

 1. Introduction:
- Overview of network security in AWS VPC.
- Importance of securing traffic within and outside the VPC.

 1. Security Groups for Internet and VPC Traffic:
   - Implementation of Security Groups:
     - Use security groups as a virtual firewall for EC2 instances to control inbound and outbound traffic.
     - Restrict inbound traffic from the internet to only essential services.
     - Limit outbound internet access to minimize exposure.
   - Best Practices:
     - Define security groups based on the least privilege principle.
     - Regularly review and update security group rules.

 2. Security Groups within Amazon VPC:
   - Inter-Service Communication:
     - Apply strict rules to control traffic between services within the VPC.
     - Ensure that services only have network access to what they need.
   - Micro-Segmentation:
     - Implement micro-segmentation to further isolate workloads and reduce the risk of lateral movement in case of a breach.

 3. Network Access Control Lists (ACLs):
   - Stateless Firewalls:
     - Use NACLs as a stateless firewall to filter inbound and outbound traffic at the subnet level.
   - Configuration Guidelines:
     - Set up NACLs to restrict traffic based on IP protocol, port number, and source/destination IP address.

 4. Other AWS Security Services:
   - AWS Shield for DDoS Protection:
     - Utilize AWS Shield for basic protection against DDoS attacks.
   - VPC Flow Logs:
     - Enable VPC Flow Logs to capture information about the IP traffic going to and from network interfaces in VPC.
   - AWS WAF:
     - Use AWS WAF to protect web applications from common web exploits.

---

 Implementation of Network Security in Stress Engineering Project

 Project Overview:
- Description of the AWS environment and services used by Stress Engineering.

 Security Groups Implementation:
- Configured security groups for each EC2 instance, allowing only necessary inbound and outbound traffic.
- Established distinct security groups for different layers (web, application, database) within the VPC.

 Internal Traffic Control:
- Implemented strict rules in security groups to manage communication between services within the VPC.
- Used micro-segmentation techniques to enhance workload isolation.

 NACL Configuration:
- Deployed NACLs to provide an additional layer of security, filtering traffic entering and exiting subnets.
- Customized NACLs to complement security group rules and offer granular control.

 Integration of Advanced AWS Security Services:
- Enabled AWS Shield for the entire AWS account for baseline DDoS protection.
- Activated VPC Flow Logs for monitoring and auditing network traffic patterns.
- Configured AWS WAF for critical web-facing services to protect against web-based threats.
"

------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
------------------------------------------------------------------------------------------------------
COST-001

"Develop total cost of ownership analysis or cost modelling
Determine solution costs using right sizing and right pricing for both technical and business justification.

Conducted TCO analysis or other form of cost modelling to provide the customer with an understanding of the ongoing costs including all the following 3 areas:

* Description of the inputs used to estimate the cost of the solution
* Summary of the estimates or cost model provided to the customer before implementation
* Business value analysis or value stream mapping of AWS solution

Please provide the following as evidence:

* Description of how to develop cost analysis or modeling with the critical components defined above
* Cost analysis example in one (1) of the submitted customer examples. Acceptable evidence types are: price calculator link, reports or presentations on business values analysis
"


------------------------------------------------------------------------------------------------------
In addition to the following answer to COST-001, please provide a concrete example of cost analysis for Stress Engineering

" Cost Analysis Example for Stress Engineering

 Project Overview:
* Description of the AWS solution provided to Stress Engineering.

 Input Description:
* AWS Resources: Utilized EC2 instances (m5.large), RDS (db.t3.medium), and S3 (100 GB).
* Usage Estimates: Estimated 700 EC2 instance hours per month, 500 GB of data storage in RDS, and 100 GB of data in S3.
* Pricing Models: Considered on-demand pricing for EC2 and RDS, with S3 standard storage pricing.

 Cost Estimate Summary:
* EC2 Costs: Estimated $XX per month for m5.large instances.
* RDS Costs: Estimated $XX per month for db.t3.medium instances.
* S3 Costs: Estimated $XX per month for 100 GB storage.
* Total Estimated Monthly Cost: $XXX

 Business Value Analysis:
* Operational Efficiency: The AWS solution automated many tasks, reducing manual effort and potential downtime.
* Cost Optimization: Identified potential for reserved instances for EC2 and RDS, estimating a XX% cost reduction over on-demand pricing.
* Revenue Impact: Improved performance and reliability of the AWS solution expected to enhance customer satisfaction and retention for Stress Engineering, potentially increasing their revenue.
"

------------------------------------------------------------------------------------------------------

Create a diagram of Classic 3-tier Web App Architecture with AWS Services for our client Stress Engineering.
Please show a highly available architecture that spans three Availability Zones, which
contain Auto Scaling Groups of EC2 instances to easily scale up as well as to protect the
application in case of failure/outage.

Create a diagram of Classic 3-tier Web App Architecture with AWS Services for our client Stress Engineering. Please show a highly available architecture that spans three Availability Zones, which contain Auto Scaling Groups of EC2 instances to easily scale up as well as to protect the
application in case of failure/outage.
