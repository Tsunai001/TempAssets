IFB240 Cyber Security 2025
Outline solutions for Week 1 Tutorial - Introduction to cyber/information security

Essential definitions: Review the de?nitions given in the lecture segments for the following terms. We will use these terms repeatedly across the semester. You should be able to define these terms and be able to apply the terminology correctly in situations and scenarios. These will be assessed in Assessment tasks 1-3.


Cyber SecurityEntity AuthenticationInformation SecurityData Origin AuthenticationAssetNon-repudiationCon?dentialityVulnerabilityIntegrityThreatAvailabilitySecurity IncidentInformation StateAttack

Tutorial questions: These tutorial questions are intended to stimulate thinking about aspects of security and provide opportunities to apply the terminology. Attempt these questions before you attend your tutorial session and have your prepared answers with you in the tutorial. Be ready to discuss your answers and/or any problems you experienced when trying to answer these questions. Your tutors look forward to discussing this with you during the tutorial.

QUESTION 1
A security breach at Red Cross Blood Service Australia is described in an October 2016 blog article by Troy Hunt, available from: https://www.troyhunt.com/the-red-cross- blood-service-australias-largest-ever-leak-of-personal-data/. [This was the Australia's largest breach of personal information at the time, but in recent years there have been several much larger breaches.] Read the article, and review the "cube" from the NSTISSI 4001 security model (at the end of the Week 1 Part C lecture segment) to answer the following questions:
a) Which Red Cross Blood Service information assets were involved (what sort of information and how much of it)?
b) What is the data state of the compromised information: is the data in transmission, in storage or being processed?

c) Which of the following security goals were compromised? Explain your answer.
i. con?dentiality
ii. integrity
iii. availability
d) Would this be considered an attack? Explain your answer, considering both the threat and vulnerability.
e) After this incident, how could the compromised information be used by others outside of the company in subsequent events?
f) Could this incident have been prevented? Would control measures involve the use of technology, policy and procedures, or education/training/awareness? Explain your answer (it can be more than one of these things).

a) Compromised asset is data: 1.3M records of blood donors. Some had multiple entries, so estimate is records of around 550,000 people. Data contained in the record is personal information including:
i. First name
ii. Last name
iii. Gender
iv. Physical address
v. Email address
vi. Phone number
vii. Date of birth
viii. Blood type
ix. If they'd previously donated
x. Country of birth
xi. When their record was created
xii. The type of donation (Plasma, Plasmapheresis, Platelet, Plateletpheresis, Whole Blood)
xiii. When each donation occurred
xiv. Donor eligibility answers (On antibiotics, over or under weight, risky sexual behavior, etc)


b) The data state: storage. This was intended as a backup for the database.
c) Confidentiality is compromised. This is personal information and the data

should have been for authorized Red Cross use. However, the database backup was placed on a publicly facing website. This information has been disclosed to unauthorized people. Troy Hunt and the person who noticed the data was available and passed it on to him, are both unauthorised viewers of the data. It is not certain whether there are others who have seen it.
d) This is not an attack - it is the result of careless behavior of an employee of the Red Cross partner firm who were looking after the data. However, it is still a very serious incident, for Red Cross and for the individuals whose data has been exposed.
e) The information could be used by malicious outsiders for many purposes, including identity theft and extortion.
f) The incident could have been prevented. The database backup should be stored with the same security considerations as the database itself. It should not be publicly accessible. The information could have been encrypted (technology), there may be organizational policy regarding the security requirements for stored data of this type, and the employee of the Red Cross partner firm responsible for the backup could have been trained in appropriate procedures.

QUESTION 2
A ZD Net article (March 13, 2017) by Steve Ranger reports on the findings of simulated phishing	attacks	performed	via	email	to	employees	of	various	companies: http://www.zdnet.com/article/phishing-would-you-fall-for-one-of-these-scam-emails/. The researchers sent emails with attachments or with embedded links. Read the article to answer the following questions:
a) What sort of information do the phishers usually try to obtain from the recipients?
b) What types of lures did the researchers use, and which were most effective?
c) Which of the following security goals were compromised when this information was provided? Explain your answer.
i. con?dentiality
ii. integrity
iii. availability

d) Following the initial compromise, how could the information obtained by the phishers be subsequently used? (Describe a chain of events)
e) What is the vulnerability being exploited in these attacks?
f) What sort of control measures could be used to address this: the use of technology, policy and procedures, or education/training/awareness? Explain your answer (it can be more than one of these things).

a) Phishers try to obtain credential information such as usernames and passwords for accounts.
b) The lures used in the phishing emails were asking the recipient to download an invoice, secure their email, complete a HR appraisal, offering a discount voucher or sending a friend request. The friend request was the most successful; almost 24% of respondents clicked on this.
c) The security goal compromised when credentials such as passwords are disclosed to phishers is confidentiality.
d) There are many possibilities. Following the initial compromise, the attackers may use the obtained information to log in to the user account and then take additional actions - depending on the account, they could read email, delete it, perhaps install and run programs on the user's device, etc. (Chain of events, where one attack provides input to the next: Phishing provides details used in subsequent attacks ...) Or they may sell the information to other criminals, who could use it similarly.
e) The vulnerability is the user who is tricked into thinking the email is authentic and follows the instructions in the email.
f) User training and awareness is important, so users recognize warning signs for phishing. Policy and practice can help with this too. For example, knowing that your company would never request your login details by email, a request for those details should raise suspicion. Also knowing what to do when you do receive an email like this (is there a policy to report it, are users aware of this, and do they know who to report to - IT Security, Helpdesk, ?? and the reporting method - do you ring up, forward the email, ...). Technology can be used - monitoring servers, mail filtering, stripping off attachments or disabling links, etc.

QUESTION 3
In December 2022, QUT experienced a serious cyber security incident. You can read about this on QUT's site here: QUT - Cybersecurity incident
and also in external media reports, such as the ABC news article on 22 December by Lilian Rangia, available here: Queensland University of Technology shuts IT systems after being hit by ransomware attack - ABC News
After reading this information, answer the following questions:
a) Which information assets are involved (what types of information and how much of it)?
b) What happened to the information assets?
c) What was the data state of the compromised information: is the data in transmission, in storage or being processed?
d) Which of the following security goals are compromised? Explain your answer, referring to different stages in the process if necessary.
i. con?dentiality
ii. integrity
iii. availability
e) Is it appropriate to refer to the incident as an attack? Justify your answer.


a) The information assets are some data files containing personal details of current and former QUT staff and students. The QUT update on February 6, 2023 gives some idea of the number of persons impacted: 2492 current employees, 17 current students, 8,846 former employees, 50 former students. The personal data that was accessed by the cyber criminals included names, tax file numbers and bank account numbers.
b) According to the news report, this was a ransomware attack, with Royal group gaining access to QUT's systems, encrypting some of the files, copying some of the data files and then sending ransom notes to all of the QUT printers.
c) The compromised information was being stored.
d) The security goal that is breached:
i. Confidentiality is breached through the unauthorized disclosure of personal information (bank account numbers, tax file numbers, ...)

to the criminals. They also threatened to publish the information they'd copied online if the ransom was not paid (read the ransom note in the ABC news article).
ii. There is no information in the article to suggest that integrity was breached, but that would usually be the case with ransomware. Data files would be encrypted, and the required decryption key would not be available for the authorized users unless they paid the ransom. So there was unauthorized modification.
iii. The IT systems at QUT were shut down on 22 December, making many assets unavailable to the legitimate authorized QUT users - this lasted for several weeks.
e) Yes, this is an attack. It is not an accident. It is a deliberate action by members of the Royal group to gain access to QUT's systems, cause harm and offer to stop/repair for a fee (described in the ransom note as a royalty).

QUESTION 4
The Australian Cyber Security Centre (ACSC) is a federal government organisation and hub for multiple government departments that aims to prevent and combat cyber security threats and to minimise harm to all Australians. Part of this role is through sharing information and advice.
a) If you, as an individual, experience a serious cyber incident, the information and contacts listed here (under Report and recover, see: https://www.cyber.gov.au/report-and-recover ) may be helpful to you. Read through the information provided on the page. There are guides to help you report a cybercrime, incident or vulnerability; contact organisations for assistance if you become a victim of cyber-crime, and advice if you think you may have been hacked. Towards the bottom of the page, there is 'Report and recover ...' advice for eight different incident types.
i. List the eight types.
ii. Follow the link to 'Report and recover from scams'. Read the information. Who does it advise that you should report scams to, and under what circumstances?
b) Find the ReportCyber link to report cybercrime to the ACSC. Follow the

ReportCyber link (this is also available as a [Report] tab on the top of the ACSC page). Look at the first page this presents.
i. What options do they give you for categorizing a report?
ii. Why do you think the ACSC would be interested in these reports?
This question is intended to increase both your awareness of information security and of Australian organisations working in this space (that's why we sent you to the ACSC site - it may be helpful for you in the future to know about this resource).
a) You, or someone you know, may be a victim of a scam or cyber-crime, so it is useful to know in advance where to go to for help.
i. Check for yourself what type of incidents are included in the specific 'Report and Recover from ...' links.
ii. The 'Report and recover from scams' link gives information about reporting when:
1. You think a scammer has targeted you, but you didn't give them your details (report to Scamwatch)
2. You have been scammed and lost money (report to your bank and ReportCyber, and take further actions to secure your online accounts)
3. You think a scammer has stolen your personal information (report to your financial institution, and any other relevant services, ReportCyber, and perhaps a credit reporting agency)
b) You can report an issue that is personal, or on behalf of a large or small organisation or a government department. The ACSC can use reports to understand what is happening in the community and to tailor advice to appropriate sectors of Australian society.

QUESTION 5
Watch Prof Avi Rubin's TED talk: 'All your devices can be hacked'. (Search for it on YouTube, or look at https://www.ted.com/talks/avi_rubin_all_your_devices_can_be_hacked#t-997806)  In the video, Prof Rubin describes things security researchers have done to hack some real-world devices, including implanted medical devices, automobiles, mobile phones, and a certain type of radio used by law enforcement and defence agencies. The researchers do things the designers of the devices may not have anticipated, resulting in some surprising outcomes.
Considering both the security goal affected (of the three listed), and the information state (also three states), see if you can find at least one example from the talk for each combination (3 x 3 = 9 possible combinations).
Information StateTransmissionStorageProcessing
Security GoalConfidentiality???Integrity???Availability???
Watching this TED talk is intended to get you thinking about how important information is in our everyday lives, in all sorts of devices used across a range of industries, but also about how vulnerable that data and those devices may be.

The talk is not new, but it raises interesting points about our connected digital lives. Exploiting vulnerabilities has the potential to cause harm - not just to the information or the device, but to people too.

It is also important to think about the scenarios and the type of actions that could result in harm - there's a range of concerns raised here. Which of these hacks did you find most concerning? Why?

Here are a few examples from the talk - you may have noted others: A: Breaching confidentiality for information being transmitted
* Law enforcement radios - researchers could listen in on conversations when the

operators forgot to turn on the encryption switch
B: Breaching confidentiality for information being stored
* Implanted medical device - researchers could see stored patient cardiac data
C: Breaching confidentiality for information during processing
* Researchers could see people entering their passcodes and text messages (through examining the reflections in glasses, windows, etc)
D: Breaching integrity for information being transmitted
* Implanted medical device - researchers could send signals to the device to change the therapies
* Vehicle hacking
E: Breaching integrity for information being stored
* Implanted medical device - researchers could change name, change therapies
F: Breaching integrity for information during processing
* Vehicle hacking - showing different speed than vehicle is actually travelling at.
G: Breaching availability for information being transmitted
* Implanted medical device - turn off the device
H: Breaching availability for information being stored
* Implanted medical device - wipe the data
I: Breaching availability for information during processing
* Implanted medical device - researchers could run down the battery so that the device no longer functioned
