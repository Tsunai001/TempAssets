IFB240 Cyber Security
Lecture 3 – Part B
InfoSec Standards & AS/NZS 27001:2023
Information Security Management Systems
Dr Leonie Simpson
lr.simpson@qut.edu.au

How do you manage information security?
• Info sec management involves asking questions like
– What needs to be protected?
• What are your information assets? Where are they? What are they worth?

– Why do these assets need to be protected?
• What could go wrong? How could the asset be damaged? (Threats & Vuln.)

– How can these assets be protected?
• What resources are needed to do this, and how much does that cost?
• How urgently is this required?

– What happens if these assets are not protected?
• And what could that cost?

– You don’t have unlimited resources, so
making tradeoffs is necessary:
• Can’t afford to protect all assets against all possible threats
• Some level of risk involved – basically, a risk management exercise
2025

IFB240

2

How do you manage information security?
• Where do I find (best) guidance on what to do?
– Two widely used risk-based frameworks to guide this
• ISO27K series
– Jointly published by International Standards Organisation (ISO) and
International Electrotechnical Commission (IEC) as ISO/IEC 27k family
– Australian Standards (AS/NZS 27K) are based on these

• NIST CSF
– (United States) National Institute of Standards and Technology (NIST)
Cyber Security Framework (CSF)

– Also some industry specific information security standards, such as the
Payment Card Industry Data Security Standard (PCI DSS)
• Information security related to credit card payments processing for orgs
that handle credit cards from major companies (Visa, Mastercard, etc)
• Compliance-based standard
2025

IFB240

3

Info security management standards
• Info Sec Management Standards: Australian
– AS/NZS 27001:2023 Information security, cybersecurity and privacy
protection – Information security management systems - Requirements
– AS/NZS 27002:2022 Information security, cybersecurity and privacy
protection – Information security controls
– AS/NZS 27005:2024 Information security, cybersecurity and privacy
protection – Guidance on managing information security risks (Discussed
in Part A)

• Info Sec Management Standards: International
– ISO/IEC 27001:2022 Information security, cybersecurity and privacy
protection – Information security management systems - Requirements
– ISO/IEC 27002:2022 Information security, cybersecurity and privacy
protection – Information security controls
– ISO/IEC 27005:2022 Information security, cybersecurity and privacy
protection – Guidance on managing information security risks
2025

IFB240

4

ISO27K series
• ISO/IEC 27000
– defines terminology used, and
– gives an overview of relationships between the various Information
Security Management Standards illustrated in this diagram (ISO27000, p19)
– Check overview to see which standards are Requirements, which are
guidance

2025

IFB240

5

Info security management standards
• USA: NIST

– National Institute for Standards & Technology
• An organisation in U.S. Dept of Commerce

• NIST Cybersecurity Framework (CSF)

– Evolved from a cyber security framework designed for use in
critical infrastructure cyber security
– Now useful for organisations of all sizes across all industry sectors

• Similar to the ISO27K series

• Risk-based
• Intended to help organisations understand, manage, and reduce
their cybersecurity risk and protect their networks and data

• Different structure than the ISO27K series

• Divided into five function areas: Identify, Protect, Detect,
Respond, and Recover

2025

IFB240

6

Info security management standards
• Now NIST Cybersecurity Framework (CSF) 2.0
•

2025

[image obtained from https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1299.pdf ]

IFB240

7

Info security management standards
• NIST CSF 2.0 introduced Govern function
– Objective:
• The organization’s cybersecurity risk management strategy,
expectations, and policy are established, communicated, and
monitored

– Includes:
• Understanding and assessing org cyber security needs
• Developing a cyber security risk strategy tailored to the
organisation
• Establishing defined risk management practices
• Developing and communicating organizational cyber security
practices
• Establishing and monitoring cyber security supply chain risk
• Implementing continuous oversight
2025

IFB240

8

Info security management standards
• NIST also have (lots of ) Special Publications

– Guidelines, recommendations, technical specifications, etc

– In the 800 series (Computer Security)
• including

– SP800-12: An Introduction to Computer Security: The NIST Handbook
– SP800-18: Guide for Developing Security Plans for Federal
Information Systems
– SP800-37 Rev.2: Risk Management Framework for Information
Systems and Organizations: A System Lifecycle Approach for Security
and Privacy
– SP800-121 Rev.2: Guide to Bluetooth Security
– SP800-210: General Access control Guidance for Cloud Systems

– In the 1800 series (Cybersecurity practice guides)
• including

– SP1800-4: Mobile Device Security: Cloud and Hybrid Builds
– SP1800-11: Data Integrity: Recovering from Ransomware and Other
Destructive Events

2025

IFB240

9

Info security management standards
• Applying Cyber/Info Sec Management Standards in an
organisation provides
–
–
–
–

Evidence of management commitment to information security
Assurance to other organizations about information security practices
Assurance to staff that appropriate practices are in place
A checklist of important aspects of information security

• If you know

– which standard an organization is applying, or
– which framework their approach is based on,

then you have an idea of their info sec management practices

• Who uses these standards?

– According to 2015 Aust. Cyber Security Survey – Major Australian
Businesses, (available from https://www.cert.gov.au/newsroom)
• 82% of organisations apply external IT security standards
• Of these, 85% followed ISO 27001

• In IFB240 we will focus on AS27K series
2025

IFB240

10

Info security management standards
• How will you know if organisations are managing
security?
– May have a certified Info Sec Management System (ISMS)
• Certified against AS/ISO 27001
– Only info sec standard in AS 2700x series possible to obtain
certification for
• May apply this standard without obtaining certification

– Number of organisations with ISMS certified against
27001: (Data from ISO 2022, 2020, 2018 Surveys, available at:
https://www.iso.org/the-iso-survey.html

• 2022: 71,549 certificates worldwide - Australia 717
• 2020: 44,499 certificates worldwide - Australia 562
• 2018: 31,910 certificates worldwide - Australia 264
2025

IFB240

11

AS/NZS 27001:2023
What is it?
• A comprehensive approach to info security management
• Scope of AS/NZS 27001:2023
– Specify requirements for establishing, implementing, maintaining and
continually improving an ISMS within the context of an organisation
– Includes requirements for assessment and treatment of info security
risks
– Requirements are generic – apply to all organisations regardless of
type, size or nature
– Can be used by internal and external parties to assess organisational
info sec management (can audit to see if organisation complies with 27001)
• Use in conjunction with AS/NZS 27002:2022 (Discussed in Part C)
– AS 27001 is about management
• How an organisation can set up and run an info sec management system

– AS 27002 is a code of practice
• Provides a set of information security goals and controls
• Organisations select controls relevant to their info sec risk environment
2025

IFB240

12

Structure of AS/NZS 27001:2023
• AS/NZS 27001:2023 contains:
– 10 Clauses:
1.
2.
3.
4.
5.
6.
7.
8.
9.
10.

Scope
Normative references
Terms and definitions (from ISO27000)
Context of the organization
Leadership
Planning
Support
Operation
Performance evaluation
Improvement

– Can’t claim to conform with 27001 if any requirements in
clauses 4-10 are excluded
2025

IFB240

13

AS/NZS 27001:2023
• Clause 4: Context of the organization
– 4.1 Understanding the organization and its
context
• Determine external and internal issues relevant to purpose …

– 4.2 Understanding needs & expectations of
interested parties
• Determine interested parties and their requirements,
• May include legal and regulatory requirements, contractual
obligations

– 4.3 Determining the scope of the ISMS
• Boundaries and applicability of the ISMS – document this

– 4.4 Information Security Management System
• Establish, implement, maintain and continually improve ISMS
2025

IFB240

14

AS/NZS 27001:2023
• Clause 5: Leadership

– 5.1 Leadership and commitment
• Management to demonstrate by

– Ensuring info security policy and objectives are established
– Ensuring integration of ISMS requirements into organization’s
processes
– Ensuring that resources needed for the ISMS are available, …

– 5.2 Policy

• Management to establish info sec policy that is

– Appropriate to the purpose of the organisation
– Includes information security objectives, …
– Documented, communicated within org, and available

– 5.3 Organizational roles, responsibilities and authorities
• Management to

– Ensure responsibilities and authority for roles assigned and
communicated
– Assign responsibility for ensuring ISMS conforms to requirements of
this standard

2025

IFB240

15

AS/NZS 27001:2023
• Clause 6: Planning
– 6.1 Actions to address risks and opportunities
• Organization should determine risks and opportunities that need
to be addressed
• Define and apply
– risk assessment process (and retain relevant documentation)
– risk treatment process (and retain relevant documentation)

– 6.2 Info security objectives and planning to achieve them
• Objectives should be
– Consistent with info sec policy, measurable, monitored,
communicated, updated, documented, …
– Organization should determine
» What will be done
» What resources are required
» Who is responsible,
» When it will be done, …
2025

IFB240

16

AS/NZS 27001:2023
• Clause 7: Support
– 7.1 Resources

• Determine and provide resources needed to establish,
implement, maintain and improve the ISMS

– 7.2 Competence

• Ensure competence of persons doing work that affects info sec
– Based on training, education and experience
• Take actions to acquire competence
• Retain documented evidence of competence

– 7.3 Awareness

• People need awareness of info sec policy, their contribution to
effectiveness of ISMS and implications of not conforming

– 7.4 Communication

• Internal and external, relevant to the ISMS

– what, when, who to, who from and processes used

– 7.5 Documented information
2025

IFB240

17

AS/NZS 27001:2023
• Clause 8: Operation
– 8.1 Operational planning and control
• Plan, implement and control the processes needed to meet
requirements and implement the actions determined in Clause 6
by
– Establishing criteria for the processes
– Implementing control of processes in accordance with criteria
• Document to provide confidence that processes carried out as
planned

– 8.2 Information security risk assessment
• Perform risk assessments at planned intervals, or when significant
changes are proposed or occur, and document these

– 8.3 Information security risk treatment
• Implement the plan and document the results
2025

IFB240

18

AS/NZS 27001:2023
• Clause 9: Performance evaluation
– 9.1 Monitoring, measurement, analysis and evaluation
•
•
•
•

What needs to be monitored?
How it will be measured, analyzed and evaluated?
When will it be done? Who will do these tasks?
Who will analyse and evaluate the results?

– 9.2 Internal audit
• Conduct at planned intervals to provide information on
– Conformance (to organizations requirements and to AS27001), and
– Effectiveness of implementation and maintenance

• Who will audit? – objectivity and impartiality
• Document and report audit results to management

– 9.3 Management review
• Review ISMS periodically to ensure continuing suitability,
adequacy and effectiveness
2025

IFB240

19

AS/NZS 27001:2023
• Clause 10: Improvement
– 10.1 Continual improvement
• Organization should continuously improve the suitability,
adequacy and effectiveness of the ISMS

– 10.2 Nonconformity and corrective action
• When nonconformity is identified, organization should
– React – control and correct, and deal with the consequences
– Evaluate the need for action, so that nonconformity does not
recur or occur elsewhere
– Implement any action needed
– Review the effectiveness of corrective action and
– Make changes to the ISMS if needed
• Document the nonconformities and actions taken, and results of
corrective action
2025

IFB240

20

Who is responsible for info/cyber
security?
• In an organisation - consider these groups
– Management
• CEO, CSO, CISO

–
–
–
–

General security staff
IT staff
Users
Third parties
• Outsourced information security management
• Customers, suppliers, business partners

• What actions can they take to enable/hamper info sec?
• Actions of one entity have consequences for others
• Need co-operation and collaboration at all levels, across and
between organisations
2025

IFB240

21

Who is responsible for info security?
And what are the consequences for failing to manage …

2025

IFB240

22

Who is responsible for info security?
And what are the consequences for failing to manage …

2025

IFB240

23

Summary
• Cyber/Info sec management is an exercise in controlling risk
• Standards provide guidelines on best practice
– In IFB240 we will focus on AS27K series
• Based on ISO27K series - mostly this is risk-based
• In L3 Part B we discussed AS/NZS 27001:2023 Information Security
Management Systems
– Useful for organizations
– Compliance with this standard requires implement all clauses
– Be aware there are
• Other frameworks (For example NIST CSF)
• Other standards (For example PCI DSS)

• When interacting with other organizations, useful to know
what their cyber/info sec management approach is
– Risk management relies on having an informed view of the situation so
appropriate decisions are made
2025

IFB240

24

