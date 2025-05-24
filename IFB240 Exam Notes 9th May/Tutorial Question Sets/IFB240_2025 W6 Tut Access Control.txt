IFB240 Cyber Security
Week 6 Tutorial Questions on Access Control 

Essential definitions
Review the deﬁnitions given in the lecture slides for the following terms: 
Controls 
(including preventive, detective, and corrective)Separation of duties/
Segregation of dutiesCountermeasuresSubjectsAccess ControlObjectsWhitelistResource ownersBlacklistDiscretionary access control (DAC)Principle of least privilegeMandatory access control (MAC)Need-to-know principleRole-based access control (RBAC)
Attempt these questions before you attend your tutorial and have your prepared answers with you for the session. Be prepared to discuss your answers and/or any problems you encountered in trying to answer these questions. 

QUESTION 1
The Australian Signals Directorate (ASD) provide advice on strategies they recommend organizations apply to significantly reduce their risk of cyber security incidents. The list of strategies is available from the ACSC page: https://www.cyber.gov.au/resources-business-and-government/essential-cyber-security/strategies-mitigate-cyber-security-incidents/strategies-mitigate-cyber-security-incidents [There is a downloadable document titled ‘PROTECT – Strategies to Mitigate Cyber Security Incidents’ available on the left-hand side of the page that may provide a more concise overview. It is a handy resource].  Strategies are rated Essential, Excellent, Very Good, … (these are colour-coded for easy identification in the downloadable .pdf file). A subset of the listed strategies, commonly referred to as The Essential Eight, is: 
1. Application control (whitelisting)
2. Patching applications
3. Configuring Microsoft Office macro settings carefully
4. User application hardening
5. Restricting administrative privileges 
6. Patching operating systems and using the latest version 
7. Use of multi-factor authentication
8. Perform regular backups
Look in the table at the column headed ‘Relative Security Effectiveness Rating’ for the strategies with the rating ‘Essential’.  Read the information about ‘The Essential Eight’ from this web page and answer the following questions.
a) The ASD grouped these essential mitigation strategies into sets, based on the risks that they mitigate. For ‘The Essential Eight’, name each of the three sets they appear in.
b) Classify each of the eight strategies as Preventive, Detective, or Corrective measures. Give a brief explanation of each of the eight strategies.
[More detail on these eight strategies can be found here: https://www.cyber.gov.au/resources-business-and-government/essential-cyber-security/essential-eight/essential-eight-explained.]


QUESTION 2
Whitelists and blacklists are commonly used for access control purposes. 
a)  Read the Media Release from the Australian Federal Government’s Ministers of the Education Portfolio on Cheating Websites available here: Cheating websites blocked | Ministers' Media Centre (education.gov.au)
i. What does the media release report that the Tertiary Education Quality and Standards Agency (TEQSA) has done?
ii. What is the role of Internet Service Providers in enforcing this action?
iii. Would this be regarded as a blacklist or a whitelist?
b)  You may be able to apply restrictions at a more local level. Investigate your web browser to see if there is:
i. a web browsing blacklist, and how you can add a website to the blacklist. 
ii. a web browsing whitelist, and how you can add a website to the whitelist.


QUESTION 3
Two commonly applied access control principles are: the need-to-know principle and separation of duties.
a)  Describe what is meant by each of these two principles.
b)  To what extent can mandatory access control (MAC) be used to implement the need-to-know principle?
c)  Explain how role-based access control (RBAC) can be used to implement separation of duties (or segregation of duties).


QUESTION 4
Many people share documents using cloud services: Google Drive, Dropbox, Microsoft OneDrive, etc. Choose a service and describe the operation in terms of the access control principles discussed in Lecture 5:
a) Is access based on blacklists or whitelists?
b) What access permissions (or modes of access) can subjects have?
c) Does the system use discretionary, mandatory, or role-based access control, or some combination of these?
d) How does the system implement access control phase 1 (policy definition) and phase 2 (policy enforcement)?
e) How can access be revoked?
f) Does the system provide a monitoring feature?

QUESTION 5
Consider access control as occurring in two phases: policy definition and policy enforcement. In the policy enforcement phase, three steps are required before an authorised party is permitted access to a restricted resource. 
a)  Explain each of these three steps in the order they must occur. 
b)  Why is the order they are performed in important?

QUESTION 6
One reason for monitoring access to resources is that it may reveal loopholes in a system that permit others to bypass the access control system and gain access without providing the appropriate credentials for authentication. An example of this is described in a ZDNet article by Catalin Cimpanu, on January 14, 2019; available at: https://www.zdnet.com/article/details-published-about-vulnerabilities-in-popular-building-access-system/ Read this article and answer the following questions:
a) What sort of information asset does this apply to? 
b) What does the article describe as the most important vulnerability in the system?
c) What is required to bypass the access control measures?
d) Was there a mitigation for this at the time the article was written? 
e) Is there any other mitigation strategy available now? (Hint: Search for articles after January 2019)
f) Are there backdoors like this in products you may be using? Look for flaws in routers, security cameras, IoT products, etc. Try a search for ‘Hardcoded password access control flaw’ and include the device name (router, webcam, etc) and/or check AusCERT security bulletins.  

QUESTION 7
An interesting vulnerability type known as Insecure Direct Object references (IDOR) is described in an article by Jessica Lyons in The Register on 29 July 2023: 
Data stolen from millions via missing web app access checks • The Register
Refer to the article to answer the following questions:
a) Explain what an IDOR vulnerability is.
b) What IDOR example is given in the article?
c) How can this vulnerability be exploited?
d) Which security goals (CIA) could be compromised by these actions?
e) In the event of a compromise, would this be regarded as a passive or active attack? 

QUESTION 8
Two factor authentication should provide better security than single factor authentication. However, this requires careful implementation. Read Graham Cluley’s security blog article on 24 October 2016 about the discovery and exploitation of a flaw in PayPal 2FA implementation, available at: https://www.grahamcluley.com/paypals-2fa-proves-easy-bypass/. This vulnerability has now been fixed, but this situation clearly illustrates the importance of user authentication as a component part of access control, and that the implementation requires careful consideration.
a) What sort of information does this apply to? 
b) What did the researcher do to trick PayPal into thinking he had provided the correct information for the second factor?
c) Which security goal is compromised (CIA)?
d) What would an attacker need to do to exploit this flaw and gain access to someone’s account?
e) Would this be regarded as an active or passive attack? Justify your answer.
f) The researcher reported this to PayPal. What did PayPal do in response? 

