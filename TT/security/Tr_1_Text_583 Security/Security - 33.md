
There is a such thing as TOO secure:

- the ouroboros snake strikes when the authentication is BEHIND the authentication wall (e.g., email authentication sent to an email on the same server)

3-2-1 rule:
- 3 copies of your data on 2 different forms of media, 1 which is stored off site

NOTE: CLARIFY "PERMISSIONS" ON THE TS SECURITY PAGE

[Should all locks have keys? Phones, Castles, Encryption, and You. - YouTube](https://www.youtube.com/watch?v=VPBH1eW28mo)
- people who crack digital locks have no sense of distance and simply run lots of numbers
- locks CAN be made unbreakable with lots of math, but not entirely
- governments REALLY want to have back-doors for encryption, though many geeky privacy advocates don't want that to happen, and those governments can't be trusted to always be good
- SIDENOTE: encrypted files are essentially in scrambled gibberish in their resting state, then temporarily become usable when that authentication passes through

Be a pro. Back up your back up. Have at least one physical backup and one backup in the cloud. Have more than one of each. How much would you pay to retrieve all your data, photos, notes, if you lost them? Backups are cheap compared to regrets.

Assume anyone asking for your account information for any reason is guilty of scamming you, unless proven innocent. The way to prove innocence is to call them back, or login to your account using numbers or a website that you provide, not them. Don't release any identifying information while they are contacting you via phone, message or email. You must control the channel.

Follow best practices
- ASafaaWeb security analyzer
- Observatory by Mozilla

Cross-site scripting
- XSS cheat sheet
- DOM based XSS cheat sheet
- Free XSS scanner

Cross-site request forgery
- Explanation and walkthrough
- CSRF cheat sheet

Secure connection (SSL) (OPTIONAL)
- Setup SSL on IIS 7
- Setup SSL on Apache
- SSL Server Test

HTTP Strict Transport Security (OPTIONAL)
- MDN Overview
- OWASP Overview

Enable Content Security Policy (OPTIONAL)
- Content Security Policy
- MDN Guide
- OWASP Overview
    - CSP Tester

Data integrity takes several forms and can be divided into four categories:
1. Entity Integrity: No duplicate rows exist in a table. For example, we can't insert Ron Weasley twice in the database.
2. Domain Integrity: Restricting the type of values that one can insert in order to enforce correct values. For example, a House can only be Gryffindor, Ravenclaw, Slytherin, or Hufflepuff.
3. Referential Integrity: Records that are used by other records cannot be deleted. A teacher cannot be deleted if they are currently teaching a course.
4. User-Defined Integrity: An "other" category that consists of business-related logic and rules to the database.

Make sure to
- Add/change wireless passwords and any router passwords, ESPECIALLY admin ones
- When formatting, clear the MBR (often with fdisk /MBR)
- Zero out all data by clearing with multiple passes (to avoid data theft afterward) - 7 passes?

there has been a large push over the last 5 or so years to move to
zero-trust networks as opposed to relying on perimeter security.
Perimeter security is only as strong as the weakest node on your
network. You should _assume_
that
someone will be able to compromise a node on your internal network, and
thus you must never trust a client simply because it has access to your
network.

See e.g. this White House memo from a couple weeks back
[Office of Management and Budget Releases Federal Strategy to Move the U.S. Government Towards a Zero Trust Architecture | OMB | The White House](https://www.whitehouse.gov/omb/briefing-room/2022/01/26/office-of-management-and-budget-releases-federal-strategy-to-move-the-u-s-government-towards-a-zero-trust-architecture/)

FUD - Fear, Uncertainty and Disinformation
PII - personally identifiable information

Note: I can make a threat model that also ASSUMES getting hacked
- It can, for example, lead to specific info that's useless, or have a full-on cap on data requests (e.g. only get 1,000 emails on ANY request)

## History of the internet

- Confidentiality - prevent unauthorized viewing of information
- Integrity - it's from who you think it is and hasn't been modified since it was sent SHA-1 is decent, but not necessarily great
    - It's useful for non-critical situations
    - The public key can make a digest, but can't decrypt
    - Receiving a signed message
    - Receive message and digest from insecure transport
    - Remove digest and add secret
    - Compute SHA digest for message and secret
    - Compare the computed digest to the received digest
MD5 hash calculator
Base64 encoder and decoder
- To successfully manage cybersecurity, you have to understand the mind of a hacker
    - That doesn't mean you need to hack, but you DO need to understand the criminal mentality that drives a hacker, and how they tend to think.
- It uses the "secure socket layer" (SSL) to send the cryptographic data
    - The private key is the only one that decrypts, while the public key always encrypts
    - There are 2 kinds of public keys:
        1. Made-up general public keys
        2. 3rd-party authorized public keys (e.g., GoDaddy, Comodo, Verisign, etc.)
            - These second public keys are "digital certificates", or "signed private keys"
            - It can be $100-200 or $1000-2000 to get your certificate formally signed.
- Cryptography makes it relatively more work to hack anyone
    - Without cryptography, anyone can go after anyone
        - Governments can surveil and attack anyone at will
        - Criminals can hack anyone at will
    - With cryptography, while anyone CAN get hacked, the governments/hackers will only attack based on a priorities list, which will protect the majority of everyone else.
    - We can't really "trust" the cryptography, because it's simply math.
        - For it to actually matter, someone has to use code WITH that math.
        - Thus, we only really trust the people who make the systems.
        - Often, the math is never broken, but the stuff AROUND it is vulnerable (software, hardware, code, etc.)
    - The more complexity in the system, the more risks inherent to the system!
        - Keeping it simple keeps it safer.

ON CLASSIFIED DOCUMENTS:

SCIF: Sensitive Compartmentalized Information Facility. 

- Typically this is a physical location (room, building, etc) with specific physical security measures to keep classified information safe. Those with access can view, store, print, or otherwise access the products. The Congressional SCIF (I presume) is just for viewing…Not sure where the committees that have access actually do their work, which would probably create classified documents. 
- SCIFs are rated for the classification level of information they contain.  All of these locations have strict access requirements including the appropriate clearance, access lists and badges, no mobile devices, earbuds, smart watches, etc.   
- TS - Top Secret (exceptionally grave damage to National Security)
- S - Secret (grave damage to National Security)
- CUI - Controlled Unclassified Information (replaced For Official Use Only - FOUO) and includes things like personally identifiable info, or other things that we generally want to keep private, but aren't strictly classified. 
- Another way to accidentally attain a higher classification is by adding multiple pieces of unclassified information together. This is one of the things we have to be careful of, because if you're not careful, the final document might be a higher classification **because** of the sum of its parts.
- Classification markings are not only on the cover sheet, but also throughout the document itself, including pages and individual paragraphs. 
- Classified documents generally have to stay inside SCIFs. Documents can **only** come out if properly packaged to protect the information and then are carried by official couriers with special training, clearances, and lockable courier cases. Not quite a briefcase with handcuffs, but close. 

Computer Systems: 

- There are classified computer networks which have no connection (air gaps) to the regular internet or outside world. These are essentially completely securely self-contained and handle information up to a particular classification level; so, there are secret systems as well as top secret systems. TS can handle any level up to TS (including secret).  Secret can only handle up to secret info. These systems include email clients so you can send documents to other users with access and need to know. 
- There are also unclassified computer systems for daily work that have internet connectivity, but are regulated by IT policies and systems that filter what you can get to. E.g., for the longest time, Al Jazeera News wasn't accessible on the unclassified network. 
- Also, all users sign acceptable use policies as a prereq to getting network access, and sites that are forbidden in the AUP are routinely blocked; so if there's a bad link on the page (site, video, etc.), you'll often get an intimidatingly official looking "ACCESS TO THIS SITE IS FORBIDDEN" in that space.  Sometimes it's the whole page. 

Getting a Clearance.

- How one **gets** a security clearance is another saga that includes a veritable colonoscopy of background checks going over years of your past, personal connections, rap sheets, foreign travel, credit score and finances, past addresses, scrutiny of your family and much more including an in person interview, and if required, possibly a polygraph. Good times.
- Clearances are also re-vetted periodically to make sure the person is still considered safe to have a clearance. It used to be that clearance reviews only happened every 5 or 10 years (depending on the clearance level), but they're changing that to "continuous vetting" now where the security apparatus overseeing this will be alerted to things like criminal offenses, bankruptcies, other "derog" (derogatory) information; one can presume that they're closely looking at social media and such as well.

All of this to say that classified information **should** be taken seriously and there are myriad policies, and procedures deliberately put in place to ensure that it is cared for properly. Even though he may have declassified it, Trump probably shouldn't have had that stuff at Mar a Lago (declassified or not, that doesn't mean that it lost any of its importance or potential to cause harm to the country). Nor should the former VP Biden have had classified dox hanging out in file boxes in his (locked) garage. There may be legitimate reasons for former presidents to have that type of stuff, but it never negates the handling requirements.

## Windows 11 Privacy Apps

Tiny11Builder
Simplewall
ShutUp10++
Bulk Crap Uninstaller
BleachBit
Mullvad VPN
Firefox - in strict mode
uBlock Origin
Decentraleyes
Privacy Badger

## How To Be Safe

1) Atestation - periodic check of every account,
2) Rotate every key, every password.
3) Verify every open port as needed
4) verify the jobs for data transferrals
5) verify every vpn
6) verify every computer/ network device
7) trust nothing
8) assuming your already compromised don't bother with a baseline your already owned start the clean up.
9) employ red team attacks
10) patch
11) correlation optics
12) externalise the siem
13) add honey pots
14) test your DR from cold offline restore
15) do background checks on your admin staff
16) add nano segmentation
