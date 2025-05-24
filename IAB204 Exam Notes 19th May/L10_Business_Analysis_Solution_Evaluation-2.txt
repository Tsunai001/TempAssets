Solution Quality
Assurance
Validation, Quality, and Testing
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

Validation Techniques

Lecture
Overview

Solution Quality

Testing Approaches
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

3

Solution
Validation/Evaluation
Evaluate Performance
Measures
• How solution performance will be
measured?
• Metrics for how well solution meets
business goals & objectives
• How those metrics will be captured
and reported
• Are measurement capabilities built
into the solution?
• Are there existing ways to extract
the evaluation data?

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

4

4

Key Performance Indicators
Measure performance of solution
• Key components of monitoring and evaluation

Indicator:
• Specific numerical measurement of progress towards a goal, objective, activity (i.e. Cycle Time, Efficiency, Productivity, Cost Reduction etc.)
• Characteristics: clear, relevant, economical, adequate, quantifiable
• Considerations: source and data collection resource, method, cost, frequency and difficulty

Metric: quantifiable level of an indicator, measured at a specific point in time
• Each indicator usually has a single metric
• May be a specific point, threshold or range
• Target metric is to be met within a certain period
• Considerations: baseline, assigning resources, political concerns

Structure: procedures for data collection (include baseline), data analysis, reporting
• Considerations: reliability, validity & timeliness

Reporting: compare baseline, current and target metrics
• Trends are generally more important than absolute values
• Charts are a useful means to show and explain data

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

5

Key Performance Indicators (Examples)
Business Process-Key Performance Indicators (KPIs)
1. Percentage of processes where completion falls within +/- 5% of the estimated
completion
2. Average process overview time
3. Percentage of overdue processes
4. Average process age
5. Percentage of processes where the actual number assigned resources is less than
planned number of assigned resources
6. Sum of cost of “killed”/stopped active processes
7. Average time to complete task
8. Some of deviation of time (e.g., in days) against planned schedule of all active
projects
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

6

Validation Techniques
Surveys
1.Gather information from large and/or dispersed populations
2.Quantify qualitative data
3.Can capture:
• Satisfaction
• Performance
• Challenges & issues
Focus Groups
1.Feedback from solution users
2.Testing
•Exploratory & User Acceptance Testing (UAT)
•Day-in-the-Life Testing (DITL)
• Use Case scenarios
•Integration Testing
•Functional Requirements Testing
•Non-functional Requirements Testing
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

7

SOFTWARE
QUALITY
TESTING

Quality
Quality?
– Degree of excellence (Oxford)
– Fitness for use (Juran)
– Conformance to requirement (Crosby,
Horch)
Quality assurance?
– A planned and systematic approach to
the evaluation of the quality of and
adherence to software product
standards, processes, and procedures
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

9

System Quality
Purpose of Quality
• To satisfy customers
needs and
requirements
• To ensure standards
are followed
• For reputation

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

Quality Programme
• To ensure that the systems
produced is of high quality,
the program involved:
– inspections – will detect
problems earlier in the
lifecycle
– testing – will detect problems
once an artifact is produced,
more on the performance,
timing and transaction
problems
10

Defects and Prevention
• Defects?
– problems detected in the output
from an activity in systems
development such as a bug in the
prototype or a flaw in the design

Defects can be detected
through inspections
done earlier in the
lifecycle i.e. :

• Types of defects:
– major. lead to failure of the system
and is observed by customers
– minor. will not lead to system
failure and unnoticed by customers

Requirement
specification

Design

Coding

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

11

How to do Inspection/Testing?
•

Can be a form of defect prevention as well
Conduct a requirement walkthrough

Conduct formal code review

• Check the requirement specification and look for
any extra or missing statements

•Let the chief architect or technical team
leader check the codes – every few weeks

Conduct peer design and code reviews

Document the results

• Compare the design with the requirement
specification
• Let fellow programmers check the codes as often
as possible – preferably every week

•For every reviews, document each findings

Collect metrics
• Collect statistics that show how many defects are found in different
stages of lifecycle
• This information will be good for estimations and risk management
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

12

Importance of Testing

In May 2015, Airbus issued an alert for urgently checking its
A400M aircraft when a report detected a software bug that had
caused a fatal crash earlier in Spain. Prior to this alert, a test
flight in Seville has caused the death of four air force crew
members and two were left injured.
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
https://www.cigniti.com/blog/37-software-failures-inadequate-software-testing/
Dr Rehan Syed. School of Information Systems, Faculty of Science

On June 4, 1996 the Ariane 5 rocket, which was scheduled
to put telecommunications satellite into space, exploded
just after lift-off. The European Space agency had spent
over a decade for developing the $7 billion rocket and
preparing it for its first voyage. The total destruction was
valued at $500 million. The inquiry board’s investigation
report attributed the failure to a software error in the
inertial reference system.
13

13

Importance of Testing: Confirmation of Expected Results
(Insurance Company Example)
•

•

Consider the example of an insurance company where the business need is to provide a software solution so that
a claim can be submitted via a mobile device. part of the evaluation of the solution is to look at the results of test
where the claim is retrieved using the mobile device to ensure that the actual claim is presented as expected.
However, in an insurance company, a claim can be retrieved in other ways, such as through a reporting
mechanism or another interface such as a claim adjuster’s workstation. When those usages are not part of the
scope of the solution, it is still part of the scope to accurately store the claim data so that it is available for any
usage.
To verify that the data is accurately stored an available for other forms of retrieval, the results that were obtained
by accessing the data directly from its storage location should be reviewed to confirm whether the actual stored
values match the expected stored value. even when direct confirmation of stored data is included during testing, it
is worthwhile to confirm it again as part of evaluating the most used portion of the functionality. evaluation of a
software solution is usually conducted against a system that is either about to be released or has already been
released; therefore, testing during evaluation usually encompasses a larger body of data then the initial testing. as
a result, new and different kinds of data anomalies may be uncovered by looking at the results of tests use to
directly confirm the data, and those anomalies will need to be analysed.
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

14

Software Testing Methods
Unit testing
• To test each module
Integration testing
• To test the integration between modules
System testing
• To test the performance of the whole system
User Acceptance Testing (UAT)
• To get users acceptance
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

15

Unit Testing
Test
Case
ID

Requirement
Reference #

Unit: Login Form
1
5.1

Test Case Objective

Procedure to
follow

Login to the system
1) Enter correct
with the correct User
User Name and
Name and Password
Ex – IT User
Password.

Input

Expected
Output

Actual
Output

Success or
Failure

Comments

Displayed
“welcome”
message

Failure

Change the format
of the message
box

No error
message

Failure

Construct code to
display the
message in a
message box.

User Name :
Display
No error
Paul
“Incorrect User message
Password: 321 name or
Password”
Message

Failure

Construct code to
display the
message in a
message box.

User ID: Syed Display
Password: 123 “Successful
Login”
Message

2) Click “Login”
Button
2

5.1

Login to the system 1) Leave all fields
with no User Name
as a blank
and Password (blank
Fields)
2) Click “Login”

-

Display “Fields
cannot be
Empty”
Message

Button
3

5.1

Login to the system
with Incorrect
Username and
Password

1) Enter User
Name and
Password.
2) Click “Login”

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

16

Integration Testing
Test Case
Id
01

Test Case Objective
Login form and Service Catalogue
Management Module

02

Integration of the above modules with
Service Request Management Module

03

Integration of the report module with the
above modules mentioned in test case Id 1
and 2

Expected Result

Actual Result

Comments

User should be able to
login successfully and
conduct functions of
service catalogue
management module
The information flow
from one module to
another should be
smooth and
appropriate.
Filtered and accurate
results should be
displayed

Successful User
login.
Viewed/accessed
service catalogue
functions.
Incorrect access to
confidential reports
for User-Category#.

-

Incorrect values in
daily service
reports.

-

-

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

17

System Testing
Test
Case
Id
01

02

System Configuration

Expected Result

Actual
Result

Comments

OS- Windows 7 64-bit
operating system) Intel (R)
Core (TM) i3 processor
320GB Hard Drive
OS-Windows 7 (32-bit
operating system) Intel (R)
Core (TM) i7 processor
320GB Hard Drive

Application load
time should be < 8
seconds

Loading
took 12
seconds

-

Application load
time should be < 5
seconds

Loading
took 3
seconds

-

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

18

User Acceptance Testing (UAT)
Usability Acceptance Questionnaire for Web Based Help Desk System
Criteria
Visibility
Performance

Navigability
Consistency
Functionality

Have the colors been used Effectively?
How user friendly is the font size used?
How user friendly is the Font Type used?
To what level does the system meet your
requirements?
To what level does the system meet the
efficiency?
To what extent does the system provide the
expected outcome?
To what extent does the security reach your
expectation?
To what level does the system developed satisfy
you?
To what level Does the system provide you Clear
accessibility to other pages from the home page?
How consistent is the usage of font size, types and
colors?
How consistent is the design and layout?
Clear labeling of functions
Ability of beginners as well as expert level users
Availability of essential functions

Rank (Please Provide a rank scale from 1-5 for each criteria)
Very High
High
Moderate
5
4
3
5
4
3
5
4
3
5
4
3

Low

2
2
2
2

Very low
1
1
1
1

5

4

3

2

1

5

4

3

2

1

5

4

3

2

1

5

4

3

2

1

5

4

3

2

1

5

4

3

2

1

5
5
5
5

4
4
4
4

3
3
3
3

2
2
2
2

1
1
1
1

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

19

Functional Acceptance Criteria
Preconditions

Event

Expected Results

Customer X is an
active medium-term
customer

Customer X
submits a claim for
$600

Claim is created as pended claim

Claim’s maximum
automatic settlement
amount is $500

Actual Results

Message is “Thank you for submitting
your claim. Your claim will be forwarded
to a claim adjuster and will be
settlement in 5 days.”

Manual settlement
service-level
agreement is 5 days
TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

20

Non-Functional Acceptance Criteria
Field

Definition

Example Criteria (Insurance case study: Slide 14)

Type

Designation of the kind of non-functional requirement for
which the acceptance criteria is being defined

Useability

Name

A unique designation of this non-functional requirement

Customer ease of use

Description

A very short summary that explains what is to be measured

Elapsed time between the time a new customer starts to
submit a claim and the time that the new customer
completes the submission (a new customer is someone
who is submitting a claim for the first time)

How to measure

How the solution characteristics will be measured and what
the measurement units will be

Elapsed time in minutes to complete a claim submission (as
measured by a stopwatch for paper forms and by weblog
timestamps for mobile app)

Worst Case Value

The minimally acceptable value

Not more than 15 minutes for 90% of the measurements

Target Value

The expected value for the solution characteristic

Not more than 10 minutes for 90% of the measurements

Best Case Value

The ideal measurement for the solution characteristic,
where there is no commitment to achieve this value

Not more than 5 minutes for all measurements

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

21

Use Cases as Test Cases

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

22

Decision Tables
• Definition:
• A decision table is a tabular method for
representing and analyzing decision rules.
• Key Components:
• Conditions: The criteria that influence the
decision.
• Actions: The possible outcomes or decisions.
• Rules: The combinations of conditions that
lead to specific actions.
• Benefits:
• Simplifies complex decision-making
processes.
• Ensures consistency and completeness in
decision-making.
• Facilitates communication and understanding
among stakeholders.

Condition

Rule 1

Rule 2

…

Rule…N

Condition 1
Condition 2
…
Condition N

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

23

Action

Decision Tables
Example: Decision table for a loan
approval based on credit score and
income level.

Example: Decision table for discount
eligibility based on customer type and
purchase amount.

Credit Score

Income Level

Loan Approval

Customer Type

Purchase Amount

Discount Eligibility

700+

High

Approved

Regular

Above $100

Eligible

700+

Low

Approved

Regular

Below $100

Not Eligible

Below 700

High

Approved

Premium

Above $100

Eligible

Below 700

Low

Denied

Premium

Below $100

Eligible

TEQSA Provider ID PRV12079 Australian University | CRICOS No.00213J

Business Analysis (IAB204)
Dr Rehan Syed. School of Information Systems, Faculty of Science

24

Thank you
25

