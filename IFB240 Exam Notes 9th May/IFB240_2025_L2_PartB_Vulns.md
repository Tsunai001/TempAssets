IFB240 Cyber Security
Lecture 2 - Part B
Vulnerabilities
Dr Leonie Simpson
lr.simpson@qut.edu.au

2025

IFB240

1

Vulnerabilities
• Characteristics of, or weaknesses in, a system
– that, if acted on by a threat, could cause harm to
information assets

• Consider the components of information system
– Property

People

Data

– People
– Procedures

Procedures

Hardware

Software

• Vulnerabilities exist in all of these
2025

IFB240

2

Vulnerabilities
• Property includes
– Physical assets: buildings and contents
– Hardware: computer systems, data communications
devices, data storage devices
– Software: Operating system, applications
– Data: System and organisational data: files,
databases, passwords, …
• Consider possible vulnerabilities for each
– This list is not exhaustive, just some of the possibilities…

2025

IFB240

3

Vulnerabilities
Property – physical assets
• Aspects to consider include
– Location of information assets
• In a geographical area that is:
– Susceptible to natural disaster
– Near storage of flammable or corrosive materials
– Close to targets for disruption (may be collateral
damage if neighbouring building is target)
embassy, military site
– Easily accessed by outsiders?

– Physical security mechanisms
• Fences, walls, locks, gates, partitioning of internal
space
2025

IFB240

4

Vulnerabilities
Property – physical assets
• Example: India, February 2024
fireworks factory explosion
Eight Dead, 80 Injured in India Firework Factory
Explosion (voanews.com)

2025

IFB240

5

Vulnerabilities
Property – physical assets
• Aspects to consider include
– Maintenance
• Is asset in working condition?
• Is perimeter protection maintained?

– Monitoring and logging physical access
• Use of suitable equipment for monitoring access to facilities
and environmental conditions
– Examples:
» CCTV, Intrusion Detection/Alarm system,
» Fire detection and automatic fire suppression
system, etc
• Do these depend on other systems – telecommunications, etc?
2025

IFB240

6

Vulnerabilities
• Property – ICT hardware and software
• Aspects to consider include
– Reliability and robustness of
• Asset
– Susceptibility to environmental conditions (dust, heat, humidity)

• Supporting infrastructure
– Power supply, air conditioning, etc.

– Redundancy
• What happens if/when equipment fails?
• Is there sufficient alternative resources?
– Uninterruptible Power Supply (UPS),

• What fail state does equipment revert to? (Open/closed?)
2025

IFB240

7

Vulnerabilities
• Property
– ICT Hardware and
software
• 2019/2020 Bushfires

• Mobile phone coverage
dependent on power
supply
• Powerlines destroyed in
fires
• Significant loss of
services
2025

IFB240

8

Vulnerabilities
Property – ICT Hardware and software
• 2022 Floods

• Significant loss of
services
•

2025

What is happening with
telecommunications in
flood-hit regions of
Queensland and NSW |
ZDNet

IFB240

9

Vulnerabilities
• Property – ICT hardware and software
• Aspects to consider include
– Source of software: authorised, legitimate, vendor
supported?
• Still using Windows XP?
Vendor support ended in 2014
• Still using Windows 7?
Vendor support ended Jan 2020
• There will be no updates to correct vulnerabilities in software

– Downloading and installing: what is permitted?
• Can users install whatever software they like, obtained from
wherever they like?
• What processes are followed?
• Could install software containing malware 
2025

IFB240

10

Vulnerabilities
• Property – ICT hardware and software
• Consider aspects including
– Design, creation and testing of software
• There are often flaws (bugs) in software
– Example: common input problems: buffer overflows, injections

– Possible that an attacker may exploit this

– Need for patching and upgrading
• Patch: Vendors make changes to software to correct bugs, and
make the updated code available
– Needs to be installed to be effective

• How soon should the update be installed once it is available?
– ACSC Annual Cyber Threat Report 2022 (p60) notes: ‘The time
between vulnerability disclosure and exploit is closing rapidly; what once
took weeks is now taking days or even hours.’

• Are there other systems that may be impacted by an update?
(dependency and compatibility issues)
2025

IFB240

11

Vulnerabilities
• Property – ICT hardware and software
• Consider aspects including
– Configuration/misconfiguration
• Has the system been implemented and set up appropriately?
• Has the setting been changed from the default setting?
– Is the default setting secure?

2025

IFB240

12

Vulnerabilities
People - Lack of awareness of threats
• Example - vulnerable to social engineering
– ACSC defines social engineering as
• ‘The methods used to manipulate people into carrying out specific
actions, or divulging information.’
– Lack of awareness that this occurs makes people vulnerable
– ACCC Scamwatch figures:
– 2024 Phishing statistics:
• Amount lost: $20, 510,354
• Number of reports: 97,831

2025

–

Source:

–

https://www.scamwatch.gov.au/research-and-resources/scam-statistics

IFB240

13

Vulnerabilities
People – within organisations
• Example: Employees
– Recruiting staff suitable for the position
• Failure to check background is common

– Monitoring access of people to property & processes
• Disgruntled employees, clients or contractors can be
exploited or threat source

– Inadequate training and awareness of staff re threats
- for example, are staff aware of policies regarding
•
•
•
•
2025

providing information by email or over phone
downloading software
configuration of product
checking publicity photos before release, etc
IFB240

14

Vulnerabilities
• Example: People – recruiting failure

2025

IFB240

15

Vulnerabilities
• Example: People – recruiting failure
– Source: Brisbane Business News - January 2012

2025

IFB240

16

Vulnerabilities
People – within organisations
• Example: People – lack of training and awareness –
software download
•

A student pirating software led to a full-blown Ryuk ransomware attack (bleepingcomputer.com)

2025

IFB240

17

Vulnerabilities
People – within organisations
• Other aspects to consider include
– Employees
• Are there key personnel critical to organisation’s operation?
– May be unavailable due to accident or illness, or other
event (transport failure, natural disaster, lotto win ☺)
– May be uncooperative
• Vulnerable if no back-up for these people
– Especially if procedures they perform are undocumented

– Others
• Are security conditions included in contracts with consultants,
contractors, outsourcing?
2025

IFB240

18

Vulnerabilities
Processes used
• Aspects to consider include
– Access control and privilege management
• What are the processes used for managing these?
• Including keys, ID cards, passwords, …

– Backup of files and systems
• Who does this?
• When/How often?
• Where are these stored? Encrypted storage or not?

– Business continuity plans
• For recovery of information assets after disaster
• There is a plan, right?
– Who knows about it? Has it been rehearsed? Is there a drill?
2025

IFB240

19

Vulnerabilities
Processes used
• Aspects to consider include
– Communications
• What is the acceptable use policy for communications systems
– Example: confirmation for sending/receiving messages
» Will you know if a message has been misdelivered?
• Does it matter what the message is?
– Is it OK to email a new password to someone? Or should a
different process be used?
– Is it OK to login to a website using http and provide a PIN?
– What about PIN for ATM card? Can that be sent in email?

– Example: Passwords - see plaintextoffenders.com
2025

IFB240

20

Vulnerabilities
• Example: Communications
processes
• How do you join a Zoom meeting?
Do you
1.
2.

Go to Zoom, enter meeting ID and
password? OR
Click on the link in the Zoom invite?

• Why does this matter?
• Source: NZ Herald, 24 November
2020
•

Fake Zoom invite warning: The click that cost a hedge fund $8.7
million - NZ Herald

2025

IFB240

21

Vulnerabilities
Processes used
• Aspects to consider include
– Checks and balances
• People make mistakes: are there processes to detect, correct
or reduce the impact of errors?
– Example: Separation of duties

– Processes associated with staff joining/leaving
organisation
• Clear statement of duties
• Nondisclosure/confidentiality agreements

– Software management processes and auditing
• Application whitelisting?
2025

IFB240

22

Vulnerabilities
• Example: Is there a process to detect when people make
mistakes?
•

Source: https://www.news.com.au/finance/work/at-work/a-major-financial-accident-samsungemployee-makes-140-billion-fat-finger-mistake/news-story/7c927c899c9a534ba8a82c63ccff34ba

• Paying dividends
– to employees owning shares

•

Dividend payment error:
– Instead of 1000 won per share
issued dividend equal to
– value of 1000 shares per share

2025

IFB240

23

Summary
• For information assets and their support systems
– Many threats
– Many vulnerabilities

• To protect information assets, need to understand
–
–
–
–
–
2025

What the asset is, where it is, what the value is
Possible threats
Existing vulnerabilities
Likelihood of threats and vulnerabilities coinciding
Potential consequences if that does happen
IFB240

24

