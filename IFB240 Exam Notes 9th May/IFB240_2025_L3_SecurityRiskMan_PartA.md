IFB240 Cyber Security
Lecture 3 – Part A
Managing Cyber/Info Security
Dr Leonie Simpson
lr.simpson@qut.edu.au

Why manage cyber/info security?
• Do you use
•
•
•
•

email including images, links, attachments?
external services for data storage (cloud) or email?
mobile devices: tablet, laptop, phone …?
portable data storage media?

• Do you connect to Internet for
•
•
•
•
•
•
•
•
•
•

Banking
Buying stuff
Checking the weather
Gaming
Getting health information and updates
Getting travel info (booking flights, accommodation, etc – or cancelling bookings )
Learning – Uni?
Looking at maps
Searches
Social networking

• Do you install software on your devices?

• ….. Lots of regular activities put info assets & systems at risk
2025

IFB240

2

How do you manage cyber/info security?
• Managing Cyber/InfoSec involves asking questions, such as
• What needs to be protected?

• What are your information assets? Where are they? How critical are they?

• Why do these assets need to be protected?

• What could go wrong - how could the asset be damaged? (Think threats & Vulns.)
• If this happened, what would the consequences and impact be?

• How can these assets be protected?

• What resources are needed to do this, and how much does that cost?
• How urgently is this required?

• What happens if these assets are not protected?
• And what could that cost?

• You don’t have unlimited resources, so making
tradeoffs is necessary
• Can’t afford to protect all assets against all possible threats
• Some level of risk involved – basically, a risk management exercise
2025

IFB240

3

What is risk?
• Definitions (Oxford Dictionary)
• A situation involving exposure to danger
• The possibility that something unpleasant will happen
• A person or thing regarded as a threat or likely source of danger
• http://www.couriermail.com.au/news/queensland/southeast-queensland-road-closures-cancellations-and-advice/story-fnkt21jb1227228368307?nk=a1c96f5eee1da509f6e281fdc9f8833c

2025

IFB240

4

What is risk?
• What does ‘risk’ mean in cyber/info security?
• Definition in the standard document AS/NZS 27005:2024
Information security risk management, on p 2 (Clause 3.1.3)
• Risk: ‘effect of uncertainty on objectives’

• Usually considered in terms of risk sources, potential events,
their consequences and their likelihoods
• Effect of event – consequences, deviation from normal state
• includes positive and/or negative

• Uncertainty – how likely is it that this event will happen?
• Objectives - Aspects of enterprise objectives to consider
•
•
•
•

financial
health and safety
information security
environmental

• May consider risk at different levels

• organizational, project, product, process

2025

IFB240

5

What is risk?
• Cyber/Info security risk of events is expressed in terms
of likelihood and consequences
• An event occurs
• With some likelihood: ‘chance of something happening’, and
• Has consequences: ‘outcome of an event affecting objectives’
• The consequence has some magnitude and impact

• Perception of magnitude defined by stakeholder perspective
• Example: $1000 loss from bank account
• Perspective of student account owner is different to perspective
of bank

• Impact on stakeholder varies – need to understand context

• We’re interested in security

• consequences that concern us most are negative ones

2025

IFB240

6

What is risk?
Info sec risk considers potential for threats and vulnerabilities to coincide and harm assets

Threat

Vulnerability

Event

Event

Likelihood of occurrence

Consequence of occurrence

(sometimes called chance or risk)

Risk
(sometimes called business risk)
2025

IFB240

7

What is risk?
• Negative event examples
• Power loss
• to device/building/suburb/entire east coast

• Communications system component failure
• In building/block/suburb/region

• Loss of access to stored data
• Theft of intellectual property
• Public disclosure of confidential information

2025

IFB240

8

What is risk?
• How does a threat act on an entity or asset?
• Via a vulnerability: a characteristic that allows threat to
manifest in security event
• Might be a flaw or weakness that can be exploited
• Vulnerability may not be a flaw – could be integral part of item
• Example: Computers require power -> Deny access by removing power supply
Vulnerability

Vulnerability

Entity

Threat
Source

Vulnerability

Entity

Entity

Threat

Threat

Threat

System

• Consequence of one event may be another event
• Can lead to a chain of events
2025

IFB240

9

What is risk?
• Recall that the threat source can be
• Natural

• Example: Bushfire, Earthquake, Flood, Storm, Tidal Wave

• Human action (Classify by threat actor intent)

• Accidental: Example: Errors, Omissions, Negligence,
• Deliberate: Consider motivation and capability of adversary

• There’s always a way into a target system

• A determined threat actor will find a vulnerability – maybe in
• Property

• Physical
• Technical (Exploit vulnerability, Bypass controls, Malware)

• Processes
• People (Phishing, Watering hole attacks, Disgruntled employee)

• You may not be the ultimate target, but you could be
collateral damage – are you a stepping-stone in a pathway
to another system (the intended target)?
2025

IFB240

10

How do we manage risk?
• Can’t eliminate every vulnerability
• Need process for determining most effective actions
• For organisations, process should be systematic and continual

• Best practice information security risk management is documented in
Australian Standards (based on ISO docs)
• AS/NZS 27005:2024 Information security, cybersecurity and privacy
protection – Guidance on managing Information Security Risk
• Part of a series of Standards documents for Information Security
Management, sometimes referred to as ISO27K
• We will discuss these in the Lecture 3 segments
• AS/NZS 27001:2023 Info security, cybersecurity and privacy protection –
Information security Management Systems - Requirements (Part B)
• AS/NZS 27002:2022 Info security, cybersecurity and privacy protection (Part C)

• These Standards docs available to QUT students for free via QUT Library
(details on how to access included in Week 3 tutorial question sheet – there are
some restrictions on QUT access, but this is a valuable resource)
2025

IFB240

11

How do we manage risk?
• Information security
risk management
process
• Process diagram from
AS/NZS 27005:2024 p8
• We will look at the
components of this, and
how they connect to each
other
• NOTE: you will use this process
as a framework for your
Assessment Task 2

2025

IFB240

12

Risk management process
Establish the context (Clause 6 in AS27005:2024)

• Consider these aspects

• External context: Relationship between organisation and external
environment
• Internal context: Understand the organisation – capabilities, goals,
objectives
• Risk management context: Goals, objectives, strategies, scope and
parameters of area the risk management process is being applied to
• Define risk criteria (Criteria against which risk is to be evaluated)
• For risk evaluation, consider
•
•
•
•

How consequences and likelihood will be defined, predicted and measured
How the level of risk will be determined
How combinations and sequences of multiple risks will be taken into account
The organization’s capacity

• For impact evaluation, consider

• Level of classification of asset, and type of breach (CIA)
• Degree of impairment/disruption/loss of business

• For risk acceptance, consider

• What the timeframes will be
• What level of risk is acceptable

• We don’t all have the same appetite for risk - actions deemed too risky by some
may be considered acceptable by others

2025

IFB240

13

Risk management process
Risk assessment (Clause 7 in AS27005:2024)
• Risk assessment is an important
part of risk management
• Sometimes done as a stand-alone
activity
• Need to consider context for risk
assessment to be effective

• Three main steps, performed in
this order
1. Risk Identification
2. Risk Analysis
3. Risk Evaluation

2025

IFB240

14

Risk management process
Risk Assessment: Step 1. Risk Identification
• What can happen, where and when?

• Want to identify risks to information security objectives of organisation
• Use an asset-based approach:
• Identify operational scenarios, in terms of assets and consider plausible
threats, existing controls and existing vulnerabilities,

• Or an event-based approach:

• Identify strategic scenarios through considering risk sources and how they
impact (evaluate events and consequences for business processes)

• Why and how can it happen?

• Consider causes and scenarios

• Tools and techniques
• Identify risks using

• Checklists (From other standards documents)
• Judgements based on experience (your own or others)
• Systems analysis

• Include all risks, whether they are under the control of the organisation or
not
2025

IFB240

15

Risk management process
Risk Assessment: Step 2. Risk analysis
• Use to determine the magnitude of identified risks
• Types of analysis
• Qualitative

• Uses descriptive scales (in words) with ordered categories
• Example:
• Consequence: Minor, moderate, major, catastrophic
• Likelihood: Rare, unlikely, possible, likely, almost certain

• Quantitative

• Use numerical values for scales
• Example:
• Consequence: $$$ to replace item, number of days w/out service, …
• Likelihood: Probability value (in range of 0 to 1, or expressed as %)

• Semi-quantitative !!!WARNING!!!

• Use qualitative scales, then assigns numerical values to categories
• Can be used in formulae for prioritization (with caution!)
2025

IFB240

16

Risk management process
Qualitative Risk Analysis: Example
Qualitative Consequence scale example:

Increasing Damage

From Information Risk Management Best Practice Guide p19

2025

Measure

Description

Major

Major problems would occur and threaten the
provision of important processes resulting in
significant financial loss
Services would continue but would need to be
reviewed or changed

Moderate

Minor
Insignificant

Effectiveness of services would be threatened
but dealt with
Dealt with as a part of routine operations

IFB240

17

Risk management process
Qualitative Risk Analysis: Example
Qualitative Likelihood scale example:

Increasing Probability

Information Risk Management Best Practice Guide p19

2025

Measure

Description

High

Is expected to occur in most conditions
(1 or more times per year)

Medium

The event will probably happen in most
conditions (about once every 2 years)

Possible

The event should happen at some time

Unlikely

The event could happen at some time
(once every 10 years)

(once every 5 years)

IFB240

18

Risk management process
Qualitative Risk Analysis: Example
Qualitative Determination of Level of Risk: Combine consequence
and likelihood scales to form table, cell entry indicates level of risk

Likelihood

Consequence
Insignificant

Minor

Moderate

Major

High

M

H

E

E

Medium

M

M

H

E

Low

L

M

M

H

Unlikely

L

L

M

M

Legend
E: extreme risk; immediate action required
H: high risk; senior management attention needed
M: moderate risk; management responsibility must be specified
L: low risk; manage by routine procedures
2025

IFB240

19

Risk management process
Quantitative Risk Analysis: Example

• Quantitative parameters
• Can sometimes obtain numerical values for likelihood
and consequence
• Based on prior knowledge, e.g. industry sector statistics
• Easier to estimate costs for physical items (hardware, etc) than
for other assets (value of files, reputation, etc)

• Where asset value is known (in $$) use
• Asset Value (AV): Estimated total value of asset
• Exposure Factor (EF): % of asset loss caused by threat
occurrence
• Annualized Rate of Occurrence (ARO): Estimated
frequency a threat will occur within a year

in numerical calculations for risk analysis …
2025

IFB240

20

Risk management process
Quantitative Risk Analysis: Example

• Formulae for calculations
• Single Loss Expectancy (SLE)
• SLE = AV  EF
• Expected $value of loss if this event happens once
• Annualised Loss Expectancy (ALE)
• ALE = SLE  ARO
• Expected $value of loss for this event in one year

• USE WITH EXTREME CAUTION
• Results obtained from these calculations are worthless if
based on unreliable or imprecise data

• Sometimes qualitative analysis is more appropriate
2025

IFB240

21

Risk management process
Quantitative Risk Analysis Example

• Calculation example
• Risk description
• Asset: Public image (and trust in organisation)
• Threat: Confidential customer data made public after unauthorised intrusion into
database
• Impact: Reputational damage, cost to repair/replace data, compensation to affected
customers

• Parameter estimates
•
•
•
•
•

AV(public image) = $5,000,000
EF(public image affected by breach) = 0.01
SLE = AV  EF = $50,000
ARO(unauthorised intrusion and public posting) = 2
ALE = SLE  ARO = $100,000

• How much would you be prepared to spend on
controls to deal with this threat?
2025

IFB240

22

Risk management process
Risk Assessment: Step 3. Risk evaluation
• Compare the estimated risk found during risk
analysis with the established risk criteria
• NOTE: Risk analysis and criteria should be on same basis qualitative or quantitative

• Decide which risks need treatment, and when
• Output of this stage: Prioritized list of risks for further
action
• High or extreme risks require immediate consideration
of treatment possibilities
• Risks in low or acceptable risk categories may be
accepted without further treatment
2025

IFB240

23

Risk management process
Risk Treatment (Clause 8 in AS27005:2024)
• Options for treating risk
• Risk avoidance

• Stop doing the activity that gives rise to the risk

• Risk modification

• Apply controls to
• Change likelihood of the event (reduce it)
• Change consequences to reduce the
magnitude

• Risk sharing

• Share with another party that can effectively
manage risk (use a control that modifies
consequence or likelihood, but delegate
responsibility for implementing that to another
party)

• Risk retention

• Know the risk exists, but decide to do nothing –
knowingly retain the risk

2025

IFB240

24

Risk management process
Risk Treatment
•Example: Event – Business email compromise
• Risk avoidance

• Risk modification

• Controls to reduce likelihood
• Physical controls
• Technical controls
• Policy/process controls

• Controls to reduce consequence
• Physical controls
• Technical controls
• Policy/process controls

• Risk sharing

• Risk retention
2025

IFB240

25

Risk management process
Risk Treatment

• Assessing risk treatment options
• Assess options based on the extent of risk reduction, and
any additional benefits obtained
• High risk levels may be acceptable if beneficial opportunities arise
as a result of taking the risk

• Balance the cost and effort of implementing treatment
option against benefits derived (proportionality principle)
• Large risk reductions for low expenditure should be implemented

• May need to use multiple treatment options
• Also, some controls can be applied to treat multiple risks

• Risk treatment itself can introduce secondary risks!
2025

IFB240

26

Risk management process

Level of risk (risk value)

Prioritising risk treatment
implement
reduction
measures

use judgement

?

uneconomic

Cost of reducing risk ($)
2025

IFB240

27

Risk management process
Risk Treatment
• Prepare and implement treatment plans
• Document how the chosen options will be
implemented
•
•
•
•
•
•

Proposed actions
Resource requirements
Responsibilities
Timing
Performance measures
Reporting and monitoring requirements

• Determine the residual risk

• Residual risk = risk remaining after risk
treatments have been applied
• Does this meet organisation’s risk criteria?

• Reiterate risk assessment - including effects
of proposed treatments
• NOTE: Risk treatments can create new risks or
modify existing ones – this is not ‘set and forget’
2025

IFB240

28

Risk management process
Risk communication and consultation phase
(Clause 10.3 in AS27005:2024)

• Communication and consultation
• should be considered at each step of risk management process

• Develop a communication plan for
• internal stakeholders
• external stakeholders

• Two-way dialogue: communication and consultation so all
stakeholders understand
• the basis on which decisions are made
• why particular actions are required

• Stakeholders: those people and organizations who may affect, be affected
by, or perceive themselves to be affected by, a decision or activity

2025

IFB240

29

Risk management process
Risk communication and consultation phase

• A risk statement
• Is a relatively short summary of a risk - usually 2 to 3
sentences
• Used to communicate a risk to stakeholders
• Which stakeholders? - Whoever needs to know
• Usually, hopefully, this includes the risk owner
• Very often this is not an info/cyber sec professional

• For effective communication, the language used for
communication must suit the audience
• What is the definition of risk owner in ISO 27000?
• Check up on this hint: p10
2025

IFB240

30

Risk management process
Risk communication and consultation phase
• Risk statements can be simple or complicated
• A simple risk statement could be formed as:
• There is a risk that <event/incident> occurs
leading to <consequence> that causes <impact>
• Example: Risk statement about business email compromise
• If the audience is a business manager:

• There is a risk that emailed invoice messages may intercepted and
altered during transmission, leading to the message recipient
making their payment to a bank account that does not belong to
our company that causes financial problems for both our company
and our customers

2025

IFB240

31

Risk management process
Risk monitoring and review phase
(Clause 10.5 in AS27005:2024)

• Ongoing review essential to ensure continuing relevance
• Need to monitor
• Identified risks

• Any changes in likelihood or consequence?

• Effectiveness of

• Risk treatment plan
• Risk treatment strategies, and
• Management system controlling the implementation

• Identify emerging risks

• New assets to be included in risk management scope
• Any modification of asset values (value of target to various groups)
• New threats, possibly related to
• increased interconnection of systems
• new technologies

2025

IFB240

32

Risk management process
Risk monitoring and review phase
Q: How does risk change with emerging technologies: Doorbell ?

2025

IFB240

Risk management process
Risk monitoring and review phase
• Example: identifying emerging risks
• The Entire ADF Has Been Banned From Using Zoom Meetings After Hamish Blake Showed Up In One (pedestrian.tv)

2025

IFB240

34

Risk management process
Recording and reporting on the process
(Clause 10.4 Documented Information in AS27005:2024)

• Each stage of the risk management process should
be recorded
• Include in record
• Assumptions, methods, data sources
• Analyses, results
• Reasons for decisions

• Record keeping decisions should consider
• Legal and business needs for records
• Cost of creating and maintaining records
• Benefits of reusing information

2025

IFB240

35

Summary
• Cyber/Info security management is an exercise in
controlling risk
• Should be a controlled process, not ad-hoc
• Risk management relies on having an informed view of the
situation, so appropriate decisions are made

• Guidance on best practice available in standards
• Australian info sec standards you should know about
• AS/NZS 27005:2024 Information Security Risk Management
• AS/NZS 27001:2023 Information security, cyber security and privacy
protection – ISMS Requirements (Outlined in Part B)
• AS/NZS 27002:2022 Information security, cyber security and privacy
protection – Information security controls (Outlined in Part C)

• These are same as ISO standards with these numbers
• Useful for individuals as well as organisations
2025

IFB240

36

