FACULTY OF SCIENCE - 2025
IFB240 Information Security

Outline solutions for Wk 2 tut - relates to L2: Threats, Vulnerabilities and Attacks

Essential definitions: Review the de?nitions given in the lecture segments for the following terms:
ThreatDoS and DDoSThreat actorMalwareThreat actionMITM (Man-in-the-Middle/Machine-in-the-Middle)
attackVulnerabilityPhishingSecurity incidentRansomwareAttackReplay attackPassive attackSpoofingActive attackSocial Engineering
QUESTION 1
Clearly explain:
a) The relationship between threats, vulnerabilities, and attacks.
b) Whether it is possible for a threat and a vulnerability to coincide without an attack occurring.
Give examples to illustrate your answers.


a) The relationship is: when vulnerabilities are deliberately exploited by threats, this is an attack on the information asset.
i. Example: Storing sensitive hardcopy information in an unsecured physical location is a vulnerability. Threats to the information asset include theft and destruction.
i. If the documents are stolen (removed from the location by a thief), then the information security goal Availability is breached for that asset.

ii. If the documents are viewed by an unauthorized person, then confidentiality is breached for that asset. There are many possible examples for other breaches.
b) If a threat and vulnerability coincide and the threat is not the result of deliberate human action, then the result is a security incident (which may cause extensive damage to information assets) but this is not described as an attack.
i. Example 1: The Red Cross data breach discussed in the Week 1 tutorial was a security incident resulting from human error rather than deliberate malicious action, so it is considered a security incident rather than an attack.
ii. Example 2: The 2022 floods in Brisbane resulted in a loss of availability for many services. As this was due to an act of nature, it is considered a security incident rather than a DoS attack.

QUESTION 2
Vulnerabilities exist in many components of information systems. They may be related to the use of devices that are often not considered a part of your information system. Researchers have discovered vulnerabilities in many smart home devices. Read Neil Rubenking's article on the	Ring	Doorbell,	appearing	in	PC	Mag	in	November	2019	(available	here: https://au.pcmag.com/bitdefender-box-2/64310/exclusive-bitdefender-discovers-ring-doorbell- vulnerability). Use the information in the article to answer the following questions:
a) If used correctly, what does a smart doorbell like the ring Doorbell let a user do? What can they see, and what device do they use to gain this view?
b) In the initial installation of the doorbell, the doorbell device needs to be connected to a home network. What sort of communication channel is used to make that connection?
c) What is the vulnerability that the researchers found, when the device is initially connecting to the home network?
d) What is the information asset that is vulnerable?
e) What state is the information asset in when it is vulnerable?
f) Which security goal will be compromised if a threat acts on this vulnerability?
g) How did the researchers trigger the vulnerable condition?
h) If an attacker did this, would this be an active or passive attack? Justify your answer.

i) Describe some possible subsequent attacks (chain of events) and identify the security goals compromised by the attacks you describe.

a) The smart doorbell lets you see who is at the door on your smartphone, and you can answer the door remotely (if you have the model with doorbell connected to the door lock).
b) The doorbell is connected to the home WiFi network.
c) When the device is initially being connected, you connect your smartphone to the WiFi signal broadcast by the device, then you enter the credentials for your home WiFi network, so that the device can connect to that network. The vulnerability is that the initial transmission to connect the device to the home network is not encrypted, and the device sends the WiFi password in that transmission.
d) The vulnerable information asset is the home WiFi password.
e) The information is in transmission when it is vulnerable.
f) The security goal compromised by an attacker eavesdropping on the transmission is confidentiality.
g) The researchers triggered the vulnerable condition by deauthorizing the doorbell on the home network, which forced the owner to repeat the vulnerable setup procedure when the attacker was monitoring for the transmission.
h) If the attacker deauthorized the doorbell, then they have interacted with your system, and this is an active attack.
i) An attacker exploiting the vulnerability can use your home WiFi password to access to your home WiFi network. What could they do? There are many possibilities! Install devices, remove devices, change the password, ...

QUESTION 3
On Friday, July 19, 2024, there was a massive outage related to a problematic update for the Crowdstrike security software. Read the article 'Crowdstrike update crashes Windows systems, causes outage worldwide'	by	Ionut	Ilascu	in	Bleeping	Computer	on	July	19	(available	here: https://www.bleepingcomputer.com/news/security/crowdstrike-update-crashes-windows-systems- causes-outages-worldwide/ ). Use the information in the article to answer the following questions:
a) What did CrowdStrike do that triggered the outage?

b) What was the information asset that was vulnerable?
c) What impact did this have on companies that used Crowdstrike software?
d) How was the issue detected?
e) Which of the following security goals were impacted? Justify your answer.
i. Confidentiality
ii. Integrity
iii. Availability
f) The Crowdstrike CEO George Kurtz issued a statement that included this sentence: 'This is not a security incident or cyberattack.' Do you agree with this statement, or part of it? Explain your answer.
g) For affected systems, what corrective action was required?


CrowdStrike Outage:
a) CrowdStrike sent out a software update for its security product 'Falcon' that had a faulty component. The faulty update caused Windows Systems with the CrowdStrike product installed to crash, and they were unable to reboot successfully.
b) 	The information asset that was vulnerable was computers with Windows O/S that have CrowdStrike's Falcon product installed. Other operating systems were not affected.
c) The impact on companies depended on the degree of dependence on Windows-based systems. As these computers were unable to be rebooted, all the information assets stored on the devices or accessed using these machines were unavailable to authorized users. The specific impact depended on the enterprise context: some airports, TV stations, and hospitals were unable to perform their usual business operations [some universities were also affected! YES, parts of QUT!]
d) The issue was detected by end users who found themselves staring at the Blue Screen of Death!
e) The security goal compromised is clearly availability. The resources were not available to authorized users when required. There is no information to suggest that confidentiality or integrity were compromised.
f) This statement is partly correct. The first part is incorrect - This is most definitely a security incident, as availability is compromised. The second part is correct - It is not a cyber attack, as there was no deliberate attempt to cause harm. However, the outage was costly for many businesses who were unable to provide their regular services until the systems were restored - they were harmed. In the coming weeks and months, we will find out more about

the cost of this event.


QUESTION 4
Software vulnerabilities are often analysed, catalogued and given CVE IDs and a CVSS Score.
a) Find out what these acronyms refer to (you can search to find this information, or read a simple explanation here: What is a CVE? (redhat.com) ).
i. What is a CVE identifier, and why is it used?
ii. 	What is the CVSS score, and what does that indicate? (for more detail see: Common Vulnerability Scoring System Version 3.1 Calculator (first.org)).
b) Visit the CVEdetails.com site (https://www.cvedetails.com/) to find out about the prevalence of software vulnerabilities, and the various categories.
i. Look at the 'Vulnerabilities by type and year' graph, and comment on the overall trend in the number of software vulnerabilities.
ii. Look at the 'Distribution of vulnerabilities by CVSS' graph, and comment on the overall trend in CVSS numbers.
iii. In the menu on the left of the page, under 'Vulnerabilities', select 'By Type'.
i. What type of vulnerabilities are common in 2024?
ii. When categorized by impact type, what type of vulnerabilities are common in 2024?
a) CVE and CVSS
i. CVE is Common Vulnerabilities and Exposures. This is a list of known computer security vulnerabilities.
ii. CVSS is the Common Vulnerability Scoring System - gives a score from 0 to 10 to vulnerabilities in computer systems with respect to impact on security - 10 is highest score.
iii. Useful information about the CVS can be found here: Common Vulnerability Scoring System Version 3.1 Calculator (first.org) You might be interested enough to look at the C I and A inputs used in computing the CVSS Score. (Yes, C I A!)
b) Visit the site and look at the various types of vulnerabilities detected. There are thousands of vulnerabilities reported each year, and some are very serious. This question is less about the actual number, and more about raising your awareness that software frequently contains bugs, some of which can be exploited to cause harm.




QUESTION 5
Some vendors offer rewards or incentive payments ('bug bounty or bug bonus') to encourage finders of vulnerabilities to report them to the vendor.
a) A Naked Security article on 23 May 2018 reports on a 'bug bounty' payout to a university student (available at Surprise! Student receives $36,000 Google bug bounty for RCE flaw - Sophos News). According to the article:
i. Who paid the bounty?
ii. How much did the student receive as their bug bounty?
iii. What sort of bug was it?
iv. How could it be exploited, and what impact would exploitation of the vulnerability have?
b) Google continue to run a Bug Bounty or Vulnerability Reward Program, to identify and fix security issues in their products. Read up on how much Google has paid out in Bug Bounties here: Key Stats | Google Bug Hunters - Google Bug Hunters
c) Many organisations offer bug bounties. Bugcrowd maintain a list of bug bounty programs at the following location: https://bugcrowd.com/list-of-bug-bounty-programs Look at the bounties offered by various vendors - some familiar names (Australia Post, ByteDance, Facebook, Mastercard, Spotify, etc). You may need to access vendor pages for the payment amounts and details.
i. Compare these bounties with the payouts available from other sources, such as the price list for Crowdfense, available at: https://www.crowdfense.com/exploit-acquisition- program/
ii. How do the prices compare with the vendor bug bounty programs?
iii. Who are the customers of Crowdfense?
iv. What would influence your decision regarding reporting flaws to vendors or selling them elsewhere?
e) In March 2017, WikiLeaks released documents referred to as Vault 7. See, for example, this ABC news article form March 2017: http://www.abc.net.au/news/2017-03-08/wikileaks-releases- thousands-of-documents-cia-revelation/8334366.
i. Why did this release gain so much attention at the time?
ii. What is the relationship between these documents, software vulnerabilities and information security?

What do you do if you discover a serious and exploitable vulnerability? Bug bounties are one approach aimed at encouraging responsible disclosure of discovered vulnerabilities.

a) According to John Dunn's May 23, 2018 article 'Surprise! Student receives $36,000 Google bug bounty for RCE flaw:
i. Google paid the bounty
ii. The bounty paid was $36,337.
iii. The bug was in Google's Google App Engine APIs, particularly the app_config_service, and allowed remote code execution (RCE). That is, the student was able to remotely access Google resources and execute (run) code.
iv. Impact: the vulnerability allowed the student (or an attacker) to access the Google GAE and run their own code as if they were a user. The student was able to set their own app as a 'Super App'. Google asked the student to stop exploring it further, paid him the bounty and fixed the vulnerability.
b) Google payouts to date: over $45 million in total, paid to almost 3,000 different bug hunters - explore the details yourself. ? 
c) BugCrowd lists: generally to get a bounty the bug reported must be new, relevant to the listed organisation (not in a third party app) and responsibly disclosed. You tell the organisation and give them time to fix the problem before the vulnerability is made public. Bugcrowd list has links to many organisations - check up on some
:). For example, look at the Microsoft payouts.
d) The Crowdfense prices for zero-day exploits (exploiting a software vulnerability that, until now, no one knew existed) are shown in categories and can pay millions of dollars, depending on what the software is, how hard it is to exploit and what you can do.
i. Prices offered are much higher than the bug bounty programs. For example:


ii. According to Crowdfense FAQ, the customers are government institutions in need of advanced capabilities.
iii. Sale to these buyers is conditional on not reporting the flaw to the software vendor, so the product will remain flawed and exploitable. But you don't know who will be exploiting it, or for what purpose. It is a disturbing thought. Responsible disclosure might not give you the same $$ return, but you will have less to worry about afterwards. In info security, ethics is very important.
e) Vault 7 contained disclosures that allegedly revealed the US CIA's surveillance and monitoring capability; including zero-day exploits for software used on phones by major companies: Apple, Google, Samsung. Did they develop these exploits themselves, or buy these zero days? US citizens were using these very products, that the US CIA knew were vulnerable and had the capacity to exploit. Is that okay, or is the government acting against the best interests of its citizenry? These are ethical questions.

QUESTION 6
The Australian Competition and Consumer Commission (ACCC) provide information on activities related to cyber security on the Scamwatch site: http://www.scamwatch.gov.au/ .
a) 	Use the Types of Scams page to find out what the warning signs or clues are you advised to look for associated with:

i. Text messages and SMS
ii. Phone calls
iii. Email
iv. Social media
b) Use the Scam statistics page under the Research and resources tab, and select appropriate options from the dropdown menus [in the boxes click on the ? on the right hand side to see the options] to find the number of reports to the ACCC:
i. For All types of scams in 2024 (select 2024 at the top of the date list)
ii. For All types of scams in 2023
iii. Which type of scams do people lose the most money to?
iv. Which type of scams are most commonly reported?
c) Change from All types of scams to Phishing and look at the statistics again:
i. For all of 2024
ii. For all of 2023
iii. What are the most common delivery methods for phishing?
iv. What proportion of these reports have associated financial losses?
d) Change to Dating and romance scams and look at the statistics again:
i. For all of 2024
ii. For all of 2023
iii. What are the most common delivery methods for this type of scam?
iv. What proportion of these reports have associated financial losses?
e) What are you advised to do to protect yourself from scams?
f) Watch the Stop Check Protect video available here: https://www.scamwatch.gov.au/ . If you have time, go to the Research and Resources tab, and select Resources. Watch some of the other Scam Awareness videos.
g) Take the Phishing Quiz at https://www.opendns.com/phishing-quiz/ to see how well you can distinguish between a legitimate site and a phishing site.

The type and number of scams is rapidly increasing, and something you need to keep in mind when you are contacted - whether by text, phone, email, social media...
a) Find out the warning signs. Protect yourself. The vulnerability being exploited by scammers is with the people who receive and respond to messages: some are

fooled, thinking it is legitimate. Some QUT students have been victims, and we want to raise your awareness, so that you are less likely to be one of the victims.
b) Scam statistics from ACCC: play with the menu options to find out the numbers.
c) Phishing statistics: play with the menu options to find out.
d) Dating and romance scams: notice the rate of financial loss with these?
e) Find out how to protect yourself.
f) Watch some of the Scam awareness videos from earlier years: 2021 and 2022. The
Stop scams. Speak up. message is a good one, as is the shopping scams.
g) Try the Phishing exercise for yourself. Go on, try it! Test your skill when you are actively thinking 'Is this a phish or not?'. How often are you paying this much attention to deciding on legitimacy when reading your email?

NOTE: We don't want you to be a scam victim, but it may happen to you or to someone you know. So be aware of
* things you can do to make it less likely that you will be a victim, and also
* things you can do if you (or a friend or family member) are scammed, to reduce the impact.
