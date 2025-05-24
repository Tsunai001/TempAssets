Requirements Analysis
Modelling for Analysis
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

Requirements Analysis
•

•
•

Requirements analysis involves organising requirements,
modelling requirements and designs, validating
information, identifying solutions that answer the
business needs, and assessing the potential value gained
by performing these tasks
Activities and techniques used to analyse stated
requirements that will define the required capabilities of a
solution
It includes the definition of:
• Stakeholder requirements, which describe what the
solution must be capable of
• Solution requirements, which describe component
behaviours in enough detail for them to be
constructed
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

3

3

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

(as a <> I want to <> so that)

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

Support

(Why a project is required?)

Stakeholder Requirements

Support

Implemented by

Business Requirements

Direct/Constrain

Non-Functional Requirements

Functional Requirements

(Operating Condition for a
solution)

(a solution must include?)

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

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

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

Business Rules

(Policies, Org.
Constraints)
•
•
•

Approvals & Authorisations
Methods
…

Must comply with

4

Specify and Model Requirements
• Document and analyse stakeholder desires
and/or the current state of the organisation
using a combination of textual statements,
matrices, diagrams and formal models

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

5

Characteristics of Requirement Quality
• Cohesive – defines a single aspect of the desired business process or system.
• Complete – individual requirement is not missing necessary or relevant
information. Set represents all relevant requirements
• Consistent – not contradictory, uses similar terms and wording, level of
detail
• Unambiguous – must be written objectively; only one interpretation
• Correct – will lead to a valid solution
• Feasible – within technical architecture, budget, time, resources
• Modifiable – logically structured so that requirements can be re-arranged
easily (*not changed)
• Testable – must be able to prove that the requirement has been fulfilled
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

6

Solution Scope
ATM System
Check
Balances
Deposit
Funds

Customer

Withdraw
Cash
Transfer
Funds

Perform
Maintenance

Repair

ATM Technician

Context Diagram

Use Case Diagram

Business Process Model

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

7

Writing Guidelines
• Express exactly 1 requirement at a time
• Avoid complex conditional clauses (eg. nested ifs)
• Do not assume reader has domain knowledge
• Use consistent terminology
• Use terminology familiar to the stakeholders
• Clearly describe who is responsible for fulfilling the requirement

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

8

Common Issues
• Missing or incorrect requirements
• Inclusion of non-essential requirements
• Vague or incomplete requirements
• Avoid vague words: minimise, maximise, optimise, rapid,
user-friendly, easy, simple, often, normal, usual, large,
intuitive, robust, state-of-the-art, improved, efficient,
and flexible.
• Never use: "and/or" or "etc."
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

9

Requirements Terminologies
Keyword(s)
SHALL
SHALL NOT
SHOULD

Denotes
Absolute requirement
Absolute prohibition
Can be ignored in
certain
circumstances

Alternatives
MUST, REQUIRED
MUST NOT
RECOMMENDED

SHOULD NOT

Can be included in
certain
circumstances

NOT RECOMMENDED

MAY

Optional requirement

OPTIONAL

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

RFC2119 http://www.ietf.org/rfc
/rfc2119.txt
10

Diagrams & Models
• Provide a set of views of the requirements that are (together with text and
matrices):
– Comprehensive
– Complete
– Consistent
– Understood by all

• Simplified representation of a complex reality
• May use text to annotate graphics
• May be formal (follows rules, semantics, syntax) or informal
• – Meaningful for the audiences

• Can be used to describe: Business processes

A scope (define boundaries)
Thoughts & action flows

Categories & hierarchies
Components & relationships
Business rules and logic

Levels of Abstraction
• How much detail is expressed varies when describing requirements
 depends on the audience
 organisational standards or
 methodologies may determine abstraction levels
• What vs How…
• Different stakeholders  different perspectives

Modelling limitations
• A model is one representation of the real world
– Can’t capture everything

• A model is never perfect
– If GPS tells you to drive into the river, do you do it?
– Trying to perfect it usually not a good use of BA time

Current State
• Current domain models are useful for:
– Validating the solution scope with stakeholders
– Identifying improvements to the current state
– Assisting stakeholder understanding

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

14

Model Selection
• Formulae / diagrams / text descriptions / scale constructions
• Models abstract and simplify reality in their own specific way
– May need multiple models to fully represent a requirement to enable
its ‘bringing to life’

• BA models work in different ways. For example:
– BPM captures the process then identifies roles, events etc.
– Use cases identify goals and then capture processes and (actor) stakeholders

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)

6.2ofOrganise
Reqs:Systems,
ElementsFaculty of Science
Dr Rehan Syed. School
Information

15

Common modeling elements
• Users (classes, profiles, roles): categorise and describe the people who interact
with the solution
• Concepts & Relationships: people, places, things, entities relevant to the business
domain and with possible relationships to other concepts / objects
• Events: a request to a business system to do something
– The system responds to events in a pre-planned way
– Internal, external, time based

• Processes: a sequence of repeatable activities executed within an organisation
– Describe who and what is involved in these activities

• Rules: used by organisations to enforce goals and make decisions
– Determines operations and priorities

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

16

Modelling Techniques
Users Concepts Events Processes Rules
Users

Modelling Technique

Business Rules Analysis

X

Data Flow Diagram

X

Data Modelling

X

Functional Decomposition

X

Organisational Modelling

X

Process Modelling

X

Scope Modelling

X

X
X

State Diagrams
Use Cases

X

User Stories

X

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

X
X

X
X

X

X

X
X

X

X

X

X

X

17

Use Case Scenario

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

18

Consider a bookstore…

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

19

Question
How do the bookstore retailers respond to customers’ business needs?

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Buyers have a business need

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

Sellers have a pre-planned response
20

Possible User Stories
As a book buyer, I want
to have access to a book
seller so that I can
purchase a book of my
choice.

As a book seller, I need to
use a purchase and
inventory system so that
I can sell a book to a
buyer.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

21

10 Mins Exercise: List the interactions
• Of the seller
– Their pre-planned response to a customer who wants to buy a book
– Assume the bookstore has common point-of-sale and EFTPOS
technology
• And of the buyer
– Their required information flows and actions to complete the
transaction
• Don’t describe alternative purchasing activities – just pick one type of
transaction and describe that…
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

22
22

You may have something like this....
1.
2.
3.
4.
5.
6.

Buyer presents the item to be purchased to the store assistant
Store assistant sets POS machine state to ‘New Sale’
Store assistant scans (the bar code of) the item
Store assistant scans further items (optional)
Store assistant informs the customer of the total amount payable
Store assistant asks the customer what method of payment they will employ: [cash,
EFTPOS or credit]
a)

Example: Cash – Shop Assistant takes the cash, enters the amount tendered into the POS
machine. POS machine calculates change and opens the cash draw. Shop assistant puts
amount tendered on the ledge on top of the draw; takes the change from the drawer and gives it
to the customer then puts the tendered amount in the draw. POS machine prints receipt.

7. Store assistant applies item to device that neutralises the security RFID embedded in
the item
8. Store assistant packs the items and includes the receipt, finalising the transaction
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

23

This is an example of a “Use Case Scenario"
• Scenarios are written to describe how an actor
interacts with a solution (or object or system) to
accomplish one particular goal.
• A Scenario describes one possible way of achieving
the goal
• A Use Case describes all the possible outcomes of an
attempt to achieve the goal
• Consider more scenarios for a bookstore interaction
e.g. book out of stock, gift card, payment declines
etc.
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

24
24

What is a Use Case?
• a collection of related success and failure scenarios,
describing actors using the system to support a goal.
• A list of steps an actor might take in trying to get something
done:
– Starts with whatever event serves as a trigger for their interaction with a
business (or system)
– Recounts each and every step they take
– Ends when they’ve either succeeded or failed in what they need to do

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

25

Actors
• Who are the ‘actors’ in the Use Case?
– Any person, system or event external to the
system (under design) that interacts with the
system

• The primary actor initiates an interaction with
the system
– Primary actor is a user whose goals are fulfilled
by the system (importance: define user goals)
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

26

Relationships
• Association: a relationship between an
actor and a use case
– They don’t represent inputs, outputs, time or
dependency

Open
account
Customer

• Stereotype: a relationship between use
cases
– An Extend Stereotype will reference an original
(complete) use case, to describe additional
behaviour
– An Include Stereotype makes use of common
or shared functionality in another use case.

t en
ex
<<

>
d>

Defer
Payment

Pay Bill
Patient

i
<<

>>
de
u
l
nc

Check
Patient
Record

Make
Appointment
Patient

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

27

Generalization
General
“User” actor

Login

Login

User

Passenger

Business Traveler
Login

The Generalization
Arrow

The specialized
“Administrator”
actor

Tourist

Login
Employee

Business
Traveler

Tourist

Employee

Administrator

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

28

Use Case Diagram (UML)
association

ATM System

subject, organization or
solution boundary

Check
Balances
Deposit
Funds
Customer

actor

Withdraw
Cash

actor

Transfer
Funds
Perform
Maintenance

Repair

use case

ATM Technician

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

Source: uml-diagrams.org

29

UML Use Case Diagram (Bookstore)
Bookstore

Search
Book
Order
Book

Buyer
<<extend>>

Back
Order
Supplier

Seller
<<include>>

Make
Payment
Bank

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

30

Pre-conditions
• Can we assume certain pre-conditions: things that must exist or
be true when the Use Case begins?
– Consider each actor
1.
2.
3.
4.
5.

Sufficient cash in the till to provide change
Shop assistants identified / logged in
RFID security device enabled
POS machine operational and connection to the bank enabled
Customer has appropriate payment capability

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

31

Post-conditions
• Any fact that must be true when the use case is complete.
• Sometimes called guarantees
– true for successful and unsuccessful executions of the use case
1. Cash draw must be closed
2. Transaction must be completed
3. All items processed

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

32

Summary of Definitions
• Actor: a person or object (e.g. external system) that exhibits a behaviour relevant to the
solution (enabled by the use case)
• Stakeholder: a person with a vested interest in the behaviour of the solution
• Primary Actor: the stakeholder who initiates an interaction with the solution
• Use Case: a collection of scenarios that describes how a primary actor uses the solution to
achieve a specific goal
• Use Case Set: a model of the required behaviour of the solution
• Scope: identifies the extent of the solution, or system of interest
• Pre-conditions and post-conditions: what must be true before and after the use case runs
• Main Scenario: the most common successful scenario in a Use Case (sometimes called the
result)
• Extensions: all possible alternative scenarios and error conditions that can happen in a specific
Use Case
• Inclusions: other full or partial scenarios or use cases that are ‘called’ by the use case in
question
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

33

7 Steps to Writing Use Cases
1. Identify the Actors
2. Identify the goals
3. Define the Pre-Conditions
4. Define the Post-Conditions
5. Describe the Main Flow
6. Describe the Exceptions (failure conditions)
7. Describe the Alternate Flows
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

34
34

Functional Decomposition Diagram
1. Prescription
Tracking

1.1 Track
Patients

1.1.1 Enter
Patient Info

1.2 Track
Drugs

1.2.1 Enter
Drugs

1.1.2 Enter
Patient History

1.2.2 Enter
Drug
Instructions

1.3 Track
Insurance

1.2.3 Process
Recalls
1.2.3.1
Receive Recall
Info

1.4 Track
Doctors

1.3.1 Enter
Insurance
Companies

1.4.1 Enter
Doctor Info

1.3.2 Enter
Covered Drugs

1.4.2 Enter
Prescriptions

1.2.3.2 Verify
recalls
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

1.2.3.3 Enter
recall

35

Data Flow Diagram

Context Level-DFD

Level 0-DFD

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

36

Data Flow
Diagram Rules

D1

D1

B1

A process is needed to
exchange data flows
between external agents

B1

A process is needed to
update/use a data store

D1

A process is needed to
present data from a data
store

D1

A process is needed to
move data from one
data store to another

B2

D1

B1

D2

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

D1

37

D2

Common Data Flow Diagram Errors
Gray Hole:

B1

Membership
application

B2

Black
Hole:
Inputs but no

3.1.2
Create a new
member
account

outputs

B1

D1

D1

Bank Statement

Employee status

Member
Accounts

D1

Employees

New account status

D1

D1

Employee

Existing
account

D2

D1

Insufficient Inputs to

Miracle:

D2

D2

3.1.3
Freeze
member
account
number

3.1.1
Generate an
employee bank
statement

Employee address

Accounts
Receivable
Department
Frozen account
notification

Outputs with no inputs

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

38

produce outputs

Activity Diagram
1. Identify the Process: Determine the
process or workflow you want to model.
2. Define Activities: List all the activities
involved in the process.
3. Determine the Sequence: Establish the
order in which the activities occur.
4. Identify Decision Points: Identify any
decision points where the flow can branch
based on conditions.
5. Add Swimlanes (if needed): Use swimlanes
to show which actor or system component
is responsible for each activity.
6. Draw the Diagram: Use UML notation to
draw the activities, decision points, and flow
of control.
7. Review and Refine: Check the diagram for
accuracy and completeness, and make any
necessary adjustments.
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

39

Elements of a UML activity diagram
Element

Description

Event

The event that triggers the business process. This is shown as a filled-in circle.

Actor

A named person, group or IT system with responsibility for carrying out one or more tasks.

Task

A round-cornered rectangular box that represents work conducted by an actor in one place at one time.

Swimlane

A ‘row’ of tasks that are conducted by one actor; a boundary is shown for each swimlane to distinguish the work of one actor from that
conducted by another actor. Where a task is completed by two actors together, for example, where a hotel booking is made by telephone,
a task should be shown straddling both swimlanes.

Decision point

A diamond-shaped box that represents the application of a business rule in order to determine the next task to be performed. Each process
flow emerging from a decision point is clarified using a ‘guard expression’, which is shown in square brackets. The guard expression
represents the business rule that determines whether or not the process can progress in a particular direction of flow. There may be
several flows emerging from a ‘decision diamond’, each of which has a guard expression stating the rule that must be satisfied.

Fork and join

Two lines are used to indicate where parallel processing is taking place.

Outcome

The situation resulting from the completion of the business process. This is shown as a bullseye – a filled-in circle within an outer circle.

Process flow

An arrow shown from an initiating event to a task, between tasks or from a task to a final outcome.

Timeline

A timeline indicating the length of time taken to conduct tasks within the process. This is an optional element but can be very helpful when
considering organisational or customer timing requirements.
40

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

40

Process Models

(a)
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

(b)
41

Process Modelling Exercise

• When a claim is received, we first check if the claimant has a valid
insurance policy. If not, the claim is rejected and the claimant is
informed.
• Otherwise, we assess the severity of the claim. Based on the
outcome (simple or complex claim), we send the corresponding form
to the claimant.
• Once the form is returned, we check it for completeness.
• If the form is complete, we register the claim in the Claims
Management System and the evaluation of the claim may start.
• Otherwise, we ask the claimant to update the form. When we receive
the updated form, we check them again and continue.

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

42

Requirement Interrelationships
•

Common relationships are:
– Necessity – implementing one particular requirement first needs another requirement
to be implemented. This relationship can be uni- or bi-directional.
– Effort – if the implementation of one requirement makes it easier to implement
another
– Subset – when the requirement is the decomposed outcome of another
requirement
– Value – when one requirement affects the desirability of another (+ve or –ve) or is
strongly related to another in delivering business value

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

43

Tracing: Requirement Interrelationships
Requirement ID

Requirement Description

Effort Estimate

R1

The stop button shall be red.

R2

The system shall provide a stop button.

R3

The system shall provide reports of accounts receivable older than 60 days.

4 days

R4

The system shall provide a general-purpose report generation utility.

5 days

R5

The system shall enable the user to specify the order of the displayed list in a wide
variety of ways.

5 days

R6

The system shall enable the user to specify that the list be displayed in alphabetical
order.

7 days

R7

The system shall enable the user to specify that the list be displayed in chronological
order.

2 days

R8

The system shall enable the user to specify that the list be displayed in employment
seniority order.

13 days

Dependency
Necessity

-2 days

Effort

Subset

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

44

44

Thank you

