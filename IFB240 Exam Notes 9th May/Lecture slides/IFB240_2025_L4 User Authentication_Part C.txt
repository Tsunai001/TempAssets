










IFB240 Cyber Security
Lecture 4: Part C
Other User Authentication Mechanisms

Dr Leonie Simpson lr.simpson@qut.edu.au

User authentication mechanisms
• User authenticators can be categorised as
- Knowledge-Based [Discussed in Lecture 4 - Part B]
• Something you know (should be a secret only the entity knows)
- Object-Based
• Something you have (physical item only the entity possesses)
- ID-Based
• Something you are (physical characteristic of person - biometric)
- Location-based
• Somewhere you are

• Multi-factor authentication uses combinations from multiple different categories of authenticators






• Object-Based (Something you have)
- Characterized by physical possession of a token
- Examples
• Magnetic swipe card
• Token used for generating access codes
- Advantages include
• Difficult to share (effort required to make a copy)
• If lost, the owner may realise - sees evidence of the loss
- Disadvantages include
• If lost, the finder can make use of the token

Tokens
• A token could be
- Physical key
- Swipe card
- An ID badge
- Your phone, receiving one-time codes to enter in another system
- Or a device that generates a sequence of one-time passwords
• Need password generators in the token and at host system synchronized to produce the same sequence of random passwords
- Two common methods:
• Clock-based tokens
• Counter-based tokens


• Operation
- Token display shows a constantly changing value
• Clock time used as input to algorithm calculating
display value
- To log in to system
• User provides ID, then types in current value on
token as authenticator
• Possession of token necessary to know correct value for the current time
• NOTE: Clocks in token and at host system must be synchronised


• Example: RSA SecurID
- Each RSA SecurID authenticator has a unique symmetric key (uses cryptography - more on this in later weeks)
- That key is used with a proprietary algorithm (SecurID Hash) to generate a new 6 digit code every 30/60 seconds
- The codes appear unpredictable and dynamic
• Difficult to guess correct code at given time

- Some tokens have an extra security feature: they require a PIN to access the display value
• Something you have, or something you know?




USER'S

HOST
























PIN


• Major limitation - requires synchronization
- System fails if clocks in token & host not synchronized
- CIA?
• For network usage, need to provide an acceptable window of time to allow for transmission and network delays
- If too short: may lock out legitimate users
- If too long: possible that an intermediate node may capture token value and then log in as user (MITM)


• Operation

Counter-based tokens

- Instead of a clock value, use an internal counter value
- Increment the counter with each successful login
- Token device generates 'password' value as a function of the
counter value and other internal data, without external inputs
• Example: HOTP
- HMAC-Based One-Time Password Algorithm
- Described in RFC 4226 (Dec 2005)
• http://www.rfc-archive.org/getrfc.php?rfc=4226
- Uses a shared secret value (stored on token) as shared key
- Value displayed on token is HMAC value of current counter value
- Extended to Time-based OTP (TOTP) in RFC 6238

Counter-based tokens - HOTP
OTP Generation



Tokens
• Security requirements for user
- Physical protection for token/device
- If PIN used to access device, then user must protect this as for knowledge-based authenticator
• Security requirements for system
- Information related to users to be stored securely
• Same calculation being performed at user end on token as at
host end, based on PIN, etc
- C: don't store PINs in plaintext
- I: what happens if unauthorised modification of stored
data occurs?
- A: need to be available when required

Object based authenticators
Tokens - breach
Security compromise - RSA SecureID
- March 2011 - announced SecurID token records breached
- Alleged that attackers gained remote access to RSA internal network via spear phishing emails
• Emails had malicious Excel attachments used to install remote
access tools
- Speculation (not confirmed by RSA) that attackers managed to access database containing seed values for all SecurID tokens - could reproduce displayed values
- Evidence of attempts to use these to access systems
- Consequence for RSA?
• replaced about 40,000,000 tokens for customers, reputation?

ID-based authenticators

• ID-Based: Something you are
- Characteristic unique to one person
- Examples include
• biometrics such as fingerprint, eye scan, voiceprint, signature
- Advantages include
• Characteristic can't be forgotten or lost
• May be difficult to copy, share or distribute
• Should require the person being authenticated to be present
at the time and point of authentication
- Disadvantages include
• Harder to replace a compromised biometric authenticator,
than to replace passwords or tokens
• Biometric systems costly

Biometrics and data breaches
• US OPM breach - June 2015
• https://www.opm.gov/cybersecurity-resource-center/#url=Cybersecurity-Incidents

• What is a biometric system?
- Automated methods of verifying or recognising a person based upon a physiological or behavioural characteristic
• Biometric characteristic examples
- fingerprint
- facial recognition
- eye retina/iris scanning
- hand geometry
- written signature
- voice print
- keystroke dynamics


• 4 Requirements for biometric characteristics
- Universality
• each person should have the characteristic
- Distinctiveness
• any two persons should be sufficiently different in terms of the characteristic
- Permanence
• the characteristic should be sufficiently invariant (with respect to the matching criterion) over a period of time
- Collectability
• the characteristic can be measured quantitatively


• Practical considerations
- Performance
• What is the achievable recognition accuracy and speed?
• What resources are required to achieve desired recognition
accuracy and speed?
• Are there operational and environmental factors affecting the accuracy and speed?
- Acceptability
• The extent to which people are willing to accept the use of a particular biometric identifier (characteristic)
- Circumvention
• How easy is it to fool the system using fraudulent methods?

Biometrics system components








• System components
- Sensor module: captures the biometric signal of an individual
• Example: fingerprint sensor that images the ridge and valley
structure of a user's finger
- Feature extraction module: processes the acquired biometric signal to extract a set of discriminatory features
• Example: feature extraction module of a fingerprint-based biometric system extracts the position and orientation of minutiae points (local ridge and valley singularities) in a fingerprint image

• System components
- System database module: used to store the biometric templates of enrolled users
- Users are included in biometric system database in enrolment phase
• Biometric characteristic of individuals scanned by a biometric reader to produce a digital representation (feature values) of the characteristic
• Quality check performed to ensure acquired sample can be reliably processed by successive stages
• Input digital representation is further processed by a feature extractor to generate a compact representation called a template
• May store multiple templates to account for variations


• System components
- Matcher module: features captured during recognition are compared against the stored templates to generate matching scores
• Example: matcher module of a fingerprint-based biometric system determines the number of matching minutiae between the input and the template fingerprint images
- reports a matching score s
- Matcher module also includes a decision making module which uses matching score to
• confirm a user's claimed identity (verification mode) or
• establish a user's identity (identification mode)


• Modes of operation
• Enrolment
• Analog capture of the user's biometric attribute
• Processing captured data to develop a template of user's attribute
• Store user templates in database
• Verification of claimed identity (1-to-1)
• Capture of a new biometric sample
• Comparison of the new sample with that of the user's stored
template
• Decision on access acceptance or rejection
• Identification (1-to-many)
• Capture of a new biometric sample
• Search database of stored templates for a match based solely on
the biometric

Biometrics - Enrolment mode










Source: Salil Prabhakar, Sharath Pankati, Anil K. Jain, Biometric Recognition: Security and Privacy Concerns
https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=22cfef1e3db4abc92e31a77057c854618d6421c0

Biometrics - Verification mode












2025

Source: Salil Prabhakar, Sharath Pankati, Anil K. Jain, Biometric Recognition: Security and Privacy Concerns
https://citeseerx.ist.psu.edu/document?repid=rep1&tIyFpeB=p2d4f&0doi=22cfef1e3db4abc92e31a77057c854618d6421c0	24

Biometrics - Identification mode









Source: Salil Prabhakar, Sharath Pankati, Anil K. Jain, Biometric Recognition: Security and Privacy Concerns
https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=22cfef1e3db4abc92e31a77057c854618d6421c0

Biometrics - Issues with errors
• Possible errors
- Two samples of the same biometric characteristic from the same person (for example, two impressions of a user's right index finger) are not exactly the same due to
• imperfect imaging conditions (e.g. sensor noise and dry fingers)
• changes in a user's physiological or behavioral characteristics (e.g. cuts and bruises on the finger)
• ambient conditions (e.g. temperature and humidity) and
• user's interaction with the sensor (e.g. finger placement)
- Captured features compared with stored template to generate matching scores - used for decision making, so variations can result in decision errors

Biometrics - Two types of decision error
• Reject legitimate user
- If we expect sample to be exact match with stored template, then any variation leads to rejection of legitimate user
- To reduce possibility of rejecting a legitimate user, may adjust system to tolerate some variation between captured features and stored template
• This introduces another possible error
• Accept unauthorised user
- An unauthorised user may be able to provide a sample with captured features similar enough to those of the stored template for a legitimate user that unauthorised user can masquerade as the legitimate user
• Recent cases demonstrate this for iPhone and Samsung
Galaxy

Biometrics - Describing error types
• Biometric verification systems can make two types of errors in decision making
- False match
• mistaking biometric measurements from two different persons to be from the same person (results in allowing unauthorised person access)
- False non-match
• mistaking two biometric measurements from the same person to be from two different persons (so rejecting legitimate user)
- Trade-off between false match rate (FMR) and false non-match rate (FNMR) in every biometric system

Biometrics - Error types and tradeoffs
• The system decision is tuned by a threshold t
- Pairs of biometric samples generating matching scores s higher than or equal to t are inferred as mate pairs (system decides it is the same person)
- Pairs of biometric samples generating scores lower than t are inferred as non-mate pairs (system decides it is from different persons)
• Both FMR & FNMR are functions of threshold t
- If t is decreased
• to make the system more tolerant to input variations and noise, then FMR increases
- If t is raised
• to make the system less tolerant of variation, then FNMR
increases

Location-based authenticators
• Location-based (Somewhere you are)
- Characterized by your location in space and/or time
- Examples
• Use of location and tracking technologies
- triangulation of cell-phone signals, or global positioning systems (GPS)
• Machine IP address and DNS name
• Link location to time
- Advantages include
• Can improve network security, if access locations are (relatively) local
- Disadvantages include
• Privacy issues (more on this later in the semester)
- who should know where you are, when?


• Combines authentication techniques from two or more
different categories
- Aim: stronger and more reliable than single factor
• Most commonly used
- Two-factor authentication (2FA) based on
• something a user knows (factor one), plus
• something the user has (factor two)
- Frequently used combination is password and token
• Example: password and verification code sent to mobile phone (ie phone as token)
• Example: PIN and swipe card


2025	IFB240	31


• Multifactor authentication
- Offers potential for increased security compared to single factor
• If a criminal manages to obtain one item used as an
authenticator
- such as your password,
• then they will still need to obtain and use the other required
factors to gain access to your account
- so better security than a password alone
- Australian Cyber Security Centre (ACSC) advises MFA is one of the most effective ways to protect valuable assets against unauthorised access

Summary
• User authentication
- Process used to decide whether the identity a user claims is
genuine (authentic) or not
• Important to ensure authentic users if you use identity for
- Access control decisions
- Accountability measures
• Common access control mechanisms
- Knowledge based - Passwords
- Object-Based - Tokens
- ID-Based - Biometrics
• Advantages and disadvantages for each type
- Cost, level of security provided, user acceptability, etc
- Security requirements for both user and system
• Multifactor authentication can provide greater assurance


































































