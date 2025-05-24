IFB240 Cyber Security

       Outline solutions for W9 tutorial questions for L8: Asymmetric Cryptography Essential concepts: Review the lecture slides for the following terms or phrases:
Secure channelModular exponentiationInsecure channelKey pairSymmetric cipher key establishment problemPublic keyPre-distribution of keysPrivate keyTrusted third partyDigital signatureAsymmetric cryptographyNonrepudiation
QUESTION 1
Suppose a symmetric cipher is to be used to provide confidentiality for messages sent within an organization.
a) How many keys are required for two people to communicate confidentially using a
symmetric cipher?
b) How many keys are required for five people to communicate confidentially using a
symmetric cipher, so that any two of the five people can communicate securely?
c) How many keys are required for ten people to communicate confidentially using a
symmetric cipher, so that any two of the ten people can communicate securely?

Using a symmetric cipher,
a) For two people to communicate securely, one shared secret key is required.
b) For five people to communicate securely, so that any two can share confidential messages, ten shared secret keys are required. Each of the five people needs keys to communicate with each of the other four people (5 x 4 = 20), but the key A uses to communicate with B is the same as the key B uses to communicate with A, so total number is 20 / 2 = 10.
c) For 10 people, need (10 x 9)/ 2 = 45 distinct keys.

QUESTION 2
For encrypted messages to be exchanged, each communicating party needs the secret key.
a) Describe three ways to perform key distribution securely if asymmetric ciphers are not used (Options given in Lecture 8 Part A).
b) If key distribution occurs without the use of asymmetric ciphers, how does this restrict the type of entities who will be able to communicate securely?

a) Key distribution could be performed:
i. Over a different, secure channel, perhaps ahead of the need to communicate over the insecure channel (referred to as pre-distribution).
ii. By making use of a trusted third party with existing shared secret keys to users: they can perform the role of a key server - in a similar manner to Kerberos.
iii. Diffie-Hellman key agreement can be used - this algorithm has both private and public components of the participant's contributions to the shared secret key, so it is a public-key protocol, but cannot be used for encryption.
b) The restriction relates to trust. Either
i. a trusted channel is required to pre-distribute the key, or
ii. a trusted third party is required, or
iii. if Diffie-Helman is used, then the participants need to trust that they are communicating with the party they think they are.
       In situations where these are unreasonable expectations, shared symmetric keys cannot be established.

QUESTION 3
The Diffie-Hellman key agreement algorithm allows two entities to establish a shared secret key without requiring the use of a secure channel. That is, they can establish a shared secret key even though the messages they send may be observed by others.
a) What sort of mathematics is required to perform Diffie-Hellman key agreement?
b) One problem with this scheme is that each entity has no assurance about the identity of the entity they are communicating with.
i. What sort of attack is possible because of this?
ii. What impact does this have on the security of subsequent communications?

a) The mathematics used is modular exponentiation: integer exponentiation over a finite set of integers. For Diffie-Hellman, the modulus must be a prime number.
b) Because there is no authentication of the communicating parties, a man-in-the-middle attack is possible:
* Carol can pretend to Alice that she is Bob, and pretend to Bob that she is Alice. Then she can establish keys to use with each of them.
* The messages that Alice thinks she is sending securely to Bob are in fact going to Carol (pretending to be Bob) who can read them and forward them on to Bob (even modify them if she wants to).
* Bob receives the messages he thinks are from Alice (but they are really from Carol). The situation is similar for messages sent from Bob intended for Alice.
* The impact on the security of the communications is that they are not really secure at all. Carol has access to the content (so confidentiality of communications between Alice and Bob is breached) and can modify it (integrity breach), or decide not to pass the message on at all (availability breach).


QUESTION 4
Alice wants to send a confidential message to Bob. They do not have an existing shared secret key. Suppose that Alice and Bob agree to use an asymmetric cipher (say, RSA). Bob has a public key KBpub and the associated private key KBpriv.
a) What should Bob do with each of these keys to permit people to send confidential messages to him?
b) Outline the set of steps that Alice must follow to encrypt a message to send to Bob.
c) Outline the set of steps that Bob must follow to decrypt ciphertext received from Alice.

a) Bob should keep his private key KBpriv secret (no one else should know what it is). He should make his public key KBpub available to others.
b) Alice to encrypt and send message to Bob:
1. Alice prepares the message M, which may include coding the message as an integer (or a series of integers, depends on the size of the message).
2. Alice encrypts the message using the agreed asymmetric cipher encryption algorithm (say, RSA) and Bob's public key KBpub, to produce ciphertext C, where C = E(M, KBpub).
3. Alice then transmits the ciphertext C to Bob.
c) Decryption by receiver (Bob):
1. Bob receives the ciphertext C.
2. Bob decrypts the ciphertext using the agreed asymmetric cipher decryption algorithm (RSA) and his private key KBpriv, to recover the encoded message M, where M = D(C, KBpriv).
3. Bob decodes the message, if necessary, to recover the plaintext.

QUESTION 5
The Guardian newspaper promotes itself as an independent news organisation that delivers fearless investigative journalism, free from political influence, giving a voice to the powerless. People can contact journalists at The Guardian with information to assist in their investigations. However, those contacting the journalists may be worried that the information they provide will be read by others. The Guardian provides an option for people to 'privately contact our journalists'.
Go to https://www.theguardian.com/pgp and scroll down to find the list of journalists, and the corresponding key information. Use this information to look at the public keys for several journalists.
a) What do you notice when you compare the keys for Geneva Abdul and Lisa Bachelor?
b) You can use these keys to encrypt a message you want to send to the journalists. Which security service does this provide (think CIA)?
c) What do you need to do if you want the journalists to send an encrypted message to you in response?

The keys are not the same size! Lisa has a much shorter key. This has security implications.
This is encryption for the purpose of providing confidentiality for your message.
If you want the journalists to send an encrypted response message, then you need to have a key pair, and give the journalist a copy of your public key to encrypt the message with.
Then you would use your private key to decrypt the message.

QUESTION 6
Locate the CrypTool Online site https://www.cryptool.org/en/cryptool-online. Under Modern encryption, select RSA (explained step-by-step). In the Readme document at the top right of the screen, read the information about the type of numbers that are used to generate the public and private keys.
a) Choose the two primes p and q to be 17 and 19. [This is for demonstration purposes - in reality much much bigger primes would be used to provide computational security.] Then choose the public key value e = 23. Use the CrypTool online site to check that this is a valid choice, and then list the public key.
b) What is the corresponding private key?
c) What sort of messages can be encrypted using RSA:
i. What type of input, and what is the size restriction?
ii. If you wanted to send the message 'Hello' (without the quotation marks) what needs to happen, before encryption can be performed?
d) Suppose the message 'Hello' is converted to 72,101,108,108,111 in an encoding step, before encryption. What is the corresponding ciphertext?
e) What key is needed to decrypt a received ciphertext message that was encrypted using this public key?

a) Computed public key is (323, 23). This is valid.
b) Corresponding private key is (323, 263)
c) Can only encrypt integers between 0 and 322 (the public key value is the modulus).
d) Hello: Is converted to 72,101,108,108,111 before encryption. Corresponding ciphertext -> 268, 271, 14, 14, 308
e) Need to use the private key to decrypt (given in part b)

QUESTION 7
Alice wants to send a message and an associated digital signature to Bob. Alice has a public key KApub and the associated private key KApriv. Similarly, Bob has a public key KBpub, and the associated private key KBpriv. Explain the cryptographic steps necessary for:
a) Alice to generate her digital signature, and
b) Bob to verify Alice's digital signature.

c) Repeat parts a) and b) if an additional step, hashing the message, is included in the digital signature formation and verification in order to reduce the computational overhead.
d) Digital signatures provide a means to obtain non-repudiation.
i. Why is non-repudiation important?
ii. Why is symmetric cryptography alone unable to provide non-repudiation?

a) Alice's signature generation:
i. Alice prepares message M (which may include coding the message).
ii. Alice inputs the message and Alice's private key to the signature creation algorithm to obtain her signature for this message: SigA(M).
iii. Alice sends both SigA(M) and M to Bob.
b) Bob performing signature verification:
i. Bob receives message M and claimed signature SigA(M).
ii. Bob inputs SigA(M), M and Alice's public key to the signature verification algorithm.
iii. If the verification output is:
* YES then Bob can be assured that SigA(M) is the signature on message M formed by Alice.
* NO then Bob has no assurance that the signature on the message was formed by Alice. It may be a different message, or a signature formed by someone else.
c) Alice's signature generation: similar to a) except the message is hashed, and the signature performed on the hash of the message.
Bob performing signature verification: similar to b) except Bob hashes the message he receives and inputs the signature and the hash of the message into the verification process. If the verification process output is:
* YES then Bob can be assured that the message he received has the same hash value as the message M signed by Alice, and if the hash function is collision resistant then it is highly likely it was the message Alice sent.
* NO then, as before, Bob has no assurance that the signature on the message was formed by Alice. It may be either a different message (so the hash would be different) or the signature was formed by someone else (so Alice's public key won't work to verify it).
d) Non-repudiation ensures that users cannot falsely deny an action has occurred.
i. It is important where it necessary to resolve a dispute about some action that has occurred, for example whether a contract was signed or a transaction authorised. Digital signatures provide authentication of the message sender, integrity and non- repudiation, so that is useful for applications such as e-commerce.
ii. Symmetric crypto cannot provide non-repudiation as message authentication using a MAC only shows that one of the parties who knows the shared secret key formed the MAC (for example shopper and merchant), and a third party (judge) will not be able to decide which of those two parties performed the action (and would also need the shared secret key to determine if the MAC was valid).


QUESTION 8
One application for digital signatures is code signing. Read the information about code signing here: https://www.digicert.com/faq/code-signing-trust/what-is-code-signing and use this to answer the following questions:
a) What is the signature intended to be used for (why would a software author sign their code - which security service/s does provide)?
b) Which key is used to create the signature?
c) Does the signature include the use of a hash function? (Look in the 'How Code Signing works' diagram.)
d) Which key is needed to verify the signature? How do you obtain the appropriate key values?

a) A verified digital signature on code validates the identity of the software author or publisher and verifies that the file has not been altered or tampered with since it was signed. [That is, there are

assurances about the authenticity of the sender and the integrity of the code. Additionally, the code signer cannot later deny authoring the code.]
b) The code should be signed with the software author's private key.
c) The code is hashed, and the output of the hash function (referred to as a digest, or fingerprint) is signed. This is done for efficiency purposes.
d) The signature was created using the signer's private key, so to verify the signatures you would need the associated public key. The code signer should make their public key available.

QUESTION 9
Cryptography is a useful security tool, but it can also be a threat to information security goals. Some common ransomware variants encrypt the files on a victim's computer, and then demand that the user pay a ransom to decrypt their files. In the last few years, there have been very damaging ransomware events. Visit the 'No More Ransom" organisation website (https://www.nomoreransom.org/en/index.html ) to find out more and answer these questions:
a) From the Ransomware: Q&A page, outline how a ransomware attack works.
b) The data locking function is actually encryption. From the section 'Why is it so hard to find a single solution against ransomware?' find out the type of encryption algorithms used for the early ransomware, and for newer versions.
c) How does the design of the current ransomware make it impossible for users to decrypt the files on their own?
d) When is it possible to decrypt files encrypted with ransomware?
e) Read the ransomware prevention advice and note the recommendations for regular users.
i. Classify the recommended measures as preventive, detective, or corrective.
ii. Determine whether the measures involve technology, policy and practice, or education, training, and awareness.

a) The attackers craft some malware which is usually included as an attachment to an email. When the attachment is opened the malware is released. The malware may not be immediately noticed by the user. It then 'locks' some of the user files and puts a message on the screen to tell the user that they will need to pay a ransom to unlock their data.
b) Early ransomware versions used symmetric key crypto. More recent ransomware uses asymmetric crypto. CryptoLocker is an example of ransomware that uses asymmetric crypto.
c) The public key is generated by the attacker's control server and used to encrypt files. The corresponding private key is held by the attackers, and never copied to the user's computer, so the user does not have access to the private key to decrypt the files. Unless they pay for it!
d) Decryption without paying for the key is sometimes possible - if the attackers make a mistake in their implementation, or publish the keys themselves, or if law enforcement agencies find the keys and share them.
e) Ransomware prevention advice includes:
1. Make regular backups so you can restore your data and don't have to be held to ransom. (Preparing a corrective measure, so you can restore if needed)
2. Don't click on links in spam, unexpected or suspicious emails. (Preventive)
3. Avoid sharing personal data (Makes you easier to phish - preventive)
4. Be meticulous with sensitive data - store on separate devices, use unique and strong passwords, update passwords, encrypt sensitive files (Preventive)
5. Use multifactor authentication on important accounts (Preventive)
6. When browsing, do not click on suspicious links, pop-ups or dialogue boxes. (Preventive)
7. Download official versions of software and from trusted websites (Preventive)
8. Use security products (things like AntiVirusSystems) with heuristic functions enabled, to pick up infection in the early stages. (Detective)
9. Don't connect unfamiliar USBs (Preventive)
10. Use a VPN when using public WiFi (Preventive)
11. Ensure security and OS software is up to date, since malware often exploits known vulnerabilities. (Preventive)
12. Do not use high privilege accounts for daily business (Minimize damage, if not prevent)

13. In Windows, Enable 'Show file extensions' and look at the sort of files - watch out for
.exe, .vbs, .scr filetypes. (detective)
14. Turn on local firewall (preventive)
15. If you discover a rogue process, disconnect your machine from other networks to stop the infection spreading, and more suggestions around response ... (minimize damage, prevent spread)

QUESTION 10
In January 2023, the Australian Cyber Security Centre (ACSC) published a ransomware profile of the Royal ransomware variant. [This is of special interest to QUT, as QUT was targeted by Royal in December 2022.] You can find the article here: https://www.cyber.gov.au/about- us/advisories/2023-01-asdacsc-ransomware-profile-royal. Use the information given in this article to answer these questions:
a) Why does Royal ransomware use encryption?
b) What is the 'double extortion' technique that Royal threat actors use?
c) What sort of techniques are used to gain initial access and install Royal software on victim systems?
d) When is the ransomware payload that encrypts the victim systems executed?
e) What actions do ASD/ACSC recommend to mitigate the risks of harm to organisations through ransomware incidents?

ASD's ACSC Ransomware profile:
a) Royal ransomware uses encryption to restrict access to corporate files and systems
- by encrypting them, the authorized users are locked out and the files are unusable
b) The double extortion technique is to
1. encrypt the files to prevent the organisation using them, but also to
2. threaten to sell the data or publically release the information if the victim does not meet the ransom demands.
c) Techniques used to gain initial access are:
a. Exploiting known vulnerabilities or common security misconfigurations
b. Making malicious downloads appear authentic by hosting fake installer files on legitimate software download sites
c. Using Google Ads in a campaign to blend in with normal ad traffic
d. Using contact forms on an organization's website to distribute phishing links
d) The ransomware payload that encrypts victim files is usually executed AFTER the threat actors have exfiltrated sensitive data from the victim's system. The ACSC Royal profile provides a great diagram illustrating the stages of the attack:



e) Recommended actions to mitigate harm are:
* Implement multifactor authentication to prevent actors from accessing valid accounts with stolen credentials
* Implement network segmentation and network traffic filtering to prevent actors from directly connecting to remote access services they have established for persistence

* Configure the Windows Registry to require User Access Control (UAC) approval for any PsExec operations requiring administrator privileges to reduce the risk of lateral movement by PsExec
* Implement hypervisor log monitoring and ensure that logs are processed on a separate system
* Implement application whitelisting (at least in monitor mode to capture unusual activity)
* Perform daily backups and keep them offline and encrypted
