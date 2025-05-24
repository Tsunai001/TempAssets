IFB240 Cyber Security
Lecture 4 – Part A
Identity and User Authentication
or

Who are you?
and

How can I be sure of that?
Dr Leonie Simpson
lr.simpson@qut.edu.au
2025

IFB240

1

Why is identity management important?
• Classic Peter Steiner cartoon
from 1993
–

Image from:
https://img.washingtonpost.com/rf/image_148
4w/WashingtonPost/Content/Blogs/comicriffs/StandingArt/STEINERinternetdogs.jpg?u
uid=Cn7v6vmREeKOhMVnMaIC-w

• Q: When/why is it important to
know who (or what) you’re
interacting with?
– Consider both physical and
logical (electronic) scenarios
– Consider both
• user and
• system

perspectives and requirements
2025

IFB240

2

Why is identity management important?
Optus: How a massive data breach has exposed Australia - BBC News

• Optus data breach - Sept 2022
– Personal data of approx. 10
million customers stolen
– Data sample published online
– Attacker demands $1 million to
avoid release of remaining data

• Optus statement:

• Alleged attacker’s statement:

2025

IFB240

3

Why is identity management important?
• Q: Why does it matter who (what) you’re interacting with?
•

https://www.threatdown.com/blog/150000-verkada-security-cameras-hacked-to-make-a-point/

2025

IFB240

4

Why is identity management important?
• Identity is important if decisions about
interactions are based on it
– Deciding whether to provide access to a resource
• Mechanisms use identity to determine if specific access
requests should be permitted
– Recall the Vishing episode where the phone account
password was changed?

– Holding users accountable for actions they take
• If user actions are logged and monitored, need to be sure the
actions were performed by that user
– and not by someone else
if you intend to hold the user accountable for their actions
2025

IFB240

5

What is user authentication?
• Process used to decide whether the identity a user
claims is genuine (authentic) or not
• Need to have
– A unique identifier for each individual
– A way to verify the identity as authentic
• This verification process is called user authentication

• Example: QUT Login
– Student/staff member
1.
2.
3.
2025

provides identifier (username)
provides password to validate identity claim
QUT system evaluates info & decides Y/N
IFB240

6

What is user authentication?
• User authentication is important if decisions are based
on user identity – for example, access control processes
Identification

Q: Who are you?
A: Claim an identity: provide User ID

Q: Is it really you?
Authentication

Authorization
2025

A: Provide credential to validate claim,
Have a process to check validity

Q: Are you allowed do this?
A: Check system records to determine
whether user is authorized to perform
requested action (more on this Week 6)
IFB240

7

User authentication fundamentals
• Systems to authenticate users need to
– Consider
1. user identifier(ID) and
2. provided authenticator

– Decide whether user claim is authentic or not

• Important characteristics
– User identifiers must be Unique and Public
– Authenticators must be something only an authentic
user could provide
– Need resources to manage decision process
• Compare provided authenticator with expected authenticator
• May need stored values to enable comparison
2025

IFB240

8

User authentication fundamentals
• Consider security implications
– For local and remote authentication
• Local authentication requires provision of
details at decision point
– Is this secure – no shoulder surfing or
eavesdropping?

• Remote authentication requires transmission
of details from user to remote system
– Is this information secure at point of entry?
– Is this information secure during transmission?
2025

IFB240

9

User authentication fundamentals
• Consider security implications
– For both user and system verifying
authenticity
• User has responsibility to maintain security of
their credentials (think CIA here)
• System has responsibility to
– maintain security of all stored values used for
authentication (for all users)
– perform comparison and make decisions on
authenticity
2025

IFB240

10

User authentication fundamentals
• Authentication mechanisms make use of different types of
authenticators - user authenticators categorised as
– Knowledge-Based
• Something you know (should be a secret only the entity knows)
– Object-Based
• Something you have (physical item only the entity possesses)
– ID-Based
• Something you are (physical characteristic of person - biometric)
– Location-based
• Somewhere you are (data item that connects to a specific
location)

• Multi-factor authentication
– uses combinations from multiple different categories
2025

IFB240

11

Summary
• User authentication
– Process used to decide whether the identity a user claims is
genuine (authentic) or not

• Important to ensure authentic users if identity is used for
– Access control decisions
– Accountability measures

• Different categories of authenticators
– Most commonly used is Knowledge based – Passwords (in Part B)

• Advantages and disadvantages
– For different types of authenticators & for multifactor authentication
– Cost, resources, level of security provided, user acceptability, etc

• Security requirements for both user and system
– Actions of both contribute to overall security of both
2025

IFB240

12

