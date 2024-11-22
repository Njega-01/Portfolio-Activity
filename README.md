# CONTROL AND COMPLIANCE CHECKLIST

## Objective
The Botium Toys Security Audit project aimed to evaluate and improve the organization's security posture by identifying existing vulnerabilities, assessing compliance with industry standards, and implementing necessary controls. This initiative focused on enhancing the protection of assets, employee equipment, customer data, and systems while adhering to regulatory requirements such as PCI DSS, GDPR, and SOC standards

### Skills Learned
- Conducting comprehensive risk assessments.
- Developing and reviewing compliance checklists for regulatory frameworks.
- Identifying and prioritizing vulnerabilities in an organization's security infrastructure.
- Recommending practical solutions to enhance security and minimize risks.
- Understanding the application of NIST CSF principles, including asset identification and impact analysis

### Tools Used
- Compliance frameworks: PCI DSS, GDPR, SOC.
- Security risk assessment methodologies.
- Asset management and classification techniques.
- Documentation tools for policy drafting and control assessment.

## Steps
#### Ref 1: Scope and Goals
Defined the audit's scope to include all assets, internal systems, and compliance practices at Botium Toys.
Established goals to identify vulnerabilities, assess controls, and improve compliance with industry standards.

![image](https://github.com/user-attachments/assets/d5545a84-3581-48eb-ad1f-990c0eca6dc4)

#### Ref 2: Current Asset Review
Reviewed on-premises equipment, employee devices, and legacy systems.
Documented systems and services including accounting, telecommunication, and ecommerce platforms.
Assessed the physical and digital infrastructure such as fire detection systems and internet access.

![image](https://github.com/user-attachments/assets/c9a926f6-733d-405c-bd33-d1afe59d65b4)

#### Ref 3: Risk Assessment
Determined a risk score of 8, highlighting the need for urgent remediation.
Analyzed existing vulnerabilities, such as lack of encryption, absence of an intrusion detection system, and insufficient disaster recovery plans.

![image](https://github.com/user-attachments/assets/cb5fb673-73c0-4f76-bc1d-c8289c4cfd14)

#### Ref 4: Controls Assessment Checklist
Evaluated the presence of controls like antivirus software, firewalls, and CCTV surveillance.
Noted the absence of critical controls such as least privilege, encryption, and a centralized password management system.

![image](https://github.com/user-attachments/assets/54e9d96e-fca2-4c91-b789-ad1120a1d7aa)

#### Ref 5: Compliance Checklist
Assessed adherence to PCI DSS, GDPR, and SOC standards.
Highlighted gaps such as unsecured credit card data and incomplete user access policies.

![image](https://github.com/user-attachments/assets/44e0f86b-411a-4a74-9030-4e5ba9b70762)

#### Ref 6: Recommendations
Suggested implementing an intrusion detection system and enforcing least privilege to mitigate unauthorized access.
Proposed stricter password policies and centralized password management to enhance security.
Recommended encrypting sensitive customer data to comply with PCI DSS and reduce risks of fines.

![image](https://github.com/user-attachments/assets/41cfcf37-a703-4a1d-a52b-7b375392192b)


# INCIDENT REPORT ANALYSIS

## Objective
The objective of this project was to apply the NIST Cybersecurity Framework (CSF) to a Distributed Denial of Service (DDoS) attack scenario. The framework’s five core functions—Identify, Protect, Detect, Respond, and Recover—were implemented to manage the incident, mitigate risks, and restore critical services. The exercise was focused on securing the network, improving monitoring, and ensuring quick recovery to maintain business continuity.

### Skills Learned
-Practical application of the NIST CSF to real-world cybersecurity incidents.

- Identifying and analyzing DDoS attack vectors, specifically ICMP floods.
- Configuring firewalls and Intrusion Prevention Systems (IPS) to mitigate attacks.
- Designing and implementing response and recovery procedures in a security incident.
- Enhancing network monitoring tools to detect and block malicious traffic.

### Tools Used
- Firewall configuration tools to limit incoming ICMP packets.
- Intrusion Prevention System (IPS) / Intrusion Detection System (IDS) for traffic filtering.
- Network monitoring software to detect abnormal traffic patterns.
- ICMP Ping tool to confirm the attack and diagnose the network issues

## Steps
#### Ref 1: Incident Identification
The security team noticed slowed network traffic and difficulties establishing a TCP connection.
Upon using the ICMP Ping tool, it was confirmed that the server was overwhelmed by a high volume of ICMP packets from multiple IP addresses, indicating a Distributed Denial of Service (DDoS) attack.

![image](https://github.com/user-attachments/assets/9ec2d9b0-de51-4904-bb1f-58c615a1927c)

#### Ref 2: Protect
A new firewall rule was implemented to limit incoming ICMP traffic and filter out potentially malicious packets.
The security team installed network software to detect abnormal traffic patterns that could indicate further DDoS attempts.

![image](https://github.com/user-attachments/assets/08d1753d-ebd5-4435-bff2-f11f4f915c75)


#### Ref 3: Detect
Source IP address verification was added to the firewall to prevent incoming ICMP packets from spoofed addresses.
An IPS/IDS system was configured to filter suspicious traffic and detect anomalous behavior in real-time.

![image](https://github.com/user-attachments/assets/40f4857e-2258-4ae5-a2a6-788427f125fa)
![image](https://github.com/user-attachments/assets/c00ee436-8629-423e-8bc1-8f09fd8b40c2)

#### Ref 4: Respond
The incident response team immediately blocked all incoming ICMP packets to halt the attack.
Non-critical network services were taken offline to isolate the impact and prevent further disruptions.

![image](https://github.com/user-attachments/assets/794c88af-bd92-48df-9ec0-0b7836961633)

#### Ref 5: Recover
Redundant systems were activated to restore critical services quickly.
Security audits were performed to confirm the integrity of the systems and prevent future attacks.
Internal communications were made following the company’s breach notification protocol.

![image](https://github.com/user-attachments/assets/fe73ce84-7112-40d4-afde-ddc044413fa5)

# FILE PERMISSIONS IN LINUX

## Objective
The objective of this project was to assess and adjust file and directory permissions on a Linux-based system to ensure they align with organizational policies. The permissions for files and directories, including hidden ones, were reviewed and modified using the chmod and ls -la commands to control access and ensure compliance with security requirements.

### Skills Learned
- Proficiency in managing file and directory permissions in Linux using chmod and ls -la.
- Understanding of the Linux file permission string format and how to interpret it.
- Experience in applying security policies by restricting access based on user roles.
- Familiarity with controlling access to hidden files and directories.

### Tools Used
- chmod: A command used to modify file and directory permissions.
- ls -la: A command used to list all files and directories, including hidden ones, and view their permissions.

## Steps
#### Ref 1: Linux Permissions String
![image](https://github.com/user-attachments/assets/65b0789f-167e-4803-b09e-a3fab0b130db)

drwxr-xr-x: A typical permission string for a directory, showing access for the user (read, write, execute), group (read, execute), and others (read, execute).
The d at the beginning indicates it's a directory. The following characters represent the permissions for the User (read, write, execute), Group (read, execute), and Others (read, execute).

#### Ref 2: Changing Permissions
![image](https://github.com/user-attachments/assets/cd2ed3f8-e865-4b17-8599-741558ff4e57)

Command: chmod o-w project_k.txt
This command removes write access for others on the file project_k.txt, in compliance with the organization’s policies.

#### Ref 3: Changing Permissions for Hidden Files
![image](https://github.com/user-attachments/assets/cdb22b93-81f9-4b28-86f2-2517a06859a0)

Command: chmod u-w,g-w+r .project_x.txt
The user and group are allowed to read the hidden file .project_x.txt, but write access is denied for both.
#### Ref 4: Changing Directory Permissions
![image](https://github.com/user-attachments/assets/51cd1b8c-9ca7-4cb6-bb13-697a910cc546)

Command: chmod g-x drafts
This removes execute access for the group research_team from the drafts directory, restricting access solely to researcher2.

# APPLYING FILTERS TO SQL QUERIES

## Objective
The project focused on investigating security issues related to login attempts and employee devices using SQL. The aim was to query data stored in MariaDB from two main tables: Log_in_attempts and Employees. This involved applying filters to retrieve specific login events and employee details, assisting in identifying potential security risks, such as failed login attempts after hours and suspicious login locations.

### Skills Learned
- Mastery of SQL queries for filtering data based on specific conditions.
- Proficient in using logical operators like AND, OR, and NOT for complex data extraction.
- Expertise in applying date and time filters to identify unusual login activities.
- Knowledge of using the LIKE operator with wildcards for partial string matching.
- Experience in analyzing data from multiple tables using SQL joins and subqueries.

### Tools Used
- MariaDB shell for managing and querying data.

## Steps
#### Ref 1: Retrieve after hours failed login attempts
To filter for failed login attempts that occurred after business hours, a SQL query was written to check the log_in_attempts table for events with a login_time > '18:00' and success = FALSE. This helped identify any suspicious activity that occurred after the workday ended.

![image](https://github.com/user-attachments/assets/6749e005-1dc4-4216-8527-97cdcfce8731)
![image](https://github.com/user-attachments/assets/80421b19-3657-436e-bf85-e8e740e1b8c2)

#### Ref 2: Retrieve login attempts on specific dates
A suspicious event on 2022-05-09 required a query to retrieve all login attempts on that date and the day before (2022-05-08). The WHERE clause used the OR operator to filter for both dates.

![image](https://github.com/user-attachments/assets/0d2e9f6a-977e-44b5-a7e6-0a5551a9bc91)
![image](https://github.com/user-attachments/assets/9a0c42ca-8627-40d5-bb46-bf8f9bae0485)

#### Ref 3: Retrieve login attempts outside of Mexico
After identifying login attempts that occurred outside of Mexico, a query was created to filter the log_in_attempts table for any records with a country not equal to Mexico. The LIKE operator was used with a wildcard to match various representations of Mexico (e.g., MEX, MEXICO).

![image](https://github.com/user-attachments/assets/015ad8f7-501a-4e99-98d8-35ab10096260)
![image](https://github.com/user-attachments/assets/b0f28d73-5d7f-4755-973b-deb6146ec08b)

#### Ref 4: Retrieve employees in Marketing
The task was to retrieve all employee devices located in the Marketing department within the East building. The query used LIKE with a wildcard to filter the office column for entries starting with 'East'.

![image](https://github.com/user-attachments/assets/25542227-2806-4604-9004-8059610f34f3)
![image](https://github.com/user-attachments/assets/80f4d7b8-05b5-4786-8237-3ccbf302e922)

#### Ref 5: Retrieve employees in Finance or Sales
To get a list of employee devices in the Finance or Sales departments, an SQL query used the OR operator to filter the employees table for employees in either department.

![image](https://github.com/user-attachments/assets/915ad111-fb14-4d27-976d-dae7d788646a)
![image](https://github.com/user-attachments/assets/350a4566-8e2d-4b2d-bc7d-34c7dae57519)

#### Ref 6: Retrieve all employees not in IT
A final query was used to retrieve all employees not belonging to the IT department. The NOT operator was applied to filter out those in the IT department.

![image](https://github.com/user-attachments/assets/e410c403-2631-43ef-8030-1d6fdee7cb53)
![image](https://github.com/user-attachments/assets/4707c482-3fc1-4dde-a337-b7c2fb34a425)

# VULNERABILITY ASSESSMENT REPORT

## Objective
The objective of this project was to assess the risks associated with a publicly accessible database server using the guidelines outlined in NIST SP 800-30 Rev. 1. This included identifying potential threats, categorizing vulnerabilities, and evaluating the likelihood and severity of threat events. The risk assessment helped in understanding the possible impacts on business operations, allowing for the development of a comprehensive remediation strategy to secure the database system and protect sensitive data.

### Skills Learned
- Comprehensive understanding of risk assessment techniques and frameworks.
- Ability to categorize and assess threat sources and events.
- Proficiency in calculating the likelihood and severity of risks.
- Application of NIST SP 800-30 Rev. 1 in risk analysis to improve security posture.
- Development of remediation strategies based on risk assessment findings.

### Tools Used
- NIST SP 800-30 Rev. 1 for risk assessment guidelines.
- Database management systems (MySQL) for practical evaluation of the risks.
- Linux operating system and server configurations for assessing vulnerability points.

## Steps
#### Ref 1: Threat Source Identification
I identified potential internal and external threat sources that could exploit vulnerabilities in the database system. This included competitors, disgruntled employees, and external threat actors.
#### Ref 2: Threat Event Categorization
I categorized potential threat events such as data exfiltration, reconnaissance, and unauthorized data alteration that could affect the database and its operations.
Likelihood and Severity Scoring: Using a combination of expert judgment, historical data, and the NIST guidelines, I calculated the likelihood and severity of various threat events.
#### Ref 3: Risk Calculation 
I applied the formula of likelihood x severity to calculate the risk associated with each potential threat event. This helped prioritize threats based on their impact and likelihood.
#### Ref 4: Remediation Strategy
Based on the risk analysis, I formulated a comprehensive remediation strategy, focusing on securing the database through stronger authentication mechanisms, data encryption, and access controls.

![image](https://github.com/user-attachments/assets/eefce431-1855-4b8d-af2e-e3afd4feff69)

# INCIDENT HANDLER'S JOURNAL

## Objective
As an Incident Handler, my goal is to efficiently detect, analyze, respond to, and recover from cybersecurity incidents. I aim to strengthen the organization’s defenses against emerging threats, ensure business continuity, and protect sensitive data from malicious actors. Through continuous learning and hands-on experience with a variety of cybersecurity tools, I work to improve the organization's incident response capabilities and overall security posture.

### Skills Learned
- Incident Detection and Response
- Threat Analysis
- Network Traffic Analysis
- Use of Security Tools
- Incident Escalation
- Report Creation and Review 

### Tools Used
- VirusTotal
- Splunk
- Chronicle 
- Company’s Playbook
- Company’s Report

## Steps
[Incident handler's journal .docx](https://github.com/user-attachments/files/17862150/Incident.handler.s.journal.docx)


# ALGORITHM FOR FILE UPDATES IN PYTHON

## Objective
The objective of this project was to automate the process of updating an "allow_list.txt" file, which controls access to restricted content based on a list of authorized IP addresses. The algorithm removes IP addresses specified in a separate "remove_list" from the allow list, ensuring that only approved addresses maintain access.

### Skills Learned
- File manipulation in Python using the open(), read(), and write() functions.
- Converting file contents from a string to a list and performing operations like .remove().
- Automating the process of file updates based on dynamic input (the remove list).
- Iterating through lists and performing conditional checks efficiently.
- Using Python’s string methods (.split() and .join()) to process file data.

### Tools Used
- Python (for algorithm implementation)

## Steps
#### Ref 1: Open the allow list file
Using the open() function in read mode, the algorithm accesses the "allow_list.txt" file to retrieve the list of IP addresses.

![image](https://github.com/user-attachments/assets/4dbd9159-9563-4231-9d12-3c415dd52bab)

![image](https://github.com/user-attachments/assets/59c47f66-0167-46c4-89d2-faf7eca92e42)

#### Ref 2: Read the file contents
The file contents are read as a string using the .read() method, containing all the IP addresses in the allow list.

![image](https://github.com/user-attachments/assets/200772c5-60c0-430a-a1ba-2eb95b70c779)

#### Ref 3: Convert the string to a list
The string containing IP addresses is converted into a list using the .split() method, which separates the string based on whitespace.

![image](https://github.com/user-attachments/assets/f35c42ff-4d0e-4d9a-8cb3-cc0e6651893a)

#### Ref 4: Iterate through the remove list
A for loop iterates through each IP address in the "remove_list" to check if it exists in the allow list.

![image](https://github.com/user-attachments/assets/417ac8e9-3ef5-4b20-96f4-f2cca4938909)

#### Ref 5: Remove IP addresses from the allow list
The algorithm checks if each IP address from the remove list exists in the allow list and uses .remove() to delete it.

![image](https://github.com/user-attachments/assets/490bd0aa-81db-4145-bc51-e4cc2dd35295)

#### Ref 6: Update the file with the modified list
After removing the necessary IP addresses, the list is converted back into a string, and the updated list is written back to "allow_list.txt" using the .write() method.

![image](https://github.com/user-attachments/assets/daf71907-d0a8-4725-b404-f20d042e76ce)
![image](https://github.com/user-attachments/assets/d2091031-900b-43b1-aab7-062358517ad4)
