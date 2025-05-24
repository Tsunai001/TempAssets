IFB240 Cyber Security

Outline solutions for tutorial questions for L7: Symmetric Cryptography

Essential definitions
Review the de?nitions given in the lecture slides for the following terms: 
CryptographyEncodingCryptanalysisDecodingPlaintextSteganographyCiphertextSymmetric cipherEncryptionStream cipherDecryptionBlock cipherCryptographic keyMessage Authentication Code
QUESTION 1 - Encoding
A Sophos blog post by Mark Stockley in April 2016 describes an access control issue that involves both an Insecure Direct Object Reference vulnerability (recall IDOR was discussed in Week 6 tutorial, Q7) and the use of encoding rather than encryption. Read through the article (available here: https://news.sophos.com/en-us/2016/04/28/the-flaw-that-left-as-websites-and-owners-exposed-for-at-least-16-years/) to answer the following questions:
a) What is the information asset that is affected?
b) What state is the information in?
c) How was the domain name in the URL represented?
d) Why is this regarded as poor practice? 
e) How can this vulnerability be exploited?
f) Which security goals can be breached?

a) This issue is a flaw in the website of the American Samoa domain registry, and the information asset affected is the records of any domain name accessible through that website.
b) The information is stored.
c) The domain name in the URL was base64 encoded. [Recall from Week 8 Activity 3 that encoding and decoding are processes performed by following an algorithm - no secret key is required. A glance at the Base64 encoding of a message may not immediately reveal the message contents, but it is very simple to recover if you want to, so this is no substitute for encryption.]  
d) As this is easily recognized and easily decoded, this provides no protection - it is clear to an attacker that this section of the URL represents the object being referenced (direct object reference). 
e) The URL is under the control of the browser user, so can be changed by a user from a domain they should be able to access to one that they shouldn't (but can), with obvious security implications given the direct access to the object. 
f) Could breach Confidentiality (see domain records including unencrypted passwords), Integrity (buttons to [Modify]) and Availability (buttons to [Delete]).


QUESTION 2 - Comparing encoding and encryption: 
Reflecting on your answers to the questions in Activity 3 of this week's preparation (on encoding and encryption), 
a) What is the main difference between encoding and encryption? 
b) Who can perform: 
i. Decoding?  
ii. Decryption? 

a) Hopefully working through Week 8 Activity 3 reinforced the idea that both encryption and encoding use an algorithm, but the encryption process also requires knowledge of a secret key (Lecture 7 Part A slide 9). 
b) Following on from part a) 
i. Anyone who knows the algorithm can decode, but 
ii. Only those who know both the algorithm and the secret key can decrypt (unless it is a small key size so you can try every possible key, or the algorithm is weak enough that you can break the cipher). The Caesar cipher has both a small key size and a weak algorithm, so it is very insecure! Do not use this for anything other than demonstrating terminology ??

QUESTION 3 - Types of symmetric ciphers
Symmetric ciphers are often used to provide confidentiality for messages. 
a) Why is the term 'symmetric' used for these ciphers? What aspect of the operation has symmetry?
b) There are two main categories of symmetric ciphers: stream ciphers and block ciphers. What is the major difference in the way messages (plaintext or ciphertext) are processed by these different categories of ciphers?
c)  What sort of applications are stream ciphers used for? 
d) What sort of applications are block ciphers used for?

a) The symmetry refers to the requirement that the key used for encryption of the plaintext and the key used for decryption of the ciphertext are the same (Lecture 7 Part A, slide 23).
b) The main difference in the way messages are processed is: 
a. Stream ciphers treat the message (plaintext or ciphertext) as a stream of characters and combine each character with a keystream character. Usually the plaintext, ciphertext and keystream are binary streams, and the combining operation is XOR. 
b. Block ciphers treat the message (plaintext or ciphertext) as a series of blocks (usually 64 or 128 bits) and process them (encrypt/decrypt) as a block. For block ciphers the key and the block are inputs to the block encryption/decryption algorithm.
The distinction can be a little blurred sometimes - particularly for some block cipher modes of operation that effectively work as keystream generators (We did not discuss these in our lecture, but there are some well-known ones: CFB, OFB, CTR).
c) Stream ciphers are generally used for real-time applications on data streams: video and audio (pay TV and mobile telephony) because they are fast and do not result in a noticeable delay in processing that would degrade the user experience.
d) Block ciphers are usually used for bulk encryption where some small delay is tolerable, for example: encrypting data files, data bases, disk encryption, email.

QUESTION 4 - Using a binary additive stream cipher:
Suppose that a binary additive stream cipher is to be used to encrypt the 9-character message 'My Secret'. The table below may be useful in recording your answers: some cells have been completed for you.

a) First, encode this message using 8-bit ASCII (The standard ASCII character set you used in Activity 3 uses only 7 bits per character but, since modern computers use 8-bit bytes, extended ASCII represents those characters as 8-bit bytes with the most significant bit set to 0, and includes 127 more 8-bit characters, where the most significant bit is set to 1.) to obtain a binary string. (Use the online tool at http://string-functions.com/string-binary.aspx  for this). 
b) Then encrypt using the keystream 01111000  00100000  01101010  01110101 01101101  01110000  00100000  01110100  01101000. (Recall for binary additive stream ciphers the encryption function is XOR.) Record your ciphertext in the table below.
CharacterMySecretASCII encoding01001101 011110010010000001110100Keystream01111000 0010000001101010011101010110110101110000001000000111010001101000Binary Ciphertext0011010100011100
c) What must the recipient of the ciphertext do to decrypt the ciphertext and recover the message?
d) Perform the decryption. Recover the message.
Binary ciphertext 
00110101 Keystream01111000 0010000001101010011101010110110101110000001000000111010001101000Recovered binary stream 
01001101Recovered plaintext
M
e) Suppose the ciphertext was altered in transmission, with the last 8-bit ciphertext block changing to 00001100. What difference does this make to the recovered plaintext?
a) and b):
CharacterMySecretASCII encoding01001101 0111100100100000010100110110010101100011011100100110010101110100Keystream01111000 0010000001101010011101010110110101110000001000000111010001101000Binary Ciphertext001101010101100101001010001001100000100000010011010100100001000100011100
c) Recipient needs to use same keystream in same position with respect to ciphertext (synchronized), and XOR ciphertext and keystream to recover plaintext. For d) see table:
Binary ciphertext 
00110101 
01011001
01001010
00100110
00001000
00010011
01010010
00010001
00011100Keystream01111000 0010000001101010011101010110110101110000001000000111010001101000Recovered binary stream 
01001101
01111001
00100000
01010011
01100101
01100011
01110010
01100101
01110100Recovered plaintext
M
y
S
e
c
r
e
te) If last block of ciphertext is altered:
Binary ciphertext 
00110101 
01011001
01001010
00100110
00001000
00010011
01010010
0001000100011100
00001100Keystream01111000 0010000001101010011101010110110101110000001000000111010001101000Recovered binary stream 
01001101
01111001
00100000
01010011
01100101
01100011
01110010
01100101
01100100Recovered plaintext
M
y
S
e
c
r
e
d

QUESTION 5
In this question you will use a block cipher (DES) to encrypt a very repetitive message. The block cipher can be used in ECB mode, or in CBC mode. Try out the online DES tool at
http://des.online-domain-tools.com. As you create the ciphertexts, save them in a text file, so that you can use them for question 6.
a) Start with a very repetitive plaintext message in hex: aaaaaaa... (at least 64 a's). Set the key to 0123456 (plaintext).
i. Encrypt in ECB mode. Record the result.
ii. Encrypt in CBC mode. Set the Init. Vector to 0000000000000000. Record the result.
b) Change to a slightly varied but still repetitive plaintext: aaaaaaaaaaaaaaaabbbbbbbbbbbbbbbbaaaaaaaaaaaaaaaabbbbbbbbbbbbbbbb   (16 a followed by 16 b followed by 16 a followed by 16 b characters). 
i. Encrypt in ECB mode. Record the result.
ii. Encrypt in CBC mode. Set the Init. Vector to 0000000000000000. Record the result.
c)   Change again to another slightly varied but still repetitive plaintext: aaaaaaaaaaaaaaaabbbbbbbbbbbbbbbbaaaaaaaaaaaaaaaacccccccccccccccc   (16 a followed by 16 b followed by 16 a followed by 16 c characters). 
d) Explain what you see. Which mode 'hides' the plaintext information more completely: ECB or CBC mode? How does this relate to the diagrams in the lecture slides for block cipher modes?
e) Change the function from DES to another encryption function, say AES. Repeat parts a) to d).
f) Try another encryption function - say RC4 (ARCFOUR).


d)   CBC mode 'hides' the information better. For ECB mode, repeated plaintext blocks appear as repeated ciphertext blocks. That doesn't happen in CBC mode, because of the cipher block chaining. 


QUESTION 6
Use the ciphertexts that you created in Question 5 for this question. For the
a) binary additive stream cipher RC4, paste the ciphertext you created in Q5f) into the input text box, 
i. Use the >Decrypt! button to recover your plaintext;
ii. Alter the ciphertext by one bit (say, change the first byte of the ciphertext from de to df, leaving the rest unchanged)
iii. Use the >Decrypt! button to recover the plaintext corresponding to this altered ciphertext;
iv. How different is this recovered plaintext from the original plaintext? 
b) block cipher operating in electronic codebook (ECB) mode; paste the ciphertext you created in Q5 a) into the input text box, 
i. Use the >Decrypt! button to recover your plaintext;
ii. Alter the ciphertext by one bit (say, change the first byte of the ciphertext from 3e to 3f, leaving the rest unchanged)
iii. Use the >Decrypt! button to recover the plaintext corresponding to this altered ciphertext;
iv. How different is this recovered plaintext from the original plaintext?
c)   block cipher operating in cipher block chaining (CBC) mode, paste the ciphertext you created in Q5 b) into the input text box, 
i. Use the >Decrypt! button to recover your plaintext;
ii. Alter the ciphertext by one bit (say, change the first byte of the ciphertext from 3e to 3f, leaving the rest unchanged)
iii. Use the >Decrypt! button to recover the plaintext corresponding to this altered ciphertext;
iv. How different is this recovered plaintext from the original plaintext?
d) Summarize your findings regarding the effect on the recovered plaintext if a single ciphertext bit of a received ciphertext message has been modified (changed, not deleted). When decryption is performed, how many bits in the decrypted plaintext would be expected to be in error in each of the following cases:
i. Binary additive stream cipher
ii. Block cipher in ECB mode
iii. Block cipher in CBC mode

Summary of effect of bitflip error:
a) For a stream cipher, only one received plaintext bit is wrong (see Lect 7 Part B slide 19). This might affect a character in the decoding, however (as seen above).
b) For ECB mode, the whole block will be decrypted to a random string. On average, half of the decrypted received block will be wrong (see Lect 7 Part B slide 30).
c) For CBC mode, the whole block will be decrypted to a random string as in ECB mode. In addition, the one bit of error will be fed forward in the decryption process (due to the chaining of the block) so that there will be a one-bit error in the following decrypted block. All other blocks will be decrypted correctly (see Lect 7 Part B slide 35).

QUESTION 7
Suppose now that a single ciphertext bit of a received message has been deleted. Repeat the exercise in Question 7 but delete a bit instead of flipping it. Observe the effect on the recovered plaintext. What happens if:
a)  The cipher is a binary additive stream cipher;
b)  The cipher is a block cipher operating in electronic codebook (ECB) mode;
c)   The cipher is a block cipher operating in cipher block chaining (CBC) mode.

Deletion error:
In all cases (for both a stream cipher and a block cipher) the output will look random for as long as synchronization is lost between encryption device and decryption device. For the stream cipher, this happens at the exact bit position where the bit has been deleted. For block ciphers, it will happen for the block in which the deleted bit should be and could continue indefinitely after one bit is lost in the ciphertext.

If it was a block cipher in ECB mode and a whole block was deleted, then the recovered plaintext would just be missing the corresponding plaintext block, and you would not necessarily detect this.

QUESTION 8 
*Hash functions are commonly used for checking message integrity. A common application of hash functions is to produce a 'checksum', 'fingerprint' or 'message digest' of an electronic document or file. Suppose you receive a document and a SHA-1 hash value intended as the document 'fingerprint'.* 
a) How can you (the recipient) make use of the 'fingerprint', and 
b) What assurance can be obtained from it?
c)  Use the internet to locate a SHA-1 demonstration tool. (There's one at http://hash-functions.online-domain-tools.com/). Check the SHA1 value for the text in this question between but not including the asterisks (*). Which one of the following values matches the SHA-1hash value you obtain?
i. 2a773b81af649f818c9fd6e4ed0c528531229b94
ii. a4596cf86cf8d28708b38eb4655b0e5778987d74
iii. 6c02e3e8c23ae91836ca40dbae42f69f2ff3d3de
d) Now check the SHA-256 value for the same text. Which one of the following values matches the SHA-256 hash value you obtain?
i. 65e587a9daf25f87807ebd582485ab05c1926a6590f60fc8bf67c02cd94349bc
ii. e7921c9d604102d49dd8fd1917959270bcaba67738d465c4b609c3b2edf5b25f
iii. fb283ee3e8dd0b5b223c1ae8ef0ace05c8d9033c4ea90b0b75d3c95c8278e780

a) You use the same hash algorithm to compute the hash for the document you receive, and compare with the received hash value, or fingerprint. If the values match, you assume the document is unaltered.
b) You have some assurance that the document has not been accidentally altered. A smart attacker who deliberately alters the document would probably recalculate the hash (since it does not require knowledge of a key) to suit the altered document and replace the old hash value with the new one. This means that you cannot rely on the application of unkeyed hash functions to pick up intentional modifications from attackers who are aware of the limitations of dedicated hash functions.
c) Matches ii.
d) Matches i.

QUESTION 9 
Alice wants to send a message to Bob and wants Bob to be able to check that the message did not change in transit. Alice and Bob have decided to use a MAC rather than a hash function like SHA-256.
a) What advantage is there in using a MAC rather than a dedicated hash function?
b) List the series of cryptographic steps that Alice must follow to create a MAC.
c)   What does Alice need to send to Bob?
d) List the series of cryptographic steps Bob must follow to verify the MAC.
e) What assurance does Bob get about the integrity of the message from Alice? 
f)  What sort of control measure is a MAC: preventive, detective or corrective?

a) Advantage: the MAC requires the use of a key, so an active attacker who alters the message should not be able to provide a valid MAC for the altered message.
b) Alice:
1. Generates message M 
2. Generates MAC = HK(M) from M using the hash algorithm H and key K 
3. Sends the pair {M, MAC} to Bob
c)  Bob:
1. Receives {M', MAC} 
2. Generates MAC' from M'. 
3. Compares the calculated MAC' and the received MAC  
4. If MAC ? MAC' then assured message has been altered; otherwise Bob assumes message is unchanged in transit.
d) If the MAC does not match, Bob knows that the message has been altered. If it does match, Bob accepts that the message is unaltered.
e)  Bob has some assurance that a message with valid MAC is unaltered, as it is unlikely that an attacker without the key could provide a valid MAC. Of course, this depends on Bob and Alice both keeping their shared secret key protected.
f)  This is a detective control. Use of a MAC does not prevent an attacker changing the message in transit, but it does let the recipient detect if the message has been changed. It is not corrective, so if an altered message is detected, Alice and Bob need to have a defined process to follow; for example, request retransmission. 

QUESTION 10
The Tapplock is a physical access device (padlock) that uses biometric data (user fingerprint) rather than a physical key to determine whether a user is authorized to unlock the padlock. The lock communicates with an app on the user's phone using Bluetooth. The phone app communicates with the Tapplock company's supporting database. The Tapplock literature advised that they used an encrypted fingerprint sensor, making use of AES-128 encryption.

Security researchers PenTest Partners investigated the security of the Tapplock product in 2018, and found some serious security vulnerabilities in the product, including in the way the encryption was used. Based on their investigation, they made an app that allowed them to unlock any Tapplock in less than two seconds. Read the Pen Test Partner's report on Tapplock (available at: https://www.pentestpartners.com/security-blog/totally-pwning-the-tapplock-smart-lock/ ) and answer the following questions:  
a) Which communication protocol does the app use for transmitting data, and why is this problematic? 
b) What sort of encryption do the Tapplock manufacturers use, and what is the key size?
c)   What did the researcher notice about the data sent to the lock when they looked at multiple attempts to connect?
d) Why is this observation considered to be a vulnerability - and how can this be exploited in an attack?
e) The Tapplock developers made a major error in deriving the serial number for the device and the encryption key to be used with AES. What was the error? 
f) What information did the researchers need to know to be able to unlock a Tapplock device? How would they be able to obtain this information?

a) Information communicated with the app is transmitted using http - this does not use encryption, so data sent can be observed by anyone monitoring communications.
b) The designers claim to use the AES block cipher, with a 128-bit key (AES-128).
c) The researcher noticed that the same 'random looking' data was sent from the app to the lock each time the researcher connected to it, and this information was necessary to get the lock to respond to commands (such as to unlock). 
d) The fact that the same information is sent to the lock each time is a vulnerability:
i. The information that is sent can be observed and captured and then (at a later time) it can be replayed to enable the padlock to be unlocked (if the vulnerability is exploited in this way, this is called a replay attack). 
ii. Even though the lock is designed to be used by multiple users (each registering their own fingerprint) the same authenticator was sent to the lock for different users - it was not individualized. If you know what it is, anyone can provide it. 
iii. Further, this information cannot be revoked or changed. So even if you cancel the permission for a user to authenticate to the lock, the mechanism has no way to prevent them doing so - they already have the required data.
e) The developers used AES encryption and derived the 128-bit encryption key to use with AES and the Serial number assigned to the Tapplock from the MD5 hash of the BLE MAC address (the Hash values output by MD5 are 128 bits long, so this probably seemed like a good idea). The major error they made here is that the BLE MAC address is public knowledge! This means that the key that is used with AES in the Tapplock is not actually a secret! The hash function being used (MD5) does not require a key, so anyone who knows the MAC address of a Tapplock can hash it to compute the key that will be used by that particular lock. No need to break AES if you know the key that is being used.
a. The article gives some details of this process - but don't worry if you can't follow all the detail. The main idea to understand is that the secret key was not actually secret (This is like leaving your house key under the front door mat). So although a strong encryption algorithm (AES-128) is being used, is not providing any real security because the secret key is not secret at all.
f) The information that the researchers needed to compute the AES key and open the Tapplock was just the Tapplock BLE MAC address. The Tapplock itself broadcasts this MAC address, so it is regarded as public knowledge. The researchers just needed a device that could detect Bluetooth communications - and mobile phones can do that (that's how the legitimate Tapplock app communicates with the Tapplock). They wrote an app that scans for Tapplocks, notes their MAC address, computes the key used for that particular app and then communicates to open the lock. If you have this app on your phone, you can use it to open a Tapplock in less than 2 seconds. The researchers did this to demonstrate the insecurity of the Tapplock design. If you have this app, you don't need to perform the replay attack discussed in part c - so no need to sniff network traffic and acquire details before opening a lock. The researchers made Tapplock aware of the vulnerabilities before they disclosed them to the public. That is part of responsible disclosure.
