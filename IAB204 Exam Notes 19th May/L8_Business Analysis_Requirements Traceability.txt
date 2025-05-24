Requirements
Traceability
Assumption, Constraints, Requirements Lifecycle

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

Requirement Traceability

Traceability Tasks

Lecture
Overview

Monitoring & Control
Assumptions and Constraints
and Impact on Requirements

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

3

What is Traceability? Organisational Goals & Objectives
Traceability is “the ability to
track solution requirements
from their origin to the
deliverables that satisfy them.”
(PMI, 2015)
• Traceability can be
bidirectional (backward and
forward)
• Traceability is important for
projects performed under
highly regulated, risky, and
complex context.

Business Requirements

Stakeholder Requirements

Solution Requirements

Solution

Transition Requirements

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

4

Requirement Traceability
•

What is Traced?
Requirements from origin to
deliverable

•

Some Traceability Attributes
•
•

Absolute reference: unique, lifelong identifier
Author: may be consulted for clarification

Project scope

•

Complexity: how difficult will it be to implement this

•

Solution design & development

•

Test strategies

•

Requirement relationships

•

Use cases

•
•
•
•
•
•

•

Models & diagrams

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

•
•

requirement
Ownership: individual or group that needs the requirement
Priority
Risks
Source: who holds the authority for a requirement
Stability: how mature is the requirement
Status: proposed, accepted, verified, prioritised,
implemented ...
Urgency: how soon is the requirement needed
Other: cost, resource assignment, revision, traced
from / to
5

Traceability & Monitoring
•

Activities related to managing
the requirement life cycle.
• Involves
– Continuous monitoring and
documenting of requirements
– Communication of the
requirements status to
stakeholders

Elicitation

Analysis

Operations

Validation

Business

Development

Specification

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

6

Requirement Life Cycle
OPEN

CLOSED

Proposed

Rejected

Approved

Cancelled

In progress

Deferred

Completed

Implemented

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

7

Assumptions and Constraints
•

Identify factors other than requirements that may affect the viability of potential
solutions

•

Assumptions

•

•

Factors believed to be true, but unconfirmed

•

May relate to current or future state

•

BA identifies, documents and attempts to confirm their accuracy and risk

•

Then identifies and manages risks around these
assumptions

Business constraints
•

Limitations on available solutions

•

Aspect of the current state that can’t be changed
•

•

e.g. budget, time, resources, skills, specific
requirements

Technical constraints
•

Architectural decisions that impact the solution

•

Resource utilisation, message size, timing, software, files, records etc.
•

Consider a mobile phone app / game

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

8

Assumptions and Constraints- Exercise
Constraint

Date (ID’d)

Assumption

Date (ID’d)

Type

Owner

Impact

Risk

Comments

Owner

Impact

Risk

Comments

1.

Technical S/W architecture is set by corporate as .NET

Technical Constraint

2.

Technical personnel only work 9-5pm

Business Constraint

3.

Users will have a late version browser

Assumption

4.

Payment is received in $AUD

5.

New page design will attract international customers

6.

No American Express credit cards

7.

Current infrastructure will handle new system

8.

New system must use existing hardware infrastructure

Business Constraint
Assumption
Business Constraint
Assumption
Technical Constraint

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

9

Five (5) Tasks of Traceability and Monitoring
5 Tasks of Traceability and Monitoring

Purpose

Tools and Techniques Used

1.Track requirements and capture the
requirement' status, sources and relationships
(including dependencies)

To provide evidence that the requirements are Traceability artefact or tools
delivered as stated
(Matrices, IBM Rational, Visual Trace
Spec, JIRA, Change Management Plan,
etc.)

2. Monitor requirements throughout their
lifecycle

To ensure appropriate supporting
requirements artifacts (such as models,
documentations and test cases) produced,
reviewed and approved, at each point in the
lifecycle

Traceability artefact or tools
(Matrices, IBM Rational, Visual Trace
Spec, JIRA, Change Management Plan
etc.)

3. Update a requirement's status as it moves
through the lifecycle stages

Track requirements toward closure

1. Communicate status to appropriate
stakeholders and
2. Record changes in the traceability
artifact

4. Communicate requirements status to PM and
other stakeholders

Keep them informed of requirements issues,
conflicts, changes, risks and overall status

Communication methods

5. Manage changes to requirements by
Maintain the integrity of the requirements and 1. Impact analysis
assessing impacts, dependencies and risks and associated artifacts
2. Dependency analysis
compare to requirements baseline
3. Risk analysis
4. Change Control plan
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

10

Task 1Track
• By using a traceability artefact or tool
• Capture requirement status, sources, and relationships (i.e. Dependencies)
• Provide evidence of requirement delivery according to specifications
Requirement Traceability Matrix
Project Name: Online Booking Management System
Business Requirement Document (BRD)
BR ID
BR-1

BF-2

Business Requiremnt / Use Case
Reservation Module

Payment Module

Functional Requirement Document (FRD)
FR ID

Functional Requirement/Use Case

Test Case Document
Priority

Test Case ID

FR-1

One Way Ticket Booking

High

TC-001

FR-2

Return Ticket Booking

High

TC-002

FR-3

Multi-City Ticket Booking

Med

TC-003

FR-4

Payment by Cash

Low

TC-004

FR-5

Payment by Credit Card

High

TC-005
TC-006

FR-6

Payment by Debit Card

High

TC-007
TC-008

FR-7

Payment by Paypal

Med

FR-8

Payment by EzyPay

Med

TC-009
TC-010
TC-011

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

IAB204-Business Requirements

11

11

Task 2  Monitor
• Through out the life cycles using a traceability artefact or
tool in order to ensure the appropriate supporting
requirements artefacts (such as models, documentation,
and test cases) are;
– Produced,
– Reviewed, and
– Approved
at each point in the lifecycle
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

12

Task 3  Update

As we move through the requirement
lifecycle stages, we:
• Communicate with appropriate stakeholders, and
• Record changes in the traceability artefact or tool
• To Track requirements towards closure.
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

13

Task 4  Communicate
To keep informed the Project Managers
and other key stakeholders on;
• Requirement issues
• Conflicts
• Requirement Changes
• Risks
• Overall status.
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

14

Task 5  Manage Changes to Requirements
•
•
•

•
•
•
•

Continuous assessment & comparison of project progress with requirement Baseline.
To maintain the integrity of the requirement and associated artefacts
Compliance with the Change Management Plan
– Plan Driven Formal (Requires approvals from a competent authority)
– Change Driven  Informal (Work with Product Backlog & Prioritisation)
Impact assessment
– When a requirement is changed the BA can review and analyse the impact
Dependencies Analysis
Requirement Coverage
– Tracing allows the BA to assess the coverage of the solution to the requirements
Risk Analysis / Changes in Risks

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

15

Task 5  Manage Changes to Requirements (cont.)
Gather information about the change
• Cost, risk, completed work, approved requirements

Impact analysis
• On baseline
• On conflicts with other requirements
• On BA work

All requests logged

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

16

Task 5  Manage Changes to Requirements (cont.)
Set out processes for requirements change requested and
approvals
• Might be based on cost of the change
• Could be a Change Control Board
Set out the Change Request Analysis Criteria:
• Costs and time estimates
• Benefits and risks
• Impact Analysis
• Recommended course of action
• Communication Plan
• Prioritisation
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

17

Task 5  Manage Changes to

Requirements (cont.)
Plan Driven Approaches

• Seeks to ensure only necessary changes occur
• May generate a mini project including elicitation,
analysis and solution design, and impact analysis
• Use change logs or registers
• In practice, if the number of changes increases
towards the end of the project, it tends to be due
to:
• Loose scope, lack of requirements ownership,
poor analysis, re-organisations, regulatory
changes and changing business needs
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

18

Task 5  Manage Changes to Requirements (cont.)

Change Driven Approaches
• Assumes it is difficult to identify
all requirements prior to
implementation starting
• Generally no separate change
management process distinct
from the iteration process –
identified changes are included in
a future iteration
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

19

Task 5 
Manage
Changes to
Requirements
(cont.)

Often more than one
alternative provided
• Pros and cons, assumptions,
risks, costs, etc
Recommendations:
• Approved
• Deferred
• Rejected
• More information needed

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

20

Thank you
21

