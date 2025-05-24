IFB240 Cyber Security
Outline solutions for Week 5 tut. questions related to User Authentication

Essential definitions Review the de?nitions given in the lecture slides for the following terms:
IdentificationTokenAuthenticationBiometric systemAuthenticatorFalse matchHash function (for info/cyber security use)False non-matchHash valueMultifactor Authentication
QUESTION 1 - Knowledge-based authentication
Reusable passwords are a commonly used authenticator for computer systems. However, there are some problems associated with their use.
a) Briefly describe the problems associated with reusable passwords:
i. With respect to user requirements.
ii. With respect to system requirements.
b) Which of these problems are specific to user selected passwords?
c) Which of these problems are more commonly associated with computer generated
passwords?
d) Week 5 Activity 1 asked you to watch an Ellen de Generes YouTube video 'Out of your Password Minder', in which Ellen discusses a password protection device. Compare your answers to the questions in Activity 1 and your answers to part a) of this question.
i. Which of the problems you identified in part a) are discussed in the video?
ii. Which of the problems you discussed in part a) are not dealt with at all by the Password Minder?
e) Another product aimed at improving password security for users is a password manager. Read The Guardian article from 20 March 2022: 'Not using a password manager? Here's why you should be ...' (available at: Not using a password manager? Here's why you should be... | Data and computer security | The Guardian) and answer the following questions:
i. Which of the problems you discussed in part a) are reduced through use of a password manager?
ii. Which of the problems you discussed in part a) are increased through use of a password manager?
iii. Which of the problems you discussed in part a) are not dealt with at all by password managers?
f) How are the password managers discussed in the article different to the Password Minder that Ellen discussed? Do they have any advantages over the Password Minder?

a) See lecture slides, most common problems with respect to
i. Users:
a. May share password (intentionally or not)
b. Might forget their password
c. Often choose easy to guess passwords
d. Might write password down (store insecurely)

ii. System:
a. Storage of user password validation value needs to be secure (for all users)
b. Don't have non-repudiation if values are known to system also
b) All the problems listed above apply to user selected passwords.
c) Computer generated passwords:
a. stop users choosing weak or easy to guess passwords,
b. but users can still share or forget,
c. and if not word-like, it may be more likely password will be written down or forgotten (unless password managers are used).
d. Also, still need secure storage of verification values at system end.
d) Ellen video on Password Minder - protection at user end:
i. Problem dealt with is users forgetting passwords. Device is a book to write them all down in (instead of using post-it-notes).
i. Ellen comments that now all the passwords are in one place, this password protection device now requires protection. It's a funny video, but this is a real security issue! The security of all the passwords depends on the protection provided to the record book. You need to think about the threat source to decide what sort of protection is appropriate.
ii. Use of the password minder may minimize the threat of loss of access to online accounts (don't need to worry about user forgetting password), may possibly reduce threat of attacker compromise through password guessing (only if written down passwords are chosen more carefully than those that are committed to memory).
ii. The Password Minder does not deal with any issues related to the choice of passwords, it is focused on user storage - nor does it deal with the storage and handling of passwords by the systems in use at the organisations the user has accounts with.
e) A password manager:
i. Reduces the likelihood of
i. users picking easy to guess passwords - it generates stronger passwords than most users would select
ii. users reusing passwords at multiple sites - it creates unique passwords for each account
iii. users forgetting their password - they don't need to remember them, just the one required to authenticate them to the password manager!
iv. users writing passwords down and leaving them where they could be observed. The Password manager stores them securely (encrypted).
ii. If you forget the password that authenticates you to the password manager, you have lost access to all your passwords!
iii. The use of a password manager does not deal with any of the problems at the system end. It is only about how the user chooses and stores their passwords.
f) Essentially, a Password Manager is a digital version of the Password minder, stored in the Password Minder Protector, but with the added assistance of a password generation process. The threat source is different, though. For the physical book, you had to be physically present to access it. If the password

minder is on your device, and remote access is possible, then the threat source need not be local. Remember the video with Kevin Roose in the Week 2 video - the hackers gained access to his password manager!


QUESTION 2 - Passwords and expiration dates
One aspect of the use of passwords for authenticators is the length of time that a password should be used before being changed. Using the same password indefinitely may be considered insecure, as an attacker who learns your password will be able to continue to use it to access your account. Does changing your password often (every 30/60/90 days) really improve security? Information security expert Bruce Schneier's blog "Schneier on Security" (available at http://www.schneier.com/blog/ ) has a posting on August 5, 2016 regarding the security implications of frequent password changes (archived post available here: https://www.schneier.com/blog/archives/2016/08/frequent_passwo.html).
a) What strategy do users adopt when frequent password changes are required?
b) How does this strategy affect the security - did the changes make it difficult for security researchers to crack the passwords?
c) What proportion of accounts could researchers crack:
i. in online attacks, and
ii. in offline attacks?

Frequent password changes:
a) The users make only minor changes - substitute a digit for a letter, or add a digit at the end: Password#1, Password#2, etc.
b) This makes it easy for researchers to predict likely changes
c) The researchers findings were
i. In online attacks, 17% cracked in 5 or less attempts.
ii. In offline attacks, 41% cracked within three seconds.

QUESTION 3 - Hash functions used for password storage and verification
A common application of hash functions is for password verification. User passwords should not be stored in plaintext (just as the user provides it), although many organizations still do this.
a) Read the information 'How Websites (Should) Store Passwords' available here: How Websites (Should!) Store Passwords | BeCyberSafe.com and use the information to answer the following questions:
i. What is the major problem associated with an organisation storing user passwords in plaintext?
ii. Why is it better for organizations to store the hash values for user passwords, rather than the plaintext passwords themselves.
iii. Explain how authentication of the user is performed where the host system stores the hash value, rather than the actual password.
b) Although storing the hash values for passwords is better than storing plaintext passwords, this approach is still vulnerable.
i. Explain the vulnerability when (unsalted) hash values are stored.
ii. How do attackers exploit this?
iii. Want to find out how hard it is to crack unsalted hashes and recover passwords? Try Crackstation's 'Free Password Hash Cracker' available here: CrackStation - Online Password Hash Cracking - MD5, SHA1, Linux, Rainbow Tables, etc. and see how long it takes to recover the passwords from the

following hash values:
i. 42f749ade7f9e195bf475f37a44cafcb
ii. e10adc3949ba59abbe56e057f20f883e
iii. daa1f31819ed4928fd00e986e6bda6dab6b177dc
iv. 7af2d10b73ab7cd8f603937f7697cb5fe432c7ff
c) An even better option is for organizations to store salted hashes. Explain how user authentication is performed when salted hash values are used.
i. How does the use of a salt address the vulnerability that exists for unsalted hashes?
ii. Which hash function property is important for this?
d) Some regulators are now fining companies for poor management of data, including of user passwords. Read the Naked Security Article by Paul Ducklin: 'Serious Security: MD5 considered harmful - to the tune of $600,000' from 30 November 2022 and available at: Serious Security: MD5 considered harmful - to the tune of
$600,000 - Sophos News and use this to answer the following questions:
i. Why is the use of the MD5 algorithm considered problematic?
ii. Why was the lack of salting considered even worse?
iii. What does this article suggest is an appropriate choice of algorithms for secure password storage (right near the end)?

a) How Websites (Should) store passwords:
i. Major problem with storing plaintext passwords is that if the confidentiality of the password file is breached, then the passwords of all the users are exposed - and someone can log in as any of these users.
ii. If the hash value is stored, rather than the plaintext password, someone who gains access to the files can see the hash values of the passwords, but these are not the actual passwords and, since the hash function is one-way, the passwords cannot be computed from the stored hash value.
iii. If the hash value of the password is stored, rather than the plaintext password, authentication would be performed by:
1. User sends UserID and password to system they want to log in to.
2. Server computes hash value of received password.
3. Server looks up record for that UserID and compares computed hash value with stored hash value.
4. If they match, user is accepted as authentic; else rejected.
b) The vulnerability with using straight hash values:
i. Where the passwords are the same, the hash values will be also. If passwords were randomly chosen it would be difficult to find a match. But users don't choose randomly!
ii. Most attackers know the common passwords that users choose, so in practice they just hash these common passwords and look for matches with those hashes. Makes it easy to identify users who choose the common passwords (such as 123456 or Password123).
iii. Go on - try it out for yourself! ? 
c) Using salted hashes, the authentication is performed as follows:
1. User sends UserID and password.
2. Server look up record for that UserID, finds the user salt value.

3. Concatenates salt and received user password, and computes hash value for that input.
4. Compares computed hash value with stored hash value.
5. If they match, user is accepted as authentic; else rejected.

i. Using salted hashes, where the salt is a random number and different for every user, is a better option than unsalted hashes because it disguises the repetition of the actual passwords. The stored hashes will be different for two users with the same password, as long as the salt values are different.
ii. All the hash function properties are important, but when salts are introduced, we want even a small change in the input to cause a large change in the output (Property H4). Did you notice this effect in the Hash Function Exploration activity?
d) Poor security management including passwords:
i. MD5 is problematic because it is known to have collisions
ii. The lack of salting is bad because a pre-computed hash table of common passwords can be used for fast cracking (the approach used for Crackstation in Q3c)
iii. The recommended choice is PBKDF2 stretching algorithm with SHA-256 as the core algorithm, a per-user 128-bit random salt value and about 200,000 iterations.

     [Hint for Hash Function Exploration activity exploring one-wayness: Input text is from top of activity statement: Hash functions are commonly used for information security applications, such as checking message integrity and for password storage, to avoid storing plaintext passwords.]

QUESTION 4 - Poor password storage, password leaks and checking up
As a user, you trust other organizations to store your password securely. How do you gain insight into the process that an organization is using? A 'forgotten your password' link might reveal a process that is less than best practice, if your actual password is subsequently emailed back to you (that shows the organisation has access to your actual password).
a) According to the 'Plain Text Offenders' website (http://plaintextoffenders.com/),
i. What proportion of sites operate in this way (Check under the About tab)?
ii. Is storing passwords in plaintext a threat or a vulnerability? Explain your answer.
iii. If you find a plaintext offender, what are the two things that the Plaintext Offenders site recommends you do (Check under FAQ)?
b) Have any of your passwords been compromised without your knowledge? You can use Troy Hunt's 'Have I Been Pwned?' service to find out: https://haveibeenpwned.com/ You may need to change them - if you haven't already.

a) Plain text offenders:
i. Plain text offenders claim that over 30% of websites store user passwords as plaintext.
ii. This is a vulnerability. The related threat is that, if someone gains access to the vulnerable system, the password confidentiality will be breached. The exposed password could then be used in subsequent security events.

iii. If you find an offender, their recommendation is to
a. Submit the information to the Plain Text Offenders site, and then
b. Contact the offending organization and share the Plaintext offender FAQs with the organization.
**Responsible behavior: we suggest contacting the offending organization first.

QUESTION 5 - Object-based authentication
Hardware tokens are an example of object-based authentication - authentication based on
something you have.
a) The synchronised one-time password generator is one method to provide user authentication. Describe the operation of the synchronised password generator method using clock-based tokens.
b) Watch the video 'How do RSA SecureID tokens work' available at: http://www.youtube.com/watch?v=k_zpbJF9pmc.
i. Look carefully at the 6-digit display showing on the device. How often does it change?
ii. From the explanation given in the video, explain how the system manages a small loss of synchronisation (say, clock drift of one minute) between the device and the authentication server (about 3 minutes into the explanation).
iii. What is the probability that an attacker could guess the correct passcode (6- digit number) and gain access?
c) Read the section of the Wikipedia entry on SecureID http://en.wikipedia.org/wiki/SecurID that relates to the RSA security breach in March 2011. What are the hackers alleged to have obtained from RSA, and how would this information be of use to them?
d) Describe one major advantage and one major disadvantage for hardware tokens, when compared to standard user-selected passwords.
e) Compare the two token-based methods (clock based or counter based). What is a possible advantage of each compared with the other?

a) See the Part C lecture slides for this:
i. The user enters PIN which is used together with clock on token to produce the current value.
ii. The value changes for each time period. The user sends the current value to the host.
iii. The host computes the same value using the algorithm with inputs: user's ID, PIN and clock value.
iv. The host compares the received value with the computed value and accepts user as authentic only if the values are the same.
b) From the RSA SecureID video:
i. The 6 digit display changes every minute.
ii. If the clocks are not synchronized, the value sent will not be the same as the one the host is expecting. When values don't match, the host system calculates the value for the minute prior to time on the host clock, and one minute after. If one of these values matches, then the host system permits access and stores an offset value, so that it knows in future that the user module has a clock time different by that much from the host clock time.
iii. The value has 6 digits, so if an attacker is just randomly guessing a 6 digit number, there's a one in a million chance that they will guess it

correctly. (Allowing for the submission of the value before or after the expected value, it's 3 in a million that they gain access.)
c) The attackers in the RSA breach are alleged to have obtained the seed inputs for the RSA SecureID tokens (the set of symmetric keys - each device uses a unique symmetric key, and the key used is linked to the serial number on the device). If these values and the time and algorithm are known, the attackers can produce all of the 6 digit codes that the devices will display, without actually having the token, so could use this to gain access to protected systems.
d) Advantage: single use (one time) password is secure against password guessing or replay: reusable passwords are not. Disadvantage: problems if synchronisation between token and host is lost, also security issues around possible loss or theft of token.
e) A possible advantage of the clock-based tokens over counter-based is that the operation is relatively simple. A possible advantage of the counter-based tokens is that they do not require a synchronised clock.

QUESTION 6 - Biometric systems
Some methods for user identification and authentication make use of biometrics.
a) A basic biometric system consists of four main modules. Briefly describe these four modules.
b) A biometric system may operate in either verification mode or identification mode.
i. Briefly explain the operation of both of these modes.
ii. When the system is in use, which of these modes is likely to return a result faster? Explain your answer.

a) See the Part C lecture slides for diagrams:
* Sensor module: captures the biometric signal of an individual. An example is a fingerprint sensor that images the ridge and valley structure of a user's finger.
* Feature extraction module: processes the acquired biometric signal to extract a set of salient or discriminatory features. For example, the position and orientation of minutiae points (local ridge and valley singularities) in a fingerprint image are extracted in the feature extraction module of a fingerprint-based biometric system.
* Matcher module: features captured during recognition are compared against the stored templates to generate matching scores.
* System database module: used by the biometric system to store the biometric templates of the enrolled users.
c) See Part C lecture slides for modes of operation:
* In verification mode the user claims an identity. A new biometric sample is captured and compared to the stored template corresponding to the user's claimed identity. A decision is made on the closeness of the match, with respect to a set threshold value. The access request is accepted if the result is over the threshold value, or rejected if it is lower.
* In identification mode the user does not claim an identity. A new biometric sample is captured and a search is conducted of the templates of all the users in the database for a match.
* Identification is likely to take longer to return a result for an individual, as it requires a search of the database (n-to-1 comparisons) instead of the 1-to-1 comparison process to determine matching required for verification.

QUESTION 7 - Biometric authentication
Any human physiological or behavioural characteristic can be used as a biometric characteristic as long as it satisfies four basic requirements.
a) Briefly describe each of these four requirements.
b) For a proposed biometric system (a system that employs biometrics for personal recognition) there are three practical aspects that require consideration. These are Performance, Acceptability and Circumvention. Briefly describe what each of these three aspects considers.
c) An article in April 2019 describes problems with the fingerprint user authentication on a mobile phone: Phone fingerprint scanner fooled by chewing gum packet - Sophos News
[There are articles on similar flaws for other phones - search for your phone :)].
i. What were the problems users had with the Nokia 9 fingerprint scanner?
ii. What are the possible consequences of these problems?
iii. How do the false positives and false negatives mentioned in the article relate to FMR and FNMR? Which error does the article suggest is worse - in this phone scenario?
d) Read the Washington Post article by Andrea Peterson on September 23, 2015 about a security breach at the US Office of Personnel Management where fingerprint records were among the compromised data. (See https://www.washingtonpost.com/news/the-switch/wp/2015/09/23/opm-now-says- more-than-five-million-fingerprints-compromised-in- breaches/?utm_term=.11f1ad770867 . According to the article, why do some experts consider this breach worse than disclosure of passwords?
e) How well do you think each of the following biometric types satisfies the characteristics and issues you described for parts a) and b).
i. Fingerprints
ii. Facial recognition

a) The four requirements are:
i. Universality: each person should have the characteristic;
ii. Distinctiveness: any two persons should be sufficiently different in terms of the characteristic that it is possible to distinguish between them;
iii. Permanence: the characteristic should be sufficiently invariant (with respect to the matching criterion) over a period of time;
iv. Collectability: the characteristic can be measured quantitatively.
b) The practical aspects to consider include:
i. Performance: the achievable recognition accuracy and speed, the resources required to achieve the desired recognition accuracy and speed, the operational and environmental factors that affect the accuracy and speed;
ii. Acceptability: the extent to which people are willing to accept the use of a particular biometric identifier (characteristic) in their daily lives;
iii. Circumvention: how easily can the system be fooled using fraudulent methods.
c) The Nokia 9 phone users

i. Initially complained about a lot of false non-matches, so Nokia adjusted the fingerprint recognition software to allow more variability. The result was an increase in false matches.
ii. The consequence of false non-match is that the user is locked out of their phone (or has to enter a PIN) whereas the consequence of false match is that the phone would unlock for other people or things. (That is, after the adjustment it was not sufficiently sensitive to differences in the fingerprints). If authentication is based on the fingerprint alone, this method can clearly be used to circumvent the access control system for the phone. Multi-factor authentication, where the biometric is only one factor, would improve the security.
iii. False negative is false non-match, false positive is false match. In the phone situation, the article suggests that false match is worse as now someone else can use your phone.
d) Experts consider this leak of fingerprint data as worse than password disclosure because of the permanence of fingerprints. Also, the extent to which an attacker can make use of the fingerprints may increase as technology evolves, if they are more widely used.
e) Using ratings of high, medium and low, respectively, where high is the most desirable (for example, High for circumvention means that resistance to circumvention is high).

CharacteristicUniversalityDistinctivenessPermanenceCollectabilityFingerprintMediumHighHighMediumFacial recognitionHighLowMediumHigh
CharacteristicPerformanceAcceptabilityCircumventionFingerprintHighMediumMedium*Facial recognitionLowHighLow
Fingerprints: A small proportion of people do not have suitable fingerprints for identification because of genetics, age, environment or occupation, so universality is medium. Fingerprints are practically unique and permanent. But they might not be secret! Fingerprint scanners are affordable and appear on many commodity devices today. It is usually possible to collect a good sample but may not always be in adverse environments.
*There are a range of different methods used, and some are easier to circumvent than others. If many people can make usable copies of fingerprints, they can circumvent the access control system.

Facial recognition: Is non-intrusive and commonly used by humans. It scores well on universality and acceptability. There are different methods to obtain an accurate quantitative sample so collectability is good. Measurements can vary considerably with lighting and viewing angle which detracts from permanence. However, facial measurements on their own provide a questionable basis for identification, so uniqueness and performance are rated low. This also affects circumvention, particularly if the subject does not cooperate (for example by presenting a different viewing angle).

QUESTION 8 - Biometric errors
The matcher module in a biometric system computes a matching score s that quantifies the similarity between the user input and the template representation stored in the database.
a) Explain how the matching score s and the threshold t are used to determine mate pairs.
b) For the terms false match rate (FMR) and false non-match rate (FNMR)
i. Clearly explain what each term means.
ii. Give an example related to facial recognition to illustrate your explanations.
c) Explain how the FMR can be reduced.
d) Explain how the FNMR can be reduced.
e) Explain how the trade-off between security (low FMR) and practicality (low FNMR) is related to the threshold t.
f) Can you think of an example where
i. it is more important that the false match rate must be very low?
ii. it is more important that the false non-match rate is low?

a) Pairs of biometric samples generating scores s higher than or equal to t are inferred as mate pairs (i.e., belonging to the same person). Pairs of biometric samples generating scores lower than t are inferred as non-mate pairs.
b) Errors:
i. False match rate (FMR): the rate at which biometric measurements from two different persons are incorrectly declared to be from the same person. Example: the rate at which the system makes an error and decides the face of one person actually matches the stored template of a different person.
ii. False non-match rate (FNMR): the rate at which two biometric measurements from the same person are incorrectly declared to be from two different persons. Example: the rate at which the system makes an error and decides the face of one person does not match the stored template of that person, when it actually is that person.
c) Reduce FMR by increasing t.
d) Reduce FNMR by decreasing t.
e) Both FMR and FNMR are functions of the system threshold t. If t is decreased to make the system more tolerant to input variations and noise, then FMR increases. On the other hand, if t is raised to make the system more secure, then FNMR increases accordingly. So it's a tradeoff.
f) Want False Match Rate to be very low in high security situations where it is critical to only allow in the authorized person, and preferable to lock out an authorized user rather than admit unauthorized user. Say accessing the controls of a high security facility.
g) Want False Non-Match rate to be low in situations where it is important that the required user is not excluded, even if other candidates are included. Say scanning for a known criminal at a border checkpoint. Picking up many wrong candidates, and then going through the pool of possibilities and excluding them may be better than setting the threshold high and letting the criminal escape.

QUESTION 9 - Multifactor authentication
Mobile phones are increasingly being used as a component in providing two-factor authentication. Many online services (Google, Facebook, Amazon,...) now support two- factor authentication using one-time passwords with time-based tokens. The Australian Government's ACSC provides some information on multifactor authentication and some practical Step-by-Step guides for implementing MFA in commonly used products on their Protect Yourself: Multifactor Authentication guide, available here: Protect Yourself: Multi- Factor Authentication | Cyber.gov.au. Read through the provided information to answer these questions:
a) Which categories of authenticators do they include in their MFA explanation?
b) Look through the list of websites and apps that they provide instructions for setting up MFA. Are there products and services that you have used or are currently using?
c) Do you use MFA (at least, 2FA) with any of these? Investigate some of your own online accounts to see if you can set up 2FA to increase your login security.

Two factor authentication for online accounts
a) Authentication category examples are:
a. Something you know (a PIN, password or passphrase)

b. Something you have (a smartcard, physical token,
authenticator app [Will be installed on a device, so this is something you have],
SMS [Sent to a registered number, so something you have] or
email [Sent to a registered address or device, so something you have])

c. Something you are (a fingerprint, facial recognition or iris scan)

b) ACSC multifactor authentication - Look and see if there are instructions for things you use. There are Step-by-Step guides for setting MFA for Apple ID, Microsoft accounts, Gmail, ...Financial services (big 4 banks + more) Online shopping, Social Media, MyGov, Gaming ...

c) Improve your personal security for the accounts that matter to you. Remember that some (low value?) accounts may contain personal information that can be used in subsequent attempts (for example in spear phishing) to compromise other (high value?) accounts. That is, compromise of an account you don't value highly could be the start of a chain of events, with escalating consequences.
