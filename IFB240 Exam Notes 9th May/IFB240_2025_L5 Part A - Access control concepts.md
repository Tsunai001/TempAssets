











IFB240 Cyber Security
   Lecture 5 - Part A Access Control Concepts

Dr Leonie Simpson lr.simpson@qut.edu.au

Introduction
• Managing information security involves assessing and treating risks, within an established context
- Try to minimize harm to information assets by countering threats, or reducing vulnerabilities
• Things we can do to reduce the risk of security incidents referred to as
- Controls
- Countermeasures
- Mitigations
- Safeguards,
- Security measures, ...
• Lots of different options to consider when choosing
controls ...


Can be categorised based on the approach taken
• McCumber model (NSTISSI 4011 Security Model) uses 3 categories
• Technology
- Hardware and software applied to protect assets
• Policy and practices
- Policies, procedures and guidelines defining how people can use information systems and assets
• Education, training and awareness
- So human users interacting with information assets understand the security implications of their actions, know what they need to do, and are trained appropriately



Can be categorised based on the role they play, with respect to potential security incidents
• Consider intended outcome if measure is applied
- Preventive controls
• Aim to prevent the security incident from occurring
- Detective controls
• Monitor to receive warning of attempts to exploit vulnerabilities, indicators of incident in progress or has occurred
- Corrective controls
• Aim to correct errors or irregularities that have been detected, repair damage

What is access control?
• Controlling or restricting the use of cyber/information assets and/or resources to
- Allow authorised users access to information resources
they need to perform their tasks
- Prevent authorised users from misusing resources, and
- Prevent unauthorised users gaining access to resources

• Resource examples include
- Hardware: processors, laptops, routers
- Software: application software, system software
- Information assets: data files, system documentation
- Services: computing, communications, power

Why is access control important?
• It's a fundamental aspect of information security,
because
- unauthorised access to resources, or
- authorised users misusing resources
could compromise the
- Confidentiality,
- Integrity, and/or
- Availability
of information assets. Consequences can be nasty :(

Why is access control important?
• Example: Hospital database breach (Mongo DB)
• https://pharmaphorum.com/news/health-records-publically-exposed/




• Example: Ex-employee gets destructive
• http://www.theregister.co.uk/2011/04/04/cyberlynk_zodiac_island/




• Example: Employee misuse
- ABC News, 15 Dec 2022
- Victorian Police officers misusing LEAP database
• Victoria Police allegedly use LEAP database to pursue, stalk, harass women prompting calls for inquiry - ABC News



• Example: Vehicles
- Smart keys & car crime
- The Guardian
- 25 February 2024
- Gone in 20 seconds: how 'smart keys' have fuelled a new wave of car crime | Motoring | The Guardian




• Some statistics on data breaches:
- From Verizon 2024 Data Breach Investigations Report
- https://www.verizon.com/business/resources/T74b/r eports/2024-dbir-data-breach-investigations- report.pdf


- Analyzed data from 30,458 real-world security incidents
• 10,626 were confirmed data breaches
• with victims spanning 94
countries

(From Verizon 2024 Data Breach Investigations Report)
https://www.verizon.com/business/resources/T74b/reports/2024-dbir-data-breach-investigations-report.pdf

• How have threat sources changed over

time?
• 
What is the threat
actor's motivation?




(From Verizon 2024 Data Breach Investigations Report)
https://www.verizon.com/business/resources/T74b/reports/2024-dbir-data-breach-investigations-report.pdf

• What types of threat actors are there?
- Organised crime
• commonly DoS and
Ransomware attacks
- End-user
• Mostly misdelivery and
miscellaneous errors
- State-sponsored
• Less common, but very
capable and resourceful



• For effective access control, need to consider
- What information assets/resources do you have?
• Where are they located?
• How sensitive/critical are these resources?
- Who/what should have access to each resource?
• What access permissions (authorisations) should they have?

- How will access control decisions be made?
• Discussed in Part B
- How will access control policy be implemented?
• Discussed in Part C


• What resources do you have?
- First step: identify all information assets, and understand risks to them
- Covered in AS/NZS 27002:2022 Clause 5 Organizational Controls
• Clause 5.9 Inventory of information and other associated assets
- Control: An inventory of information and other associated assets, including owners, should be developed and maintained
- Purpose: To identify the organization's information and other associated assets in order to preserve their information security and assign appropriate ownership
- Guidance:
" Inventory should be accurate, up-to-date, consistent and aligned with other inventories
" Asset location should be documented
" Each asset should be classified in accordance with the classification
of the information (see Clause 5.12 for more on classification)
" Asset owner has management responsibility for the asset over the whole asset lifecycle: from creation until deletion or disposal

Example: Information asset register

Basic access control concepts
• How sensitive are these resources?
- Assess the sensitivity of each resource
- Covered in AS/NZS 27002:2022 Clause 5.12 Classification of Information
• Control: Information should be classified according to the information security needs of the organization based on confidentiality, integrity, availability and interested party requirements
• Purpose: Ensures identification and understanding of protection needs
of information in accordance with its importance to the organization
• Guidance: Have a policy on information classification and
communicate it to all relevant parties
- Take into account:
" business needs for sharing or restricting information, for
protecting integrity and assuring availability
" legal requirements for confidentiality, integrity & availability
- Classification may vary over time - review and reclassify
" Value, sensitivity & criticality of info assets changes

Example: Information classification
• Qld Gov't Information security classification framework
• Information security classification framework (QGISCF) | For government | Queensland Government


Basic access control concepts
• How do users know which resources are sensitive/critical?
- Covered in AS/NZS 27002:2022 Clause 5.13 Labelling of information
• Control: Includes procedures for information labelling
particularly of sensitive or critical material
• Purpose: Facilitates communication of classification of information and supports automation of processing and management
• Guidance:
- Labels should reflect the classification scheme and be easily recognisable
- Consider format: physical and/or electronic
- Examples include: physical labels, headers and footers,
metadata, watermarks, ...


2025	IFB240	19

Example: Information classification
• Qld Gov't Information security classification framework
• Information security classification framework (QGISCF) | For government | Queensland Government
• Confidentiality classification labels for Qld Gov't information







• Who should have access to each resource?
- AS/NZS 27002:2022 Clause 5.15 Access Control
• Control: Rules to control physical and logical access to information and other associated assets should be established and implemented based on business and info sec requirements
• Purpose: To ensure authorized access and prevent unauthorized access to information and other associated assets
• Guidance:
- Owners of information assets should determine information security
and business requirements related to access control
- Consider (list of 11 items, here are some - linked to other clauses)
" Which entities require which type of access to information and other assets
" Security of applications
" Physical access and entry controls, ...


• Who should have access to each resource?
- Access control decisions for
• each user, or group of users, and
• each resource
should be stated as a policy, consistent with org.
- Authorised users should
• Have access to resources necessary for their tasks, but
• Be unable to perform other actions
- Unauthorised users should not have access


• Who should have access to each resource?
• Common principles for access control policies
- Blacklists
• Access generally permitted unless expressly forbidden
- If your name is on the list, you will be denied access
- These are the sites that you are not permitted to visit
- This software must not be installed
- Whitelists
• Access generally forbidden unless expressly permitted
- If your name is on the list, you will be granted access
- These are the only sites that you are permitted to visit
- These are the only applications that you are permitted to install


• Common principles for access control policies
- Principle of least privilege
• Access is restricted to the minimum resources and authorisations
required for an entity to perform their day-to-day function
• Intended to limit level of damage if a security incident occurs
- Where the resource is information, this may be known as need-to-know principle
• Subject given access to the least amount of information they need to know to perform their role or task
• Examples:
- Lecturer accessing student information files
" Should have access to academic transcript (mode of access?)
" Shouldn't access personal details: address, financial info, etc

• Common principles for access control policies
- Separation of duties (privileges) (segregation of duties)
- AS/NZS 27002:2022 Clause 5.3 Segregation of duties
• Control: Conflicting duties/conflicting areas of responsibility segregated
• Purpose: To reduce the risk of fraud, error, and bypassing of
information security controls
• Guidance: Separate conflicting duties between different individuals to prevent one individual from executing potential conflicting duties on their own
- Identify critical tasks, and divide each task up into a series of steps
- Ensure that the steps are performed by different entities
- Examples:
• Financial transactions - require:
- data entry to be performed by one person, and
- authorisation by another, before task completes
• Academic change of grade - require:
- request prepared by Unit Coordinator
- change authorised by Head of School, then
- data entry in grades system changed by administration officer



• Breach example: false invoicing
- 19
- ABC news report
• Former WA pub		 Paul Whyte sent			 years in jail for s	 taxpayer millio				



• What access permissions (authorisations) should subjects have?
- What modes of access are permitted?
• If you have permission to access a resource, what are you allowed to do?
- Example: possible access permissions for data resources
include
• read - observe
• write - observe and alter
• execute - neither observe nor alter
• append - alter
• search
• create
• delete

Summary
• Access control is important for information security
• Need to know:
- what your information assets are, and
- where they are located
- how sensitive/critical they are
- who needs access to each resource, and what mode of access
• Need to consider how to:
- Make access control policy decisions (discuss in Part B)
- Implement access control decisions	(discuss in Part C)


























































