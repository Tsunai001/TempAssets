IFB240 CyberSecurity
Outline solutions for Week 3 tutorial questions for L3: Managing Security

QUESTION 1 - Info Sec Risk Management Process
Use the Australian Standard AS27005:2024 Information Security Risk Management or the Lecture 3 Part A slides to answer the following questions:
a) Give a clear and concise explanation of the main elements of the information security risk management process shown in Figure 2 (on p8) of AS27005:2024 (also included as slide 12 in the Week 3 lecture segment Part A).
b) How is the term 'risk' defined in AS27005:2024 (See Part A slide 5)?
c) How are the terms `consequence' and `likelihood' defined in AS27005:2012?
d) Clause 7 of AS27005:2024 deals with Information Security Risk Assessment (see Part A slides 15 to 23).
i. List the three steps that comprise risk assessment.
ii. Give a brief description of each of the three steps. Note the required inputs, actions and outputs.
e) Clause 10.5 of AS27005:2024 deals with monitoring and review (see Part A slide 30).
i. What should be monitored and reviewed?
ii. Why is monitoring and review necessary?
a) Main elements of the information security risk management process are outlined in Clause 6 Overview and shown in Figure 2 of AS21005:2024.
iii. Establish the context - external, internal and risk management context
iv. Risk Assessment:
i. Identify risks - where, when, why and how events could prevent, degrade, delay or enhance the achievement of objectives
ii. Analyse risks - Identify and evaluate existing controls. Determine consequences and likelihood and hence the level of risk.
iii. Evaluate risks - Compare estimated levels against pre-established criteria and balance potential benefit and adverse outcomes.
v. Decision Point: If risk assessment is insufficient, return to Risk Assessment. Otherwise continue:
vi. Risk Treatment -
i. Assess risk treatment
ii. Decide whether residual risk levels are acceptable
vii. Decision Point 2: If risk levels are not acceptable repeat Risk treatment step for a new treatment, otherwise continue
viii. Communicate and consult across the whole process - with internal (appropriate managers and operational staff) and external stakeholders (could include public relations here)

ix. Monitor and review across the whole process - important for continuous improvement, and to ensure that changing circumstances do not alter priorities.


b) Risk: effect of uncertainty on objectives.
c) Consequence: outcome of an event affecting objectives. Likelihood: chance of something happening.
d) Risk Assessment: the overall process of risk identification, risk analysis and risk evaluation.
Risk identification: the process of determining what, where, when, why and how something could happen
   Input: Scope and boundaries, list of assets owners and users, locations, functions, possible threats, documentation for existing controls and treatment plans, known vulnerabilities related to assets,
   Output: Lists of assets, threats, vulnerabilities and incident scenarios with consequences related to assets and business processes.
Risk analysis: systematic process to understand the nature of, and to deduce the level of risk.

   Input: List of identified relevant incident scenarios with consequences related to assets and business processes, and existing and planned controls.
   Action: Determine business impact on organization resulting from information security incidents, and likelihood of such incidents
Output: List of risks with values assigned
Risk evaluation: process of comparing the level of risk against risk criteria
   Input: List of risks with value levels assigned, and risk evaluation criteria.
   Action: Compare risk levels with risk evaluation and risk acceptance criteria.
Output: List of prioritized risks.
e) Monitoring and review: risks and their factors (asset values, threats, likelihood of occurrence, vulnerabilities) should be monitored to identify any changes. Important because risks are dynamic.

Optional activity for Week 3 relates to AS27005 Annex C. It contains useful stuff: there may be threats here that apply to your situation that you have not already thought of. Read it and see :)

QUESTION 2 - Risk monitoring and review
An article by Gareth Corfield in The Register on 30 July 2020, reported that a device manufacturer, Netgear, had declared more than 40 of the home routers it produced "outside the security support period". That is, Netgear will no longer release software updates for these products, even if vulnerabilities are revealed. Read the article, available online from: https://www.theregister.com/2020/07/30/netgear_abandons_45_routers_vuln_patching/ Consider the information in the article in the context of information security risk management, and answer the following questions:
a) What vulnerability in the routers was revealed by Trend Micro's Zero Day Initiative in June 2020, and, if the vulnerability is exploited by a threat actor, what can occur?
b) How does the decision by Netgear to stop support for these products affect the risk for persons and organisations who are using the affected routers?
c) Explain how this information is relevant for risk monitoring and review. Consider whether other organizational changes, such as a need for staff to work from home rather than on company premises (due to COVID-19 or similar), may interact with this router vulnerability to create emerging risks.

a) There is a stack buffer overflow in the web server's handling of a script which can result in unauthenticated remote code execution with root privileges.
b) The decision to end support for these devices means that there will be no software updates, and any discovered vulnerabilities will continue to be

exploitable while the devices are in use. This increases info sec risks for the users of these products.
c) In risk monitoring and review, changes such as whether information assets have continuing vendor support or not should be noted. Other organizational changes, such as a need for staff to work from home rather than on company premises, should be noted also. The interaction of these two things may be significant - a workplace may not be using these routers on premises, but the employees may be using them in their homes, while performing their work duties. If the vulnerability in a home router is exploited, organizational information assets may be harmed.


QUESTION 3 - Risk Analysis
An article in The Register on 11 April, 2016 reported on the findings of an investigation into user behavior with respect to found USB devices. Read the article, available online from: http://www.theregister.co.uk/2016/04/11/half_plug_in_found_drives/. Use this information to answer the following questions:
a) What did the researchers do with the USBs?
b) What did the users do with the USBs?
c) What percentage of the USBs were subsequently plugged in?
d) Find out about the distribution of malware infected USBs to IBM customers in May 2018. Do you think this delivery method would have a higher or lower success rate than the 'left behind' USBs? Justify your answer.
e) 	When performing risk analysis, both likelihood and consequence may be determined quantitatively or qualitatively.
i. Explain the difference between quantitative and qualitative expressions.
ii. For both consequence and likelihood, give an example of
a. a quantitative scale
b. a qualitative scale
iii. How could the information in the article investigating user behaviour be used to inform risk analysis?
a. Could this be used for quantitative analysis? Under what circumstances?
b. Could this be used for qualitative analysis? Under what circumstances?


User behavior and found USBs:
a) The researchers spread 297 USBs around a University campus. The USBs contained embedded img tags. When the files on the USB were opened the

image was fetched from a remote server that the researchers were monitoring, to track the USBs that users opened.
b) Many of the users who found USBs plugged them in to their computers.
c) 48% of the USBs were picked up and plugged in to a computer. And only 16% of the people who picked up a USB and plugged it in ran a virus scanner over it.
d) IBM Malware distribution:
a. IBM shipped USBs containing an initialization tool for some IBM Storewize systems to customers. In some cases the USB also contained malware. The malware is reported to be the Reconyc Trojan. When the Storewize initialisation tool is launched the malware is copied from the USB onto the machine.
b. This delivery method may have a higher success rate, as people receiving this tool from IBM are likely to trust the company and insert the USB.
e) Risk analysis:
i. The main difference between quantitative and qualitative expressions is that quantitative expressions use numerical values whereas qualitative expressions use words to describe the magnitude of potential consequences and likelihoods.
ii. Example scales:
a. Consequence
* Quantitative: repair/replacement cost in dollars, and
* Qualitative: minor, moderate, major and catastrophic.
b. Likelihood:
* Quantitative: use numerical probability vals: 0, 0.1, 0.2, ..., 0.9, 1.0
* Qualitative: unlikely, likely, highly likely.
iii. The information in the article gives numerical values (48%, 16%) that may be used in quantitative analysis. This is appropriate if the application environment is similar to the test environment. The researchers performed their experiment on a university campus. Perhaps people in other environments are more or less cautious. If there is some uncertainty about how well the research data would estimate behaviour in other environments, then it may be better to use qualitative analysis.

QUESTION 4 - Risk analysis
Suppose the risk management process performed by company ABC produced the following information regarding threats associated with their internet connection:
Threat to assetCost per
incident ($)Annualized Rate
of OccurrenceTheft of equipment50,0002Software malfunction10,0000.10Data corruption due to malicious code100,0000.25
a) Use the information about the threats recorded in the table above to determine the Annualized Loss Expectancy (ALE) associated with each threat event.
b) How much can justifiably be spent on controls to address this risk to the ABC company (if the risk criteria is financial)?
c) Which information security standard provides some guidance on the sort of controls the company could consider applying to treat the risks?

a) Annualised Loss Expectancy (ALE) in $ for each of the three threats is:
I. ALE(T1: Theft) = $50,000 x 2 = $100,000
II. ALE(T2: Software malfunction) = $10,000 x 0.1 = $1,000
III. ALE(T3: Data corruption) = $100,000 x 0.25 = $25,000
b) The spending should be less per year than the ALE, for each of the threats. Keep in mind that there may be some controls which reduce the risk for multiple threats, so the amounts to be spent could be collected. But spending, say, $250,000 in total to address these three risks may be unjustified, given the tabulated data.
c) Look in AS27002:2022 for suitable controls. There are many relevant clauses.


QUESTION 5 - Relationships between standards
For each of the standards documents AS27001:2023 and AS27002:2022, read the preface (on p ii of each document) and note the objective (or refer to Part B slides 10 and 11, and Part C slide 2). Use this information to answer the following questions:
a) How are the standards AS27001:2023 and AS27002:2022 related?
b) Which one of these standards can be used for certification? Note that SAI-Global is the certification body in Australia. (http://www.sai-global.com/).
c) If an organization is certified, or claims to conform to this Standard, what assurance does that give about the management of information security within the organization?

a) AS27001 is the specification for information security management systems (ISMS), a model for setting up and managing an ISMS. AS27002 is the code of practice for information security management. So AS27002 is about the controls you might put in place, the stuff you want to do, AS27001 tells you how to go about managing the process efficiently.
b) Organisations can only be certified against AS27001. They cannot be certified against AS27002, because this is guidance for organisations to make choices relevant to their context, not a system specification.
c) If an organisation is compliant with AS27001:2023, then you are assured that they have an information security management system in place and meet all the requirements in Clauses 4-10 of AS27001. The assurance is that the information security process is managed, not that the organisation is secure. But at least you know they are paying attention to information security :)

QUESTION 6 - AS27002
AS27002:2022 provides guidelines for effective information security management practices. Use Clause 5.1 Policies for information security in AS27002:2022 (or Part C slides 5 to 8) to answer the following questions:
a) Briefly explain the purpose of an organization's information security policy.
b) Locate the Information Security Policy for QUT (in the MOPP, within Chapter F Information Management).
i. What is the stated purpose of QUT's information security policy?
ii. Who does the policy apply to?
iii. What are your responsibilities, as QUT students?
iv. What are the principles that QUT's ISMS is based on?
v. What is the QUT approach to information security classification (which categories are used)?
vi. What might the consequence of a security breach by an individual be (see Section 1.2.8)?

a) The main purpose of Clause 5.1 is 'To ensure continuing suitability, adequacy, effectiveness of management direction and support for information security in accordance with business requirements and relevant laws and regulations.'

QUT's Information security policy forms part of the MOPP, Chapter F/1.2, available from https://mopp.qut.edu.au/document/view.php?id=73 [This is readily available to members of the QUT community and does have definitions, assignment of responsibilities, etc. How many of you have read this and are aware of your responsibilities? QUT may need to link this with user awareness, education and training.]
i. Purpose: 'QUT is committed to protecting its information assets and the information it

holds about its students, partners and employees. The information security policy outlines how QUT protects its information assets against unauthorised access and use, theft, modification, destruction and unauthorised disclosure.'
ii. From Section 2 - Application, 'This policy applies to:

* all of QUT's organisational units (faculties and divisions)
* individuals with access to QUT information assets and resources, including staff, researchers, students and any person to whom the policy on Acceptable use of information and communications technology resources (F/1.11) applies
* all QUT information assets, whether processed by information technology systems or services, or held in physical records sources, regardless of whether or not the processing or storage is undertaken by QUT
* cloud-based services used by QUT
* voice and data communications equipment and software owned by QUT
* research data
* personal equipment connected to the QUT network
* QUT data in transit.

iii. As QUT students, your responsibilities will include those in the table in Section 3 - Roles and Responsibilities for the position of 'All users'
iv. QUT's Information security principles (from Section 5): Direct quotation

* Logical access and physical access security
Logical access and physical access to QUT information assets is granted on the "least privilege" principle, whereby each user is granted the most restricted set of privileges needed for the performance of relevant tasks.
* Information security risk management
Information security related risks must be identified, reported to concerned stakeholders and adequate controls are recommended to manage the risk.
* Operational security
Operational security practices must be in place to manage information security related risks.
* Information security incident management
Information security incidents must be actively managed in a defined manner in line with QUT's incident management process.
* Information classification
Information maintained in QUT's information systems and in printed format is protected based on the assigned information classification level (F/1.2.5).
* Audit and Compliance
The established information security management processes must be conducted in line with regulatory requirements and be regularly audited to promote improvements in practices.
* Human resource security
QUT must have processes in place to screen candidates, on-board and off-board employees, and educate employees on security awareness.
These principles assist in governing behaviour, objectives, approach and activities, in order to promote good practice in information security. The Vice-President (Digital) and Chief Digital Officer approves information security standards which further explain the implementation of the information security principles and define the information security controls.
v. QUT's approach to information security classification offers these

categories:

* Confidentiality measures the risk of information made available or disclosed to unauthorised individuals, entities, or processes, as either High (Protected), Medium (Sensitive), Low (Official), or Public information or data.
* Integrity measures the risk to the accuracy and completeness of information or data, as either High, Medium, or Low.
* Availability measures the risk of data accessibility on demand by an authorised entity, as either High, Medium, or Low.

vi. Consequences of security breaches are outlined in Section 8 - Security breaches: 'Serious breaches of information security by an individual user may result in disciplinary action (for staff and students) or the suspension or termination of access rights and computer accounts in accordance with the Acceptable use of information and communications technology resources policy (F/1.11). This policy supports and complements State and Commonwealth laws. Illegal access to and use of computer systems at QUT may constitute a criminal offence under the relevant legislation. Breaches of information security which are also suspected of breaching State or Commonwealth laws will be reported to law enforcement authorities for appropriate action.'

[These risk management concepts, and an information security classification framework considering Confidentiality, Availability and Integrity, with risk ratings assigned to each (Mostly these are High, Medium and Low risk) are relevant for your Assessment task 2: Risk Report.]

QUESTION 7 - AS27002
Read the story of the stolen law enforcement officer's laptop at: : Stolen laptop containing info on victims, suspects, witnesses and police - Help Net Security.
a) Based on the article, identify:
i. The information assets involved.
ii. Plausible threats to the sheriff's office information assets.
iii. Potential attacks.
iv. Possible consequences if the potential attack occurs.
b) Could these consequences lead to subsequent events (chain of events)? Explain or give examples.
c) Combine an example of a threat, a vulnerability, an event, an incident, and at least two consequences to make a risk statement. Suppose the context is that you work for a law enforcement agency and need to convey a risk about the use of mobile devices to a superior officer. Write your risk statement by putting the items in this order:
Event/incident, consequence, impact.
[The impact could be on the individual officer, on the organisation (sheriffs office) or

on other stakeholders (witnesses, informants, ...]
Here is an example risk statement from an individual officer perspective:
There is a risk that a laptop belonging to an officer will be stolen, and the information contained will be accessed by unauthorised individuals. As a result, the confidentiality of the investigation documents stored in the laptop will be compromised, and the officer's undercover position will be exposed. The officer may be in considerable physical danger as a result.

i. Write a risk statement for this sheriff's office scenario from the organisational (sheriff's office) perspective.
ii. Write a risk statement for this scenario from a police informant's perspective.

d) Taking a qualitative approach to risk analysis, use a risk matrix similar to that given in Lecture 3 Part A slide 19.
a. Determine the risk level for each of the risks you identified.
b. Which would you prioritize for treatment?
e) Now read through Clause 6.7 Remote working in AS27002:2022 (or refer to Week 3 Lecture Part C, slide17 for approximate contents). Considering the undercover detective's role, suggest some security measures that, if implemented correctly, may have prevented this incident, or at least minimized the damage (or make your own suggestions if you have difficulty accessing AS27002).

a) From the article:
a. Information asset is a laptop and personal hard drive full of case file data, belonging to a detective from the Sheriff's office. The data was not encrypted.
b. Plausible threats to the info on the sheriff's computer:
i. Unauthorised disclosure of information (breach of confidentiality)
- the person who stole the laptop containing unencrypted case files could access the files and read the content. Case files contain lots of personal information (names, licence numbers, social security numbers), witness statements, etc
ii. Unauthorised modification (breach of integrity) - the person who stole the laptop could possibly modify information in the files.
iii. Breach of availability - already occurred - as the undercover detective no longer has access to the device or the information it contained.
c. Potential attacks: The threats outlined above could easily be realized.
d. Possible consequences if the attack occurs:
i. Unauthorised disclosure of a large amount of sheriff's office information
1. compromises current investigations.
2. undercover detective exposed as a detective (so cover is blown) - may put detective in personal danger.

ii. Modification of information - consequence is compromise of the investigation. May have changed event details, suspect information etc. Data on this stolen device could not be trusted if the device were recovered.
b) Consequence of one event could be another event:
i. If confidentialty is breached,
1. the personal information recorded in the case files could be used for subsequent identity theft, with those persons becoming vicitms.
2. the information could be used to identify persons connected to a particular case, and they may be targeted for case- related reasons (pressured to alter or retract a statement, etc) ...
c) Risk statements:
i. There is a risk that a laptop belonging to an officer will be stolen, and the information contained will be accessed by unauthorised individuals. As a result, the confidentiality of the investigation documents stored in the laptop will be compromised, and the information may be made available to criminals. Several ongoing investigations will be disrupted as a result. Further, this may discourage other persons from providing information to our officers and agents.
ii. There is a risk that a laptop belonging to an officer will be stolen, and the information contained will be accessed by unauthorised individuals. As a result, the confidentiality of the investigation documents stored in the laptop will be compromised, and the names of police informants and details of the information they provided will be exposed. The informants may be in considerable physical danger as a result.

d) Risk matrix: For the identified risks, try to determine the risk level (place in table)

LikelihoodConsequenceInsignificantMinorModerateMajorHighMHEEMediumMMHELowLMMHUnlikelyLLMM
e) Yes, this question is asking you to look in the standard for possible control measures, or if you don't have access to the standard, to suggest some controls that you think would help. Be prepared to justify your choices. To prevent the incident or minimize the damage, these choices may include:

i. Requirements for physical protection of the laptop (Why was it left in unlocked pickup?)
ii. Access controls (Why no lockscreen?)
iii. Use of cryptographic techniques (encrypt sensitive data in storage - we will discuss crypto later in the semester)
iv. Remote disabling, erasure or lockout (to wipe data once you realize device is lost)
v. Backups (so you have something to refer to, you can regain access to the stored information, which will help in identifying what was on the device and is now potentially exposed).
Do you work remotely? Which of these control measures have you applied on your own mobile device?


QUESTION 8 - AS27002
A major data breach occurred at credit monitoring firm Equifax in 2017.
a) Read the following news story concerning the data breach at: https://www.csoonline.com/article/3444488/equifax-data-breach-faq-what-happened- who-was-affected-what-was-the-impact.html. Use the information in the story to answer these questions:
i. What sort of data was compromised?
ii. How many records are thought to be involved?
iii. How did the data breach occur?
iv. When did the data breach occur?
v. When did the Equifax notify consumers about the incident?
b) As part of their response to the incident, Equifax set up a site to provide information on the breach and to enable consumers to determine whether they were affected by the breach. However, , the following article describes a few problems with this process: EPIC - Equifax Data Breach. Read the Equifax response and criticisms section of and list the things that Equifax (or other organisations) could learn from this to improve this aspect of their incident response for future events.
c) In the standard AS27002:2022, Clause 5.26 deals with Response information security incident management. If you have access to AS27002:22, consider this clause - which aspects are relevant to the Equifax case? Justify your answer.

a) Equifax data breach info:
i. The compromised data was consumer names, social security numbers, birthdates, addresses and driver's license numbers, and some credit card numbers.

ii. Breach is information on 143 million American consumers, and around 400,000 British consumers.
iii. Breach is thought to occur as a result of deliberate action by external attackers. The attackers found vulnerabilities in the website software Equifax used on a web page for dealing with disputes on the accuracy of the credit monitoring information.
iv. The attackers exploited the vulnerability and were in the Equifax network between mid-May until July 29 when the intrusion was detected and stopped.
v. Equifax notified consumers that their data had been compromised on September 7, 2017.
b) Equifax incident response and the consumer information website: possible improvements for future responses
a. Use a domain name that is directly linked to the company - this is where consumers are likely to look and has trust associations.
b. Don't use a name that looks like it might be a phishing site trying to capitalize on the incident. If you do, phishing sites will try to capitalize on that.
c. 	If you post or tweet the consumer information website URL, check that the URL you provide is the actual site you set up and not an imposter site.
c) Clause 5.26 includes
* Control: Information security incidents should be responded to in accordance with the documented procedures.
* Purpose: To ensure efficient and effective response to information security incidents.
* Guidance:
The organization should establish and communicate procedures on information security incident response to all relevant interested parties.
Information security incidents should be responded to by a designated team with the required competency

The response should include:
a. Containing, if the consequences of the incident can spread, the systems affected by the incident,
b. Collecting evidence as soon as possible after the occurrence,
c. Escalation as required - including crisis management activities ...
d. Ensuring that all involved response activities are logged for later analysis
e. Communicating the existence of the infosec event with relevant internal and external parties following need-to-know principles
f. Coordinating with relevant internal and external parties following need- to-know principle
g. Once incident is successfully addressed, closing and recording it
h. Conducting info sec forensic analysis
i. Perform post-incident analysis to identify the cause
j. Identify and manage the vulnerabilities and weaknesses including those related to controls that caused, contributed or failed to prevent the incident.

Equifax should look at what they could learn from this incident -
* About how to avoid the incident:
o the software vulnerabilities that the attackers exploited which could have been patched,
o the attacker being able to access the 'crown jewels' database from a web dispute page exploitation when other network architectures may have afforded better protection, ...
* Also how to respond when an incident does occur: to avoid the info website issues.
o What were their documented procedures?
o Did they follow them?
o How could this be more effective?
