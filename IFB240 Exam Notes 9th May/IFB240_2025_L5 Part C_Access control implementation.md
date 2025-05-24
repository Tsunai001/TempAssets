











IFB240 Cyber Security
Lecture 5 - Part C Implementing access control
Dr Leonie Simpson
lr.simpson@qut.edu.au


• Access control is controlling or restricting the use of information assets and/or resources to
- Allow authorised users access to information resources they need to perform their tasks
- Prevent authorised users from misusing resources, and
- Prevent unauthorised users gaining access to resources
• Major access control approaches include
- Discretionary
- Mandatory
- Role-based
• But how does this get implemented in organisations?


• How will the access control policy be implemented?
- Just having an access policy is not enough
• Users may not abide by it
- Need to put control mechanisms in place to enforce the policy
• To do this, first need to create user accounts
- Associate privileges for resources with users (or groups of users)
- For accountability, each user should be uniquely
identifiable
- To implement a system where some subjects are permitted to access a restricted resource, need to be sure that subjects are authentic when deciding whether to allow access requests
• User authentication required (Discussed in Week 5 lecture)


• Is there guidance on this in the standards?
- AS/NZS 27002:2022 Clause 5 Organizational Controls includes multiple sub-clauses dealing with aspects of this - some of these are:
• 5.15 Access control
- Purpose: to ensure authorised access and prevent unauthorized
access to info and associated assets
• 5.16 Identity management
- Purpose: to allow for the unique identification of individuals and systems accessing the organizations information and other associated assets and to enable appropriate assignment of access rights
• 5.17 Authentication information
- Purpose: To ensure proper entity authentication and prevent failures of authentication processes
• 5.18 Access rights
- Purpose: to ensure access to information and other associated assets
is defined and authorized according to business requirements


• Two phases of access control
1. Policy definition phase where privilege is allocated and administered
a. Authorise subject by defining the AC policy
b. Distribute access credentials/token to subject
c. Change/revoke authorisation whenever necessary
2. Policy enforcement (grant access) phase* where privilege is required to gain access
a. Authenticate subject
b. Grant access as authorised by policy
c. Monitor access
*	(note: sometimes the term "authorisation" is used for this phase)




Implementing access control
Access control phases - conceptual diagram



Legend	PAP: Policy Administration Point		AC policy definition phase PEP: Policy Enforcement Point	AC policy enforcement phase

Implementing access control
• Phase 1- Administration of privileges
• How are users informed of their access privileges?
- Which assets does the user have access to?
• Physical assets - buildings, rooms, printer/photocopier, telephone
• Electronic assets - files, systems
- What sort of access does the user have?
• And the limitations of their access privilege
- Access only certain buildings/rooms, certain times,
- Restricted access e.g. local phone calls only
- Restriction on type of access to data files: read-only access,
write, append, etc

Implementing access control
• Phase 1- Administration of privileges
• How are users informed of their access privileges?
- Are there conditions on use of privileges?
• Limitations on disclosure of protected data,
• Restrictions on actions such as making copies of files
• How to handle unauthorized requests for access, etc
• Disciplinary consequences of violation of privileges
• Action to be taken if a security incident occurs
- Plan ahead for foreseeable incidents
• Reporting procedures for security incidents
- Who to report to,
- What to report,
- Format or template for details

Implementing access control
• Phase 1- Administration of privileges
• Is the handover of the means to exercise the privileges secure?
- Hand over to the intended recipient
• Check identity
- And only to the intended recipient
• Security of handover phase
• Consider process for access control measure that is:
- physical
• ID badge, uniform, door key, magnetic swipe card
- logical
• password, PIN, response

Implementing access control
• Phase 1- Administration of privileges
• How are details of users and privileges recorded?
- Are the records secure from illicit disclosure or modification?
    • Would the records be acceptable in a legal challenge?
- Can you easily identify privileges associated with
• a particular user?
• a particular resource?
• How will the privileges be withdrawn if/when required?
- Is there an expiry time of the privilege?
- Is there a procedure for automatic revocation under certain conditions?
• Example: on termination of employment
- Who needs to be informed of the withdrawal of a privilege?
• User, Administration, Security

Implementing access control
• Phase 1- Administration of privileges
• Process regarding withdrawal of privileges if required
- Are there procedures for
• the user to hand back the privilege?
• the privilege be withdrawn without the cooperation of the user?
- Often harder to revoke physical access control than logical
- Can the user prove that the privilege has been withdrawn or handed back?




Implementing access control
Access control phases - conceptual diagram



Legend	PAP: Policy Administration Point		AC policy definition phase PEP: Policy Enforcement Point	AC policy enforcement phase



• Phase 2 - Policy enforcement
• Objective is to prevent unauthorised access, so
- before a subject is given access to a resource,
- want some assurance that they are authorised for the requested access

• How will we know if a subject is authorised?
- First, need assurance on who the subject is
• Identification: the subject claims an identity
• Entity Authentication: the process of proving (validating or verifying) the subject holds the claimed identity
- Examples
" You announce who you are, and show your ID card
" You provide a user ID, and the corresponding password
- Then system checks if that subject is authorised for the requested access (set up in Phase 1) before granting access


• Phase 2 - Policy enforcement
• Identification, authentication and authorization


Who are you? Provide user ID

Is it really you? Provide credentials


Are you allowed to access this resource? In what mode? Check system records


• Phase 2 - Policy enforcement
• Identification and authentication of users important for
- Access control
• User identity is used to determine whether to permit access to resources
• Do not want
- To permit unauthorised access, or
- System that allows attackers to masquerade as legitimate users
- User accountability
• User identity is recorded in logs of events, used for auditing
• Want users to be assured that
- their actions are logged and they will be held accountable
- the process does not permit masquerade attacks (which could result in users being held responsible for actions of an attacker)


• Phase 2 - Policy enforcement
• Authorization is performed by checking that a subject does have the required permissions to access the object, in the requested mode
- Could be recorded in an Access Control List (ACL)
- Could be through use of defined Roles

• Note that the user authentication and authorization checks should be performed for each access request




Implementing access control
Access control phases - conceptual diagram



Legend	PAP: Policy Administration Point		AC policy definition phase PEP: Policy Enforcement Point	AC policy enforcement phase

Implementing access control
-Loopholes permitting unauthorised access
Example: Matthew Garrett journal entry http://mjg59.dreamwidth.org/40505.html





• Monitoring is important for
- detecting unauthorized activities
• detecting access control loopholes
• identifying security incidents
- providing evidence of security incidents,
and
- providing a model of normal system behaviour
• Used for detecting some attacks (Intrusion Detection Systems)



• Monitoring can help detect access control loopholes permitting unauthorised access

• Picture from http://www.syslog.com/~jwilson/ pics-i-like/kurios119.jpg

Implementing access control
-Loopholes permitting unauthorised access
Example: https://www.forbes.com/sites/thomasbrewster/2018/06/13/tapplock- smart-lock-hacked-in-2-seconds/#1350c28b1333

Loopholes permitting unauthorised access

• Example: Exposed access token allowing access to Shopify
• #1087489 Github access token exposure (hackerone.com)

Loopholes permitting unauthorised access

• Example: Vehicles
- Smart keys & car crime
- The Guardian
- 25 February 2024
- Gone in 20 seconds: how 'smart keys' have fuelled a new wave of car crime | Motoring | The Guardian

Summary
• Access control is important for information security
• Need to consider how to
- Make access control policy decisions
- Enforce access control policy using control measures
• Both physical and logical measures
• Monitoring required
• Implementing access control - two phases to consider
- Policy definition phase
- Policy enforcement phase
• User authentication is important,
• Both user and administrator actions affect the security of this
- Need to monitor access - it may not work as you expected!






























































