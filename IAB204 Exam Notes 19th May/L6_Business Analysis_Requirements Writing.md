Requirements Writing
Approaches and Models
Dr Rehan Syed

School of Information Systems
Faculty of Science
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

1

ACKNOWLEDGEMENT OF TRADITIONAL OWNERS
QUT acknowledges the Turrbal and Yugara, as the First Nations owners
of the lands where QUT now stands. We pay respect to their Elders,
lores, customs and creation spirits. We recognise that these lands have
always been places of teaching, research and learning. ​
QUT acknowledges the important role Aboriginal and Torres Strait
Islander people play within the QUT community.​

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

2

Business
Requirements

Levels of Requirements
Stakeholder
Requirements

Goals and
Objectives

Text, Tables, Models, Use Cases…

Solution
Requirements

Functional
Requirements

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

Business
Rules

Issues, Constraints, Risk…

Non-Functional
Requirements

Requirement Specifications
3

Levels of Requirements—Interdependencies
Business Requirements
(Why a project is required?)
•
•
•
•
•
•

Cost reduction
Market opportunity
Developing new capability
New business model
A regulatory requirements
…

Support

Stakeholder Requirements

Achieved by

•
•
•
•
•
•

Perform something
Create something
Update something
Approve something
Audit/Control something
…
Supp
ort

Implemented by

(as a <> I want to <> so that)

Functional Requirements
(a solution must include?)
•
•
•
•
•
•
•

Produce,
Delete,
Update,
Transform,
Communicate,
Block,
…

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Direct/Constrain

Business Rules
(Policies, Org.
Constraints)
•
•
•

Approvals &
Authorisations
Methods
…

Non-Functional Requirements
(Operating Condition for a solution)
•
•
•
•
•
•

Performance,
Infrastructure,
Quality features,
Safety,
Legal
…

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

Must comply with

4

Requirement Modelling Techniques
Conceptual Data
Model
Data Dictionary
Logical Data Model
Functional
Requirements
Specifications
OR
Class Diagrams

User Profiles
OR
User Persona

User Stories
OR
Use Case Descriptions

Non-Functional
Requirements
Specifications

Storyboards
Wireframes
Low-Fi /Hi-Fi
Prototypes

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

5

Requirement Writing Guidelines

Express
exactly 1
requirement at
a time

Avoid
complex
conditional
clauses (e.g.,
nested ifs)

Do not
assume
reader has
domain
knowledge

Use
consistent
terminology

Use
terminology
familiar to the
stakeholders

Clearly
describe who
is responsible
for fulfilling the
requirement

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

6

Requirement Writing Guidelines—Common Issues
Missing or incorrect requirements
Inclusion of non-essential requirements
Vague or incomplete requirements
Avoid vague words: minimise, maximise, optimise, rapid, user-friendly, easy, simple, often,
normal, usual, large, intuitive, robust, state-of-the-art, improved, efficient, and flexible.

Never use: "and/or" or "etc."
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

7

User Stories
• A brief, textual description of functionality that users need from a solution
• Usually 1-2 sentences that includes:
– WHO (Actor): stakeholder who benefits
– WHAT (Description): high-level overview of what’s required by the actor
– WHY (Benefit): the business value delivered
– Recommended Format
– As an <ACTOR>, I want to be able to <FUNCTION>, so that I can <Business:
Goal/Need/Benefit>

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

8

User Story Examples
Finding pay slips is really difficult, and it takes a long
time to request for past records. And it gets worse
during the EOFY because the accountants will have
to extract at least 5 years of pay records.
Currently, I waste too much time searching for
citizens’ tax records. Searching by names and
surnames is very inefficient and results in incorrect
records.

Employee

ATO Officer

I have a serious problem related to stock
management–over and under stock is a common
occurrence. We estimate the required inventory based
Procurement
on our judgements. Incorrect orders and quantities are Manager
sent to our suppliers, leading to unnecessary costs.
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Stories Systems, Faculty of Science
Dr Rehan Syed. School ofUser
Information

“As an employee, I want to
download my pay slips for
User Story 1
the previous 5 years to help
me do my taxes”
“As an ATO Officer, I want
to search for a client using
User Story 2
their TFN to shorten service
times”
“As a procurement
manager, I want to
generate
User Story
real-time
3
inventory reports to reduce
inventory cost”
9

EPIC

From User Stories to Task
“As a procurement manager, I
want to generate real-time
inventory reports to reduce
inventory cost”

User
Story

BA

Tasks

User
Story

Tasks

Sub-Tasks

Design
User
Interface

Design
Database
Schema

Code for
Inventory
Report

Develop
Test
Criteria

Sub-Tasks
Sub-Tasks

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

10

Developers

Characteristics of Requirement Quality
Cohesive – defines a single aspect of the desired business process or system.
Complete – individual requirement is not missing necessary or relevant information. Set represents
all relevant requirements
Consistent – not contradictory, uses similar terms and wording, level of detail
Unambiguous – must be written objectively; only one interpretation
Correct – will lead to a valid solution
Feasible – within technical architecture, budget, time, resources
Modifiable – logically structured so that requirements can be re-arranged easily (*not changed)
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Testable – must be able to prove that the requirement has been fulfilled

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

11

Requirement Writing Terminologies

Keywords

Denotes

Alternatives

• Shall

• Absolute Requirement

• MUST, REQUIRED

• Shall Not

• Absolute Prohibition

• MUST NOT

• Should

• Can be ignored in certain
circumstances
• Can be included in certain
circumstances
• Optional requirement

• RECOMMENDED

• Should Not
• May

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

• NOT RECOMMENDED
• OPTIONAL
12

Requirement Writing-Examples & Tips
The dashboard shall illuminate a warning light when engine temperature exceeds 80oC
• The system shall produce a ‘profit and loss’ statement every three
months
• Each account code shall be validated against the charter of accounts before an order can
be confirmed
Focus on What, Not How
The system shall provide a slider control to adjust the volume level
The system shall provide for the adjustment of the volume level
•

Don’t be ambiguous

The system shall display accurate temperature readings
The system shall display temperature readings to an accuracy of 0.1oC
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

13

Requirement Writing-Examples & Tips

• Check Verifiability
• The readout shall update regularly
• The readout shall update every ten seconds
• Check Consistency
• The truck shall have two axles
• The vehicle shall carry a maximum net weight of 1.5

tons

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

14

Requirement Writing-Examples & Tips
Check Ambiguity

Ambiguous

Unambiguous

The system shall check the name field
only accepts alphabetic and the address
field to be either alphabetic or numeric
but containing only Australian addresses
and the quantity field to be only
numeric

The system shall validate that:
• The name field is alphabetic only
• The address field to be either
alphabetic or numeric
• All addresses are within
Australia only
• The quantity field is numeric
When an employee passes through the
onlythe system shall display a photograph
reader,

The system provides the identity of the
employee when passing through the
reader

of the employee on the monitor

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

15

Requirement Writing-Examples & Tips
Check Precision & Consistency

Imprecise

Precise

When the department code entered does
not match the department code on file,
the system shall display an error message

When the department code entered does
not match the department code on file, the
system shall display the error message
“Invalid department code”

17.1 The security system shall …
24.1 The new security system shall …
33.2.1 The secure card system shall …
45.3 The R/F security system shall …

17.1 The security system shall …
24.1 The security system shall …
33.2.1The security system shall …
45.3 The security system shall …

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

16

Requirement Writing-Examples & Tips
Check Completeness & Verifiability
Incomplete

Complete

The card reader shall be of the same dimensions as indicated
by the card size and consistent with industry standards

The card reader shall be 5 centimeter long and 3 centimeter
wide (the industry standard)

The system shall terminate a session after the number of
incorrect password attempts exceeds the maximum allowed

The system shall terminate a session after three incorrect
password attempts

Not Verifiable

Verifiable

There shall be no more than 6 training sessions per
employee

Each employee shall have not less than 2 and no more than 6
training sessions residing on their professional development
profile

The new production line shall be efficient

The new production line shall produce not less than 5000
bottle caps per day

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

17

REQUIREMENT
WRITING
Example

Case Study Scenario: E-commerce Solution for a Dental Practice in Australia
Background
BrightSmile Dental Clinic is a well-established dental practice in Brisbane, Australia. The clinic offers a range of dental services, including
routine check-ups, cosmetic dentistry, and orthodontics. To enhance patient experience and streamline operations, BrightSmile Dental
Clinic decides to implement an e-commerce solution for selling dental products and booking appointments online.
Business Needs
1.

Increase Revenue: By selling dental care products online, the clinic aims to generate additional revenue streams. This will not only
boost the clinic's financial health but also provide patients with easy access to recommended dental products, encouraging better
oral hygiene practices.

2.

Enhance Patient Convenience: Providing an online platform for booking appointments and purchasing products will improve patient
satisfaction and loyalty. Patients can book appointments at their convenience, reducing wait times and ensuring they receive timely
care. Additionally, they can purchase dental products without needing to visit the clinic, saving time and effort.

3.

Operational Efficiency: Automating appointment scheduling and product sales will reduce administrative workload and improve
overall efficiency. Staff can focus more on patient care rather than managing appointments and inventory manually, leading to a
more streamlined and productive workflow.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

19

Case Study Scenario: E-commerce Solution for a Dental Practice in Australia: Stakeholder
Needs
Patients:

Dental Staff:

Clinic Management:

o

Easy Access: A user-friendly website and mobile
app for booking appointments and purchasing
products. The interface should be intuitive,
allowing patients of all ages to navigate easily
and complete their tasks without frustration.

o

o

Sales Reports: Detailed reports on product
sales and appointment bookings to analyze
business performance. These insights will help
in making informed decisions, identifying
trends, and planning future strategies.

o

Secure Transactions: Ensuring that all online
transactions are secure and patient data is
protected. Implementing robust encryption and
security protocols will build trust and
encourage more patients to use the online
services.

Appointment Management: A system to
manage and track patient appointments
efficiently. This includes features like
calendar integration, automated
reminders, and easy rescheduling options
to ensure smooth appointment handling.

o

o

Marketing Tools: Features to promote products
and services through targeted marketing
campaigns. Personalized promotions and
discounts can attract more patients and boost
sales.

o

Product Information: Detailed descriptions and
reviews of dental products to help patients
make informed decisions. Providing
comprehensive information, including usage
instructions and benefits, will assist patients in
choosing the right products for their needs.

Inventory Management: Tools to monitor
and manage the stock of dental products.
Real-time inventory tracking and
automated restocking alerts will help
maintain optimal stock levels and prevent
shortages.

o

Compliance: Ensuring the solution complies
with Australian healthcare regulations and data
protection laws. Regular audits and updates
will ensure the clinic remains compliant and
avoids legal issues.

o

Customer Support: Access to patient
information and order history to provide
better customer service. Staff can quickly
resolve issues and answer queries,
enhancing the overall patient experience.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

20

Case Study Scenario: E-commerce Solution for a Dental Practice in Australia: Technical
Solution
E-commerce Platform:
o

o

o

Appointment Scheduling System:

Inventory Management System:

Website and Mobile App: Develop a responsive o
website and mobile app for patients to book
appointments and purchase products. The
platform should be accessible on various
devices, providing a seamless experience
across desktops, tablets, and smartphones.

Online Booking: Allow patients to book, o
reschedule, and cancel appointments
online. The system should provide realtime availability and confirmation to avoid
double bookings and ensure efficient
o
scheduling.

Payment Gateway Integration: Secure payment o
processing for online transactions. Multiple
payment options, including credit/debit cards
and digital wallets, will cater to different
patient preferences.

Automated Reminders: Send automated
reminders to patients for upcoming
appointments. This will reduce no-shows
and ensure patients are reminded of their
o
appointments well in advance.

o
Product Catalog: An organized catalog of
dental products with detailed descriptions and
reviews. High-quality images and
categorization will help patients find and select
products easily.

Calendar Integration: Sync appointments
with the clinic's calendar system. This
ensures that all staff are aware of the
schedule and can prepare accordingly.

Stock Monitoring: Track inventory levels and
receive alerts for low stock. This helps in
maintaining adequate stock levels and
prevents disruptions in product availability.
Order Management: Manage orders from
placement to delivery. The system should
handle order processing, shipping, and
tracking to ensure timely delivery and
customer satisfaction.
Supplier Integration: Integrate with suppliers
for seamless restocking. Automated
purchase orders and supplier
communication will streamline the
restocking process.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

21

Case Study Scenario: E-commerce Solution for a Dental Practice in Australia: Technical
Solution
Security and Compliance:
o

Data Encryption: Encrypt patient data and transaction
information. This ensures that sensitive information is
protected from unauthorized access and breaches.

o

Regular Audits: Conduct regular security audits and
vulnerability assessments. Identifying and addressing
potential security risks will maintain the integrity of the
system.

o

Regulatory Compliance: Ensure the solution complies with
Australian healthcare regulations and data protection laws.
Staying updated with regulatory changes and implementing
necessary adjustments will keep the clinic compliant.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

22

Case Study Scenario: E-commerce Solution for a Dental Practice in Australia: User Stories
Patients

Dental Staff

1. Easy Access:

1. Appointment Management:

- As a patient, I want a user-friendly website and mobile app so
that I can easily book appointments and purchase dental products
without any hassle.

- As a dental staff member, I want a system to manage and track
patient appointments efficiently so that I can ensure smooth
scheduling and reduce double bookings.

2. Secure Transactions:

2. Inventory Management:

- As a patient, I want all my online transactions to be secure so
that I can trust the platform with my personal and financial
information.

- As a dental staff member, I want tools to monitor and manage the
stock of dental products so that I can maintain optimal inventory levels
and avoid shortages.

3. Product Information:

3. Customer Support:

- As a patient, I want detailed descriptions and reviews of dental
products so that I can make informed decisions about which
products to buy.

- As a dental staff member, I want access to patient information and
order history so that I can provide better customer service and resolve
issues quickly.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

23

Case Study Scenario: E-commerce Solution for a Dental Practice in Australia: User Stories
Clinic Management

Technical Solution

1. Sales Reports:

1. E-commerce Platform:

- As a clinic manager, I want detailed reports on product sales and
appointment bookings so that I can analyse business performance
and make informed decisions.

- As a patient, I want a responsive website and mobile app so that I
can access the platform on various devices and have a seamless
experience.

2. Marketing Tools:

- As a patient, I want secure payment processing for online
transactions so that I can choose from multiple payment options and
feel confident in the security of my transactions.

- As a clinic manager, I want features to promote products and
services through targeted marketing campaigns so that I can attract
more patients and boost sales.
3. Compliance:

- As a patient, I want an organized catalogue of dental products with
detailed descriptions and reviews so that I can easily find and select
the products I need.

- As a clinic manager, I want to ensure that the solution complies
with Australian healthcare regulations and data protection laws so
that the clinic remains compliant and avoids legal issues.
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

24

Case Study Scenario: E-commerce Solution for a Dental Practice in Australia: User Stories
Technical Solution
2. Appointment Scheduling System:
- As a patient, I want to book, reschedule,
and cancel appointments online so that I can
manage my appointments at my convenience.
- As a patient, I want to receive automated
reminders for upcoming appointments so that
I don't forget my scheduled visits.
- As a dental staff member, I want the
appointment system to sync with the clinic's
calendar so that all staff are aware of the
schedule and can prepare accordingly.

3. Inventory Management System:
- As a dental staff member, I want to track
inventory levels and receive alerts for low
stock so that I can maintain adequate stock
levels and prevent disruptions in product
availability.
- As a dental staff member, I want to manage
orders from placement to delivery so that I
can ensure timely delivery and customer
satisfaction.
- As a dental staff member, I want to
integrate with suppliers for seamless
restocking so that the restocking process is
streamlined and efficient.

4. Security and Compliance:
- As a patient, I want my data and
transaction information to be encrypted
so that my sensitive information is
protected from unauthorized access.
- As a clinic manager, I want regular
security audits and vulnerability
assessments so that potential security
risks are identified and addressed.
- As a clinic manager, I want to ensure
the solution complies with Australian
healthcare regulations and data
protection laws so that the clinic remains
compliant and avoids legal issues.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

25

Case Study Scenario: Functional and Non-functional Requirements for E-commerce Solution for a Dental Practice
Functional Requirements
1.
2.

3.

4.

User Authentication:
o The system must provide secure login options, including multi-factor authentication (MFA) and biometric login (fingerprint,
facial recognition).
Appointment Management:
o The system must allow patients to book, reschedule, and cancel appointments online.
o The system must send automated reminders to patients for upcoming appointments.
o The system must sync appointments with the clinic's calendar system.
E-commerce Platform:
o The platform must include a responsive website and mobile app for booking appointments and purchasing products.
o The platform must integrate with a secure payment gateway to process online transactions.
o The platform must feature an organized product catalog with detailed descriptions and reviews.
Inventory Management:
o The system must track inventory levels and send alerts for low stock.
o The system must manage orders from placement to delivery.
o The system must integrate with suppliers for seamless restocking.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

26

Case Study Scenario: Functional and Non-functional Requirements for E-commerce Solution for a Dental Practice
Functional Requirements
1.

2.

3.

4. Inventory Management:
User Authentication:
o The system must track inventory levels and
o The system must provide secure login options, including multi-factor
send alerts for low stock.
authentication (MFA) and biometric login (fingerprint, facial
o The system must manage orders from
recognition).
placement to delivery.
Appointment Management:
o
The system must integrate with suppliers
o The system must allow patients to book, reschedule, and cancel
for seamless restocking.
appointments online.
o The system must send automated reminders to patients for upcoming 5. Customer Support:
o The system must provide dental staff with
appointments.
access to patient information and order history
o The system must sync appointments with the clinic's calendar system.
to resolve issues and answer queries.
E-commerce Platform:
6.
Sales
and Marketing:
o The platform must include a responsive website and mobile app for
o The system must generate detailed sales reports
booking appointments and purchasing products.
on product sales and appointment bookings.
o The platform must integrate with a secure payment gateway to process
o The system must include marketing tools to
online transactions.
promote products and services through targeted
o The platform must feature an organized product catalogue with
campaigns.
detailed descriptions and reviews.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

27

Case Study Scenario: Functional and Non-functional Requirements for E-commerce Solution for a Dental Practice
Non-functional Requirements
1. Performance:

4. Compliance:

o

The website and mobile app must load within 3 seconds.

o

o

Transactions must be processed within 5 seconds.

The system must comply with Australian healthcare
regulations and data protection laws.

o

The system must be regularly updated to reflect any
changes in regulatory requirements.

2. Security:
o

The system must encrypt all patient data and transaction
information.

o

The system must undergo regular security audits and vulnerability
assessments.

3. Usability:

5. Scalability:
o

The system must be able to handle an increasing number
of users and transactions without performance
degradation.

6. Reliability:

o

The platform must have an intuitive user interface that is easy to
navigate.

o

The system must have a high uptime, with minimal
downtime for maintenance.

o

The design must be accessible to users with disabilities, complying
with relevant accessibility standards.

o

The system must include backup and recovery
mechanisms to prevent data loss.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

28

Thank you

