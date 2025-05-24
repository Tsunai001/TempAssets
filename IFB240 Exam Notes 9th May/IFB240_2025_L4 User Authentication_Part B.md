IFB240 Cyber Security
Lecture 4 – Part B
Knowledge based authenticators
123456

password

111111

qwerty

Dr Leonie Simpson
lr.simpson@qut.edu.au

abc123

User authentication mechanisms
• Knowledge-Based (Something you know)
– Characterized by secrecy or obscurity
• Should be something only the entity knows

– Commonly used
• Passwords
– Especially user selected reusable passwords
• Personal Identification Number (PIN)
• Responses to security questions
– your birth date, mother’s maiden name, pet’s name, etc

– Advantages include
• Readily accepted by users
• Low-cost implementation
2025

IFB240

2

Knowledge based authenticators
Passwords
• Reusable passwords
– the most commonly used authenticator
– User provides
• username or ID, and
• password

– System has prior stored value to compare with
• Providing required value authenticates user to system

• Requirements
– User must store their password securely (think CIA)
– System must store values used to verify passwords
for all system users securely (think CIA)
2025

IFB240

3

Knowledge based authenticators
Passwords - reusable
• Reusable passwords - disadvantages
– User may forget password (so locked out unless reset)
– Passwords can be shared with others by user
– May be compromised without user knowledge
• Others may know or be able to guess
• Difficult for user to know if compromised

– Threats to password confidentiality
1.
2.
3.
2025

Attacker guesses user password
Attacker steals password from user (observes on post-it
note, obtains via keylogging malware, phishing, …)
Attacker steals a password database from a server
IFB240

4

Knowledge based authenticators
Passwords - reusable
• Easy to guess passwords: March 2021 example
•

SolarWinds blames intern for weak ‘solarwinds123’ password | IT PRO

2025

IFB240

5

Knowledge based authenticators
Passwords – stolen and leaked!
• Attackers steal password database

2025

IFB240

6

Knowledge based authenticators
Passwords – stolen and leaked!
8.3 million plaintext passwords exposed in DailyQuiz data breach - The
Record by Recorded Future

2025

IFB240

7

Knowledge based authenticators
Passwords - leaked
• Have any of your passwords been leaked?
– Check if you have an account with a password that
has been compromised in a data breach
– ‘;-- Have I Been Pwned? https://haveibeenpwned.com/
• Aggregation of many password database breaches
• See if your accounts are compromised – and when

– Are you using a known/familiar password?
• Check https://haveibeenpwned.com/Passwords
• Another way to search the same database, by using
passwords as the search key
• Good infosec awareness raising tool – test out some
passwords!
2025

IFB240

8

Knowledge based authenticators
Passwords – security requirements
• Security requirements for users
– Use a ‘strong’ password
• Aspects include minimum length, character set, prohibiting
use of identifiers or known associated items as passwords,
limitation on length of time before password change required

– Store password securely
• Not on a post-it note on your monitor 

– Don’t share password with other entities
• Colleagues, friends, family, etc

– Don’t use same password for multiple systems
• Different unrelated passwords for work/study, online banking,
social media, etc
2025

IFB240

9

Knowledge based authenticators
Passwords – security requirements
• Reusable password selection strategies
– User selected, or
– Computer generated
• For user selected passwords, security policy should include
– User training
• Explain importance of choosing ‘strong’ passwords
• Explain importance of using unique passwords for each account

– Password selection guidelines
• What are the characteristics of ‘good’ passwords?

• Policy alone unlikely to be effective in many organisations
– Especially if large user population or high turnover of users
– Some users ignore guidelines, or can’t select ‘strong’ passwords
– Many choose passwords that are too short and very easy to guess
2025

IFB240

10

Knowledge based authenticators
Passwords – lessons from breaches
• Imperva paper: Analysis of user selected passwords
– http://www.imperva.com/docs/WP_Consumer_Password_Worst_Practices.pdf

– December 2009 security breach at Rockyou.com
– Attacker retrieved and posted 32 million passwords on
Internet (Passwords were stored in database as plaintext)
– Imperva analysis of the password list shows many
users make poor choices:
• About 30% of passwords length less than or equal to six characters.
• Almost 60% of passwords used characters from limited alpha-numeric
set
• Nearly 50% of users used names, slang words, dictionary words or
trivial passwords (consecutive digits, adjacent keyboard keys, and so
on).
– Most common password: “123456”
2025

IFB240

11

Knowledge based authenticators
Passwords – lessons from breaches
• Imperva paper: Analysis of user selected passwords
– Extract from p 4: Table of 20 most common passwords

2025

IFB240

12

Knowledge based authenticators
Passwords – more analysis
• Similar analysis of user selected passwords
– Password data from Cupid Media data breach 2013
–

2025

http://krebsonsecurity.com/2013/11/cupid-media-hack-exposed-42m-passwords/comment-page-1/

IFB240

13

Knowledge based authenticators
Passwords – alternative to user-selected
• Computer generated passwords
– Avoids the problem of users choosing weak passwords
– But now have another security problem …
• Passwords consisting of random characters difficult for users
to remember
• User may need to write them down
– Common locations:
» Sticky note on monitor
» Under mouse pad
» In top desk drawer
» In diary or phone (notes?)
– Better option may be a password manager

• Also doesn’t solve problem of breach from stored location
– Still important to use unique passwords for each account
2025

IFB240

14

Knowledge based authenticators
Passwords – security requirements
• Security requirements for system
– Need to store passwords securely
• System password files are valuable information assets, so
password files need to be protected
– C: don’t store passwords as plaintext
– I: unauthorised modification of password file detectable?
– A: need to be accessible when required for verification

– Note: no non-repudiation if password is known to
system (or to others outside the system)
– Ideally, users should not use their password on one
system for accounts on other systems
• but enforcing this is largely outside of system control
2025

IFB240

15

Knowledge based authenticators
Passwords – security requirements

• Protecting passwords
– Reusable passwords require confidentiality when in
• Storage (on authentication server)
• Transmission (between client and server over network)
• Use (do not display on screen when being entered!)

– If ‘clear’ or plaintext passwords are captured, attacker
may reuse the password and masquerade as the user
• Http basic authentication effectively transmits ‘clear’ passwords

– Also, attackers may masquerade as the server, and
trick the client into disclosing ‘clear’ password to the
rogue server (some phishing attacks)
2025

IFB240

16

Knowledge based authenticators
Passwords - secure storage
•

Reusable passwords & storage strategies
– System password file has entries for each user
•

Example:

User ID: Leonie, Password: myPassw0rd

– Better alternative to storing plaintext passwords?
1. Store the hash values of passwords
Example:

Leonie A422BE0E206A05BF03061140E4942382

2. At login, I provide username and password
•
•

System hashes the password I provide
Compares computed hash value with hash value stored in the
password file as the entry corresponding to my username

– Advantage: If password file is disclosed, attacker gains
a list of hash values, not actual passwords
2025

IFB240

17

Knowledge based authenticators
Passwords – storage using hashes
• Q: What do you mean – hash value?#?!
• A: The output of a hash function
– A hash function H is a transformation
• takes as input a message M of arbitrary length
• produces as output the fixed-length value H(M) called the
hash value (or message digest, or checksum, or fingerprint)

…M…

Hash Function

H

Message of arbitrary
length
2025

IFB240

H(M)

Fixed length
output
18

Knowledge based authenticators
Hash function properties
• Four important hash function properties
– H1: Fixed length output H(M)
for arbitrary length input M
– H2: H(M) is one-way
• given M, it is easy to compute H(M), but given H(M), it is
infeasible to compute M

– H3: H(M) is collision-resistant
• Hard to find 2 distinct messages M and M’ with H(M) = H(M’)

– H4: If you make a small change in M, it produces a
major (unpredictable) change in H(M)
2025

IFB240

19

Knowledge based authenticators
Commonly used hash functions
• MD5
– Produces a 128-bit hash value
– * MD-5 is not regarded as secure - it has multiple vulnerabilities

• SHA-1
– produces a 160-bit hash value

• SHA-2 set of hash functions
– output lengths 224, 256, 384, and 512
(write as SHA-256, SHA-384, etc)

• SHA-3 set of hash functions
– has same output lengths as SHA-2
– standardized August 5, 2015
2025

IFB240

20

Knowledge based authenticators
Passwords – secure storage using hashes
•

Reusable passwords & storage strategies
– Problem with storing hash values of passwords
•

•
•

•
–
2025

Suppose my ID and password are
– Leonie
myPassw0rd
Suppose system stores MD5 hash of this value in the file
– Leonie A422BE0E206A05BF03061140E4942382
Suppose another entry in the password file is
– Ali
A422BE0E206A05BF03061140E4942382
What information does this give about the passwords for
Leonie and Ali?

*only using MD5 in example as the 128-bit hash value fits on the slides
IFB240

21

Knowledge based authenticators
Passwords – secure storage using hashes
• Better solution: store salted hash values of passwords
– Salt is random but not secret information, different for each user
– Concatenate user salt value & password, then hash
• Example:
– Leonie and Ali both used password: myPassw0rd
• System has assigned different salt values: Leonie 86, Ali 44
• Compute the hashes (we will prepend the salt values)
• For Leonie, the system stores the hash value for ‘86myPassw0rd’
• For Ali, the system stores the hash value for ‘44myPassw0rd’
• System database has these entries:
• Leonie
86
427B050A20B5EB9301A6957C80A7E9B5
• Ali
44
307EB0FB17CB005AE4C7980CA8E266A0

– Salts are unique → so hashes are different even if password is not
- Harder for attackers to spot users with same password
2025

IFB240

22

Knowledge based authenticators
Passwords – secure storage using hashes
• Attackers capturing databases with stored
– password hashes, or
– salted password hashes

use common passwords, try them with different salts &
compare hashes they compute with database for matches
• Even better solution: store stretched salted hash
values of passwords
– Slow attackers down by using an iterative process for hashing,
using thousands of iterations
• Known as stretched salted hashes
– Common algorithms doing this: bcrypt, scrypt, PBKDF2
2025

IFB240

23

Knowledge based authenticators
Example: Poor password storage
https://news.sophos.com/en-us/2022/03/21/web-vendor-cafepress-fined-500000-for-giving-cybersecurity-a-low-value/

2025

IFB240

24

Knowledge based authenticators
PINs and Passcodes
• Consider 4-digit PINs where user is free to choose PIN
– Number of possible options:
• 10 x 10 x 10 x 10 = 10,000
– Examples:
• 0000, 0001, 0002, 0003, … , 9998, 9999

• If users select randomly, then the chance an
attacker guesses user passcode correctly on
first guess is 0.0001
2025

IFB240

25

Knowledge based authenticators
PINs and Passcodes
• Do users choose at random?
• ZDNet article in June 2019 reports on research by Tarah Wheeler
•

Stop using terrible PIN codes! | ZDNet

2025

IFB240

26

Knowledge based authenticators
PINs and Passcodes
• Do users choose at random?
• ZDNet article in June 2019 reports on research by Tarah Wheeler

• Most common 4-digit PINs:

PIN

% of
participants

1234

11

1111

6

0000

2

1212

1

• Others in the top 20 list include
7777, 1004, 2000, 4444, 2222, 6969, 9999, 3333, 5555, 6666, 1122, 1313, 8888,
4321, 2001, 1010

2025

IFB240

27

Knowledge based authenticators
Security questions
• Knowledge based authenticators should be something
that only the user would know
• How do these questions measure up?
– What is your mother’s maiden name?
– What city/town were you born in?
– What model was your first car?
• September 2016 Wired paper by Lily Hay Newman
•

Time to Kill Security Questions—or Answer Them With Lies | WIRED

2025

IFB240

28

Knowledge based authenticators
Passwords, PINs and problems
• Default and hard-coded
passwords
– Many password-protected
vendor-supplied software
and hardware has default
passwords
• Users may not be
prompted to change
on setup
• Sometimes not
possible to change
default (hard-coded)
– Example: ZDNet article, Catalin
Cimpanu, January 14, 2019
2025

IFB240

29

Summary
• User authentication
– Process used to decide whether the identity a user claims is
genuine (authentic) or not

• Most common authenticators are knowledge-based
– Reusable passwords widely used

• Advantages
– Cost, ease of implementation, user acceptability, …

• Security requirements for both user and system
– Problems if users choose poorly, store poorly, reuse across
multiple accounts and systems, …
– Problems if transmission or storage are insecure
– Problems with default and hard-coded passwords
2025

IFB240

30

