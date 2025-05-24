IFB240 Cyber Security
Semester 1, 2025
Outline solutions for Week 11 tut for L9: Trust and Public Key Infrastructure

Essential definitions:
Review the de?nitions given in the lecture slides for the following terms: 
a) Asymmetric key pair
b) Public key fingerprint
c)  Public key spoofing problem
d) Public key trust model
e) User centric trust model
f)  Public key ring
g) Trusted Authority model
h) Digital certificate
i) Certificate Authority

QUESTION 1
The management of cryptographic keys is an important aspect of information security. 
a) Why is key management important? What can happen if the various processes involving cryptographic keys are not well managed?
b) Explain which keys need protection, and what they need to be protected against, for: 
i. Symmetric ciphers (shared secret keys), and 
ii. Asymmetric ciphers (private keys and public keys).
c) What sort of techniques can be used for protecting cryptographic keys? Describe appropriate techniques in each case and explain what the technique protects against. 

a) Management of cryptographic keys is essential part of effective use of cryptographic mechanisms. Need to consider the whole lifecycle of keys: generating, storing, archiving, retrieving, distributing, retiring and destroying keys. If any part of this process is not well managed and there is a compromise or loss of keys, this may lead to a compromise of the confidentiality, integrity, availability and/or authenticity of information assets. Recall the problems we have seen in previous tutorials - for example, the poor key generation process for Tapplock (Q11 in Week 9 Tutorial questions) 
b) All cryptographic keys (symmetric and asymmetric) require protection against modification (integrity breach) and loss (unauthorized destruction). 
i. Symmetric (secret) keys also need protection against unauthorised use and disclosure.
ii. Asymmetric private keys also need protection against unauthorised use and disclosure. Asymmetric public keys do not require confidentiality!
c) Cryptographic techniques can be used to protect cryptographic keys. For example, signatures in digital certificates provide assurance that the public keys have not been modified; symmetric encryption can be used to protect keys during storage; asymmetric crypto could be used to protect symmetric keys for distribution (recall the hybrid cryptosystem discussed in Lecture 8). Physical protection of equipment used to generate, store and archive keys should also be applied.

QUESTION 2
Answer the following questions related to the authenticity of public keys:
a) What is the spoofing problem, with respect to the use of public keys?
b) How can you gain assurance that a public key really does belong to the entity claimed?

a) The spoofing problem is when an attacker replaces a public key (say Alice's public key) with a different public key whose private key is known to the attacker. This allows the attacker to pretend to be Alice (for example, to read encrypted mail intended for Alice). Note that the private key that Alice (the real Alice) has is not the corresponding private key for the public key the attacker has posted as Alice's, so now the attacker can read the mail intended for Alice, but Alice cannot.
b) You need someone to vouch for the information. Someone you trust, or a trusted authority might provide assurance that a particular public key belongs to an entity. A digital certificate issued by a CA gives some assurance that the public key in the certificate belongs to the entity identified in the certificate, provided that the CA has an adequate checking process before they issue digital certificates to entities.

QUESTION 3
Suppose two colleagues, Alice and Bob, use an asymmetric cipher (say, RSA) to communicate confidentially. Their public keys are listed in a file available on the corporate network. Another employee, Carol, wants to know what they are communicating. Carol cannot break the RSA algorithm but is able to access and alter the file containing Alice and Bob's public keys.
a) How does altering the public keys help Carol to gain access to the confidential communications between Alice and Bob?
b) What sort of alterations must Carol make?
c) Explain how this allows Carol to access the messages intended to be sent between Alice and Bob confidentially.

a) When Carol replaces a public key (say Alice's public key) with a different key whose private key is known to her, this allows Carol to pretend to be Alice (for example, to read encrypted mail intended for Alice). Note that the private key that Alice (the real Alice) has is not the corresponding private key for the public key that Carol has posted as Alice's, so now Carol can read the mail intended for Alice, but Alice cannot. The situation is similar for Bob.
b) Carol has to replace each of the public keys with a different public key from a pair where Carol knows the corresponding private key. She will then have access to all messages intended for Alice or Bob after she alters the corresponding public keys. The messages sent before this (using their real public keys) are not available to Carol. If Carol keeps copies of the original public keys belonging to Alice and Bob, and Alice and Bob do not realise that the public keys in the file were changed, then Carol can position herself as a MITM and manage conversations between Alice and Bob as she chooses.
c) Suppose Alice decides to send a confidential message M to Bob. 
1. She looks up the network file for Bob's public key KBpub, but she actually finds the public key Carol substituted for Bob, KXpub. 
2. Alice uses this public key to encrypt her message, M, and sends the resulting ciphertext C= E(M, KXPub) to Bob.
3. The ciphertext C can only be decrypted by the person with the corresponding private key KXpriv (that is: Carol). In mathematical notation, we would write M= D(C, KXPriv). If Carol can intercept the ciphertext, she can decrypt the message to recover the plaintext M. 
4. Once Carol reads M, she can decide whether she wants to pass the message on to Bob unchanged, or if she wants to alter it to Mx. 
5. Carol then encrypts M or Mx with the original public key for Bob, KBpub, and sends CX= E(MX, KBPub) to Bob.
6. Bob can decrypt this message using his private key: MX= D(CX, KBPriv).
So Carol's role is the traditional MITM attacker.

QUESTION 4
With respect to the public keys used with asymmetric ciphers, 
a) What is a Certification Authority (CA)? What role does a CA play in providing assurances of the authenticity of public keys?
b) What is a digital certificate?
c) How much trust can be placed in a digital certificate? Explain your answer. Relate this to the Week 11 - Activity 4: Find out about Certification Practices questions.
d) Is a digital certificate the same as a digital signature? Explain your answer.

a) A certification authority (CA) is a trusted authority who creates, issues and revokes certificates binding entities and public keys. The CA maintains certificate status information and issues CRLs, publishes current certificates and CRLs, and maintains archives of status information.
b) A digital certificate is an electronic file that contains information identifying a particular entity (say, Alice) and containing the public key belonging to that entity. The certificate binds a public key to an entity. The CA who issued the certificate (and signed it with a digital signature) is vouching for the information. The certificate provides a solution to the spoofing problem if it is issued by a recognised CA which has procedures in place to check identification details before providing certificates.
c) You can trust the information in the certificate (ID-public key binding) if you trust the issuing CA to have identified the certificate owner and you can verify the CA signature on the certificate. [Two things to check here: 1. You can find out about the identity checks performed by the CA from their Certification Practice Statement - this is a legally binding document. 2. Recall from Lecture 8 Part C: Signature verification provides message integrity assurance and authentication of message sender]. To verify the CA's signature, you need an authentic copy of the CA's public key.
d) No, a digital signature is not the same as a digital certificate. Alice's digital certificate will be the same each time she sends it, but her digital signature on a message will differ as the message content differs (or the hash of the message content, if hashing is used as part of the signature process). A digital certificate is a specific type of message binding a public key value to an entity and signed by the CA vouching for the information.

QUESTION 5
This question relates to the digital certificate QUT has for Canvas. Go to the QUT Canvas home page (https://canvas.qut.edu.au), and click on the padlock icon, to obtain the certificate. The actual process varies a little from browser to browser, so you may have to investigate this a bit: 
* In IE and Edge, when you click on the padlock, a dialoque box opens; View Certificates or Connection is Secure is an option in the box. Click on this and then click on the little certificate icon (look up near the top to see it) to view the certificate.
* In Firefox, when you click on the padlock, a Site information box opens; follow the arrow from Connection and you will find the Site Security information, there is a More information link at the bottom of the box. Click on this to get to View Certificate.
* For other browsers, there'll be a similar process. Explore your browser to find certificate details.
   
View the details of the QUT Canvas certificate (use the General and Details tabs near the top of the box, and scroll bar in the Certificate Fields to see the different fields) and answer these questions:
a) Who is the certificate issued to?
b) Who is the certificate issued by?
c) What is the validity period for this certificate?
d) Which X.509 certificate version is used?
e) Which cryptographic algorithm is used to sign the certificate?
f) What type of public key algorithm is certified, and what is the key size?
g) Click on the public key to view it. Although the key is a 2048 bit key, rather than seeing the string of bits (0's and 1's) it appears as a series of digits 0-9 and characters A-F. What format is used here, and why?
h) Now look at the certification path (IE and Edge) or certificate hierarchy (Firefox and Chrome). Which CA issued this certificate?
a. View the CA's certificate. How does it compare to the QUT Canvas certificate, especially with respect to the version numbers, validity period, key size, and signature algorithms used?
b. Which CA issued that CA certificate? Follow the path. View that CA's certificate and compare it with the QUT Canvas certificate and the intermediate CA certificate; especially with respect to the version numbers, validity period, key size, and signature algorithms used. 
i) Who signed the root CA's certificate?
j) In the certificate details (on any of these except root certificates) there is a field for CRL Distribution Points. What does the CRL refer to? Why is this required? 
k) Did you find a mention of OCSP? What does this refer to?

The detailed values are not important here, the main thing is to get a feeling for the type of information provided in certificates and to observe the features of the browser PKI. You should find all the answers to the questions above by exploring certificates available in your browser. I have used Chrome for this. 
a) Issued to: canvas.qut.edu.au (from the 'General' tab)
b) Issued by: R11 (from the 'General' tab)
c) The validity date - from dd/mm/2024 to dd/mm/2024. (No, it's not dd or mm on the certificate. Look in the certificate for the actual date and month).
d) The certificate version - V3 (from the 'Details' tab)
e) The cryptographic scheme used for certificate signature - PKCS #1 SHA-256 With RSA Encryption 
f) The type of public key algorithm certified and the key size: PKCS #1 RSA Encryption, 2048 bits. 
g) Public key is presented in hexadecimal format. In binary it is not easily human readable :) (from the 'Details' tab, click on the public key field to see key value in the box below)
h) The certificate was issued by the CA called R11, Let's Encrypt, US. You can view their certificate by going to the Certification Path tab, and clicking on R11) 
a. The R11 certificate is a Version 3 certificate, valid from 3/13/2024 to 3/13/2027, signature algorithm is PKCS #1 SHA-256 With RSA Encryption, and key size is 2048 bits.
b. The R3 certificate was issued by ISRG Root X1. Their certificate is a version 3 certificate, valid from 4/06/2015 to 4/06/2035, signature algorithm is SHA256RSA, and key size is 4096 bits. This certificate is one of the certificates preloaded in your browser (appears as a trusted root CA)
i) The root CA's certificate is a self-signed certificate (Issuer and Subject are the same entity). You can only trust this certificate if you know that you (actually, your browser) received it through a trusted channel. 
j) The CRL is the certificate revocation list: a list of certificates this CA has revoked before they reach their expiry date. Certificates may be revoked for several reasons, as noted in the Week 11 Activity 4 questions: if the private key corresponding to the public key in the certificate has been compromised, lost or stolen; if a CA discovers the certificate was issued in error; domain name details have changed, ...
k) OCSP = Online Certificate Status Protocol. This protocol will check regularly to see if the certificate presented has been revoked.


QUESTION 6
An alternative means for examining certificates is via browser menus. 
* For IE, you can check certificates through 'Settings' 'Internet Options' 'Content' 'Certificates'
* For Firefox, you can check certificates through 'Menu' 'Options' 'Privacy and Security' and scroll down to 'Security' to find 'Certificates'. Click on 'View Certificates'.
* For Chrome, the process is included in the Part C lecture segment.
* For other browsers, there will be a similar process.

Investigate some of the other digital certificates you have stored in your browser.
a) Can you find any certificates which: 
i. Are for intermediate CAs?
ii. Are for trusted Root CAs?
iii. Have validity periods of less than one year?
iv. Have validity periods of more than five years?
v. Have already expired?
b) Are there any 'untrusted' certificates listed (you may need to scroll across to find these - look for arrows to find additional fields)?
c) Suppose there have been some fraudulent certificates issued recently that are not currently listed by your browser as 'untrusted'. What are the security implications in this situation?

a) Again, the details of individual certificates are not that important and will vary across different installations. Some generalisations: normally you will find that certificates issued to end users (which could be organisations, or servers within organisations) have shorter lifetimes from a few months, to one or two years. Intermediate CA certificates are more likely to be for five to 10 years and root CA certificates are typically self-certified and have lifetimes of 10 to 50 years. You can probably find some CA certificates which have expired. Most browsers give some kind of warning when you open an expired certificate but will let the user continue to use the information if desired. They will prompt the user to make a trust decision.
b) Untrusted certificates: Look for TurkTrust and DigiNotar, among others. There should be quite a few. Some will have expired already, but some have validity periods beyond 2023. Search the information security news for the stories behind these breaches. Or read the Wikipedia entry for DigiNotar, available here: DigiNotar - Wikipedia
c) If there are certificates issued that are fraudulent, but not currently listed as untrusted, the user will make trust decisions based on the apparent validity of the certificates. For example, they may consider a website as legitimate (there'll be no browser warnings) when in fact the site is false. This situation can be exploited by cybercriminals. 


QUESTION 7
Describe the main features of the hierarchical and user centric trust models. What are the relative advantages and disadvantages of these two approaches?

See lecture slides for details of these models. The features relate to trust relationships. 

       The hierarchical model (discussed in Part B) is highly regulated. In a strict hierarchy, a single root CA is the root of a tree, this provides certificates to intermediate CAs (nodes), who provide certificates to users (the leaves). There are rules regarding procedures for checking identity claims and issuing certificates. 
       
       The user-centric model (discussed in Part A) is more anarchic - users can decide who they trust and sign to endorse each other whenever they want to.

Hierarchical model: advantages
* Good fit for highly structured organisations, such as military and government.
* The tree structure results in unique certification paths between any two entities (so finding certification paths is simple)
* This structure also scales well to larger systems - can add another CA if required by growth in organizational structure, etc
Hierarchical model: disadvantages
* need a trusted third party (root CA) so not suitable for all applications.
* 'single point-of-failure' target (no redundant pathways). If any node is compromised, trust impact on all entities stemming from that node. 
* Strict hierarchy does not work well for global implementation (who is trusted root?)
 
User centric model: advantages
• It's a very simple model 
• Works well for a small number of users
• Does not require expensive infrastructure to operate
User centric model: disadvantage
• Decisions on trust rely on human judgment
• Might vary from user to user, or a single user might make variable decisions over time.
• Might not be suitable for general public use, where purpose and implications of misuse is not understood
• Not appropriate for trust-sensitive areas such as finance and government.

QUESTION 8
Read the Ars Technica article 'Renegade Certificate removed from Windows. Then it returns. Microsoft stays silent' by Dan Goodin (available at Renegade certificate removed from Windows. Then it returns. Microsoft stays silent. | Ars Technica) and answers the following questions:
a)  What type (hierarchy level) of certificate did Microsoft remove from Windows?
b)  What was the impact of the certificate removal on users of some applications?
c)  The article suggests that the certificate removal may have been intentional. If so, what might have motivated Microsoft to remove this certificate?
d)  From the included screenshots of the certificate under discussion, what was the validity period (in years) of this certificate?
e)  According to the article, what ultimatum did Google give Symantec in 2015? What motivated Google to issue that ultimatum?
f)  How do the actions of CAs affect the security of networked communications? 
g)  How do the actions of vendors such as Microsoft and Google affect the security of networked communications?
a) Microsoft removed a particular root certificate from Windows. 
b) The certificate was a root certificate, in the certificate hierarchy for some other certificates used for app signing. When the certificate was removed, some Windows users accessing apps such as QuickBooks and Avatax received warning messages that the apps were untrusted. 
c) The certificate in question was issued in 2015 by Symantec, who improperly issued certificates for several domains, including google.com. Back in 2015, there was a major discussion of whether Symantec could be trusted and calls for their certificates to be revoked. 
d) This was a root certificate with a validity period from 8/11/2006 to 17/07/2036. 
e) In 2015, when Symantec was found to have issued certificates that it should not have, Google threatened to remove the Symantec root certificates from Chrome. This would have meant any certificates in hierarchies that traced back to those root certificates would be shown as untrusted in Chrome. However, this would have impacted many other organisations with certificates in those hierarchies. 
f) If CA's issue certificates to entities without performing appropriate checks that the Certificate signing request is valid, then the people obtaining those certificates can impersonate those entities - for example, set up fake websites. (For example, the fake google site will have a key pair, and the padlock symbol will appear in the browser). The browser vendors require CAs to perform the checks that they state in their Certification Practice Statements as their practice, as trust in online services relies on this. 
g) The browser vendors (such as Microsoft, Google, ...) choose which root certificates they will include as trusted root certificates. It is important that the trust pathways supporting public key use are trustworthy. Many (but not all) network communications protocols rely on public keys obtained through certificates, and industry sectors such as e-commerce are built on this infrastructure.
