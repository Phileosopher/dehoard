
NOTE: THIS IS TL;DR CYBERSECURITY
- the Security page will be more complete
- focus on basic aspects of what non-tech people want to know

PRINCIPLE THAT MAY GO TO SECURITY OR CYSEC, MAYBE GIS
- One way to protect against invasion is to have multiple barriers, with degrees of safety for each
- e.g., subsidiary corporations that can get sued without the parent company being affected
- e.g., city walls in layers toward the government center
- e.g., multiple firewalls with different encryptions each layer

if you're particularly paranoid, make sure to change your devices' MAC address, since that MAC has the origination and likely information about the firmware on it

Have a burner browser
- Even if you use privacy-minded things in a browser (e.g. private windows, no cookies), some services detect this.
- For this reason, have a "burner" browser that has absolutely nothing in it
- Preferably, it should use a different framework (e.g., Firefox uses Gecko, so use Chromium w/ Brave)

Identity theft protection
- On average, it takes 800 hours to resolve identity fraud.
    - Good protection services will assign a counselor to clean up the mess.
- Don't get ID theft protection that only monitors credit reports.
    - Several popular services like [Credit Karma](https://www.creditkarma.com/) will monitor credit for free.
- identity theft insurance can often be part of the ID theft protection package - https://www.cnbc.com/select/id-theft-insurance/

With peer-to-peer payments (P2P), you can transfer money to someone from your bank account, debit card, or credit card using a website or mobile app such as Zelle, Cash App, PayPal, or Venmo. P2P payments can also include your financial institution's apps, such as Schwab Mobile. While P2P payments are popular and convenient, understanding the risks can help you avoid becoming a victim of scams and fraud.

How do scams and fraud differ?
Fraud involves someone accessing your account without your permission and completing unauthorized transactions. A scam involves being tricked into authorizing a transaction or sending a payment. It's important to remember the difference, as the same protections do not always apply to both.

In general, be VERY vigilant about the information you enter, and consider how it makes any sense to get used
Do NOT enter your credit card info into something just because they need to "verify your age"
You don't need to "make a login" for a public site like wikipedia
those logins will often ask for extra information, much of which you shouldn't give away freely

The reason this is a big issue, EVEN IF THE COMPANY IS LEGITIMATE, is because your personal information is as safe as that company's server is safe from getting hacked
i.e., it can happen to anyone who wasn't paying attention to 1 setting in a computer somewhere and 1 teenage/incel found it

NOTE: when making any purchase online, MAKE ABSOLUTELY SURE that you're seeing the "lock" symbol in the top left
(must research what that actually means, I'm presuming a certified certificate)

FROM NORDVPN TEST
- Wifi:
    - secure password
    - disable SSID on router
    - WPA2/WPA3 encryption
    - enable MAC address filtering on router
- Password security???
- Malware causes:
    - opening random downloaded files
    - clicking on unknown links
    - visiting suspicious sites
    - opening emails from unknown sources
- IoT problems
    - no encryption
    - no-password access
    - no standards/regulation on many things
    - discreet audio/video recording

What information could do
- With your passport number, someone could:
    - Book an international flight as you
    - Apply for anything that requires proof of identity documentation with the government, e.g. Working with children check
    - Activate a SIM card (and so get an internet connection that's traceable to you, not them, hiding them from the government)
    - Create a fake physical passport from a template, with the correct passport number (which they then use to cross a border, open a bank account, or anything)
- with a password, soemoene could
- login to that particular computer (if 2FA wasn't enabled
- login to ANY other site that had the same password/email combo

CySec hardening concepts
- Disable/remove Native VLAN
- Check for redirects and diversions
    - #62* redirect
    - _#21# diversions_
    - _##002# remove redirections_
- _Packet analyzer for phones_
    - _##197328640#_#
    - UMTS RR Information (cell ID#)
    - MM Info > Serving PLMN (area code)
    - Netmonitor website (OpenCellID, e.g.)
- Record all relevant information
    - IMEIs of all devices #06#

Dial *67 in North America to make calls labeled as anonymous

We can apply obfuscation in our own lives by using practices and technologies that make use of it, including:
- The secure browser Tor, which (among other anti-surveillance technologies) muddles our Internet activity with that of other Tor users, concealing our trail in that of many others.
- The browser plugins TrackMeNot and AdNauseam, which explore obfuscation techniques by issuing many fake search requests and loading and clicking every ad, respectively.
- The browser extension Go Rando, which randomly chooses your emotional "reactions" on Facebook, interfering with their emotional profiling and analysis.
- Playful experiments like Adam Harvey's "HyperFace" project, finding patterns on textiles that fool facial recognition systems - not by hiding your face, but by creating the illusion of many faces.

Web content is frequently insecure because it's often a hybrid of secure AND insecure elements
- this is especially egregious with web forms, which can send insecure content EVEN WHEN IT'S A HTTPS SITE!

Plan for a catastrophic laptop crash, with either a USB drive or a recovery partition.

[Gen Z falls for online scams more than their boomer grandparents do : technology](https://old.reddit.com/r/technology/comments/16rdi9s/gen_z_falls_for_online_scams_more_than_their/)
- the best cure for tech safety is experience

CYSEC TIP:
Post-it note/sticker over built-in camera

## privacy

NOTE: will connect to other non-TS page?

Privacy and complete freedom are inversely connected
- if everyone has privacy, there's the opportunity for injustice
- if everyone has freedom, there's technically no privacy
 
article on how there needs to be a tech version of attorney/client, doctor/patient privilege
- basically, there's too much [power] in the hands of these geeks that there must be a legally bound implicit standardized agreement
- without this, any random person can steal any information they want because copying computer information is EASIER than moving it

[Privacy is the most important concept of our time | Hacker News](https://news.ycombinator.com/item?id=24661271)
[Why Privacy Is the Most Important Concept of Our Time - In Re](https://inre.me/why-privacy-is-the-most-important-concept-of-our-time/)

[Cover Your Tracks | Hacker News](https://news.ycombinator.com/item?id=25166703)
good dialogue on uniqueness
[Introducing Cover Your Tracks! | Electronic Frontier Foundation](https://www.eff.org/deeplinks/2020/11/introducing-cover-your-tracks)

[Privacy Is a Human Right | Hacker News](https://news.ycombinator.com/item?id=28997501)
[Privacy is a Human Right | The Tor Project](https://blog.torproject.org/privacy-is-a-human-right/)

[Cops Are Suing a Teen for Invasion of Privacy After False Arrest Vid Goes Viral | Hacker News](https://news.ycombinator.com/item?id=37956714)

[Internet Health](https://foundation.mozilla.org/en/internet-health/)

[Block YouTube ads on AppleTV by decrypting and stripping ads from Profobuf | Hacker News](https://news.ycombinator.com/item?id=37279109)
[Block YouTube Ads on AppleTV by Decrypting and Stripping Ads from Profobuf](https://ericdraken.com/pfsense-decrypt-ad-traffic/)

[When an app asks for permissions, it should have a "feed fake data" option | Hacker News](https://news.ycombinator.com/item?id=36644895)
[Nifflas: "When an app asks for permissio…" - Gamedev Mastodon](https://mastodon.gamedev.place/@Nifflas/110668040598715116)

[Privacy vs. "I have nothing to hide" (2019) | Hacker News](https://news.ycombinator.com/item?id=32835966)
[Privacy vs "I have nothing to hide" | Kev Quirk](https://kevquirk.com/privacy-vs-i-have-nothing-to-hide/)

[No user accounts, by design | Hacker News](https://news.ycombinator.com/item?id=30503482)
[No user accounts, by design | F-Droid - Free and Open Source Android App Repository](https://f-droid.org/en/2022/02/28/no-user-accounts-by-design.html)

[The case for banning children from social media | Hacker News](https://news.ycombinator.com/item?id=35447588)
[The Case for Banning Children from Social Media | The New Yorker](https://www.newyorker.com/news/our-columnists/the-case-for-banning-children-from-social-media)

[What is AT&T doing at 1111340002? | Hacker News](https://news.ycombinator.com/item?id=29135559)
[What is AT&T doing at 1111340002?](https://scribe.rip/telecom-expert/what-is-at-t-doing-at-1111340002-c418876c212c)

[Wearable Microphone Jamming | Hacker News](https://news.ycombinator.com/item?id=28885739)
[Wearable Microphone Jamming](https://sandlab.cs.uchicago.edu/jammer/)

[A single laser fired through a keyhole can expose everything inside a room | Hacker News](https://news.ycombinator.com/item?id=28466737)
[NLOS Keyhole Imaging Can See Inside a Closed Room](https://gizmodo.com/a-single-laser-fired-through-a-keyhole-can-expose-every-1847638281)

[Who Owns My Name? | Hacker News](https://news.ycombinator.com/item?id=28007547)
[Who Owns My Name?. Does my name belong to me? Does my… | by Amanda Knox | Medium](https://amandamarieknox.medium.com/who-owns-my-name-93561f83e502)

[Website Fingerprinting on Early QUIC Traffic | Hacker News](https://news.ycombinator.com/item?id=25969886)
[[2101.11871] Website fingerprinting on early QUIC traffic](https://arxiv.org/abs/2101.11871)

[Your computer should say what you tell it to say | Hacker News](https://news.ycombinator.com/item?id=37050035)
[Your Computer Should Say What You Tell It To Say | Electronic Frontier Foundation](https://www.eff.org/deeplinks/2023/08/your-computer-should-say-what-you-tell-it-say-1)

[Is Internet Privacy a Myth? - codepaste](https://codepaste.net/static-topic-4/)

[Ask HN: How do you trust that your personal machine is not compromised? | Hacker News](https://news.ycombinator.com/item?id=34388866)

### digital sovereignty

[5G: The outsourced elephant in the room | Hacker News](https://news.ycombinator.com/item?id=26843068)
[5G: The outsourced elephant in the room - Bert Hubert's writings](https://berthub.eu/articles/posts/5g-elephant-in-the-room/)

[Sov's Compendium](https://sovs.notion.site/Sov-s-Compendium-41f097d28dae4d09801f10cde1b2d03b)

[Your online identity is owned by your email provider (2019) | Hacker News](https://news.ycombinator.com/item?id=32563735)
[Your online identity is owned by your email provider | Ctrl blog](https://www.ctrl.blog/entry/email-identity-provider.html)

### privacy community

[Toolkits - Transparency.org](https://www.transparency.org/en/toolkits)
[Home - Transparency.org](https://www.transparency.org/en/)

[dig deeper](https://digdeeper.neocities.org/)
[dig deeper](https://web.archive.org/web/20210102182957/https://digdeeper.neocities.org/)
articles on privacy on/and the internet
[Dig Deeper](https://digdeeper.club/)

[Teaching Privacy |](https://teachingprivacy.org/)

### privacy news

[Latest Privacy](https://latestprivacy.org/)
[RestorePrivacy](https://restoreprivacy.com/category/news-reports/)
Privacy News

[/r/privacy](https://www.reddit.com/r/privacy/)
everything about privacy on reddit

[10 Best Antivirus Software in 2024: Windows, Android, iOS, Mac](https://www.safetydetectives.com/)

### privacy is important

[Mo Bitar](https://dev.to/bitario/privacy-is-power)
Privacy is Power

[You can opt out of airport face scans | Hacker News](https://news.ycombinator.com/item?id=41051327)
[Can you opt out of airport face scans? Yes! Here’s how. - Vox](https://www.vox.com/future-perfect/360952/summer-travel-airport-facial-recognition-scan)

[People Still Aren't Patched or Protected : cybersecurity](https://old.reddit.com/r/cybersecurity/comments/tz8q44/people_still_arent_patched_or_protected)
