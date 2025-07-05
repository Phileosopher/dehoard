
## Rare sats

Crudely speaking there are two sorts of crypto tokens. There are _fungible_ tokens, like Bitcoin and Ether and Tether and Solana, which have approximately cash-like properties: If a thing costs two Bitcoins, it doesn’t matter _which_ two Bitcoins you use to pay for it; any two Bitcoins are just as good as any other two Bitcoins. And there are _nonfungible_ tokens, NFTs, like Bored Ape Yacht Club, which have approximately art-object-like properties: Each Bored Ape is different, and some — based on their rarity or aesthetics or provenance — are worth much more than others.

Intuitively, fungible tokens are indistinguishable coins, while NFTs are unique images. But _really_ neither of those things is true. Really they are both entries in detailed permanent transaction ledgers. An NFT, for example, _isn’t_ the little drawing of the monkey; the NFT is simply a numbered entry in a ledger that [points to the drawing of the monkey](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly9tb3hpZS5vcmcvMjAyMi8wMS8wNy93ZWIzLWZpcnN0LWltcHJlc3Npb25zLmh0bWw/60e87ce39a995a4b1a2deb96Bcc92646f). I [once wrote](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly93d3cuYmxvb21iZXJnLmNvbS9mZWF0dXJlcy8yMDIyLXRoZS1jcnlwdG8tc3RvcnkvP2NtcGlkPUJCRDA1MTYyNF9NT05FWVNUVUZGJnV0bV9tZWRpdW09ZW1haWwmdXRtX3NvdXJjZT1uZXdzbGV0dGVyJnV0bV90ZXJtPTI0MDUxNiZ1dG1fY2FtcGFpZ249bW9uZXlzdHVmZg/60e87ce39a995a4b1a2deb96B61340118) that “an NFT consists of a series of numbered tokens, and the thing that makes it an NFT is that it has a different number in its tokenId field from the other tokens in its series.” 

Meanwhile a fungible token like Bitcoin is _not_ a _numbered_ entry in a ledger; there is [such a thing as](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly9vcGVuc2VhLmlvL2Fzc2V0cy9ldGhlcmV1bS8weGJjNGNhMGVkYTc2NDdhOGFiN2MyMDYxYzJlMTE4YTE4YTkzNmYxM2QvMw/60e87ce39a995a4b1a2deb96Bc622db60) “Bored Ape Number 3” but there is no such thing as “Bitcoin Number 3.” But there is a permanent immutable computer ledger containing every Bitcoin transaction, which means that you _could_, sort of, trace the ledger back to find what the third Bitcoin was and who holds it now. [[7]](imap://dave%40stucky%2Etech@mail.stucky.tech:993/fetch%3EUID%3E.INBOX%3E5707#footnote-7)

More generally, you could, if you wanted to, treat Bitcoins as completely nonfungible. You could trace back the history of any Bitcoin, or fraction of a Bitcoin. And then you could say things like:

- “I am willing to pay more for old Bitcoins, ones that were mined in like 2009, than I will for new Bitcoins, ones that were only mined in 2024.”
- “I am willing to pay more for Bitcoins with cool provenance, like ones that were once [owned by Satoshi Nakamoto](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly93d3cuYmxvY2tjaGFpbi5jb20vZXhwbG9yZXIvYmxvY2tzL2J0Yy8wMDAwMDAwMDAwMTlkNjY4OWMwODVhZTE2NTgzMWU5MzRmZjc2M2FlNDZhMmE2YzE3MmIzZjFiNjBhOGNlMjZm/60e87ce39a995a4b1a2deb96B86599764) or used to pay for the [2010 Bitcoin Pizza](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly93d3cuY29pbmRlc2suY29tL2NvbnNlbnN1cy1tYWdhemluZS8yMDIzLzA1LzIyL2NlbGVicmF0aW5nLWJpdGNvaW4tcGl6emEtZGF5LXRoZS10aW1lLWEtYml0Y29pbi11c2VyLWJvdWdodC0yLXBpenphcy1mb3ItMTAwMDAtYnRjLw/60e87ce39a995a4b1a2deb96Ba3f3d853), than I will for regular old Bitcoins with no fun history.” 
- “I am willing to pay _less_ for Bitcoins with a troubled regulatory history, like the ones that were [stolen in the Bitfinex hack](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly93d3cuYmxvb21iZXJnLmNvbS9vcGluaW9uL2FydGljbGVzLzIwMjItMDItMDkvYnVzaW5lc3MtcmFwcGVyLXdhcy1iYWQtYXQtYml0Y29pbi1sYXVuZGVyaW5nP2NtcGlkPUJCRDA1MTYyNF9NT05FWVNUVUZGJnV0bV9tZWRpdW09ZW1haWwmdXRtX3NvdXJjZT1uZXdzbGV0dGVyJnV0bV90ZXJtPTI0MDUxNiZ1dG1fY2FtcGFpZ249bW9uZXlzdHVmZg/60e87ce39a995a4b1a2deb96B48ddeb97), than I will for Bitcoins with a clean regulatory history.”

Bitcoins are fungible simply because it is standard convention among Bitcoin users to _treat_ them as fungible, but they _are_ distinguishable from one another, and if you wanted to discriminate among Bitcoins you _could_. People mostly don’t, but the last thing on that list — “try not to accept Bitcoins that have been stolen or are [otherwise of interest](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly93d3cudHJtbGFicy5jb20vcG9zdC91cy10cmVhc3VyeXMtb2ZhYy1zYW5jdGlvbmVkLXJ1c3NpYS1iYXNlZC1jcnlwdG8tZXhjaGFuZ2VzLWFuZC1maW50ZWNocy1mb3ItZmFjaWxpdGF0aW5nLXNhbmN0aW9ucy1ldmFzaW9u/60e87ce39a995a4b1a2deb96Ba1ca7d56) to US law enforcement” — _does_ have some traction. Some Bitcoins really _are_ less valuable than others.

And some are more. Here is [a delightful story from Joel Khalili at Wired](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly9hcnN0ZWNobmljYS5jb20vaW5mb3JtYXRpb24tdGVjaG5vbG9neS8yMDI0LzA1L3RoZS1odW50LWZvci1yYXJlLWJpdGNvaW4taXMtbmVhcmluZy1hbi1lbmQv/60e87ce39a995a4b1a2deb96Bed00c94f):

> In the same way a dollar is made up of 100 cents, one bitcoin is composed of 100 million satoshis—or sats, for short. But not all sats are made equal. Those produced in the year bitcoin was created are considered vintage, like a fine wine. Other coveted sats were part of transactions made by bitcoin’s inventor. Some correspond with a particular transaction milestone. These and various other properties make some sats more scarce than others—and therefore more valuable. The very rarest can sell for tens of millions of times their face value; in April, a single sat, normally worth $0.0006, sold for $2.1 million.

There are two interesting points here. One is simply the existence of “rare sats”: To at least some … Bitcoin collectors? … some satoshis are worth more than others, due to their history or provenance. 

The other is that, while some Bitcoin enthusiasts value rare sats highly and will pay a lot for them, others just cheerily assume that Bitcoin is a fungible currency. And so there is a trade:

> [Bill] Restey is part of a small, tight-knit band of hunters trying to root out these rare sats, which are scattered across the bitcoin network. They do this by depositing batches of bitcoin with a crypto exchange, then withdrawing the same amount—a little like depositing cash with a bank teller and immediately taking it out again from the ATM outside. The coins they receive in return are not the same they deposited, giving them a fresh stash through which to sift. They rinse and repeat.

If you deposit one Bitcoin on a crypto exchange and then withdraw it, you will get one Bitcoin. But you will not get the same Bitcoin you put in. The exchange will say “ehh Bitcoins are Bitcoins, it doesn’t matter.” But you might disagree.

[7] In actual fact the first 50 Bitcoins were minted all at once, and that set of Bitcoins, [according to Blockchain.com](https://link.mail.bloombergbusiness.com/click/35403556.275801/aHR0cHM6Ly93d3cuYmxvY2tjaGFpbi5jb20vZXhwbG9yZXIvYmxvY2tzL2J0Yy8wMDAwMDAwMDAwMTlkNjY4OWMwODVhZTE2NTgzMWU5MzRmZjc2M2FlNDZhMmE2YzE3MmIzZjFiNjBhOGNlMjZm/60e87ce39a995a4b1a2deb96C86599764), “is unredeemable, as it was omitted from the transaction database. This means any attempt to spend it would be rejected by the network. Whether this was intentional or not still remains unknown.” Also I am being a little loose with terminology here; there is not such a thing as “a Bitcoin,” but rather any amount of Bitcoin that you get is the residue of various prior transactions that can be traced back in time to when batches of Bitcoin were mined. It’s not like individual coins have passed from hand to hand, but the Bitcoins in your account reflect the history of the transactions that brought them there.

## NFT backdating

In 2021, Damien Hirst offered art collectors a proposition that was very 2021 and very Damien Hirst:

1. Hirst had made 10,000 paintings of “colourful hand-painted dots on A4 paper,” as [today’s story in the Guardian](https://link.mail.bloombergbusiness.com/click/35465286.278788/aHR0cHM6Ly93d3cudGhlZ3VhcmRpYW4uY29tL2FydGFuZGRlc2lnbi9hcnRpY2xlLzIwMjQvbWF5LzIyL2RhbWllbi1oaXJzdC1hcnR3b3Jrcy1wYWludGVkLXllYXJzLWxhdGVyLWN1cnJlbmN5LWFydGlzdA/60e87ce39a995a4b1a2deb96Bf2cabe34) puts it, and he was offering them for sale, but with a twist.
2. The twist was that you could buy a nonfungible token (NFT), on the blockchain, corresponding to one of those dot paintings.
3. Then Hirst would light your painting on fire, and you’d get to keep the NFT.
4. _Or_, or, or, you could keep the painting, but then you would lose the NFT.

“In total, buyers chose to retain the physical versions of 5,149 paintings”; almost 4,000 buyers chose the fire and the NFT. (“Hirst kept 1,000 of the works, although he opted to hold them as the NFT versions,” says the Guardian.) 

Anyway Hirst obviously did not bother putting all the dots on all 10,000 papers; there was a factory:

> According to sources familiar with the production of The Currency series, dozens of artists were hired to assist with the factory-style production of the paintings in 2018 and 2019. Some worked eight-hour days for several months, wearing cumbersome masks to protect from the paint fumes. ...
> 
> Lawyers for Hirst and Science said they always adhered to relevant health and safety rules and practices.

Sure. But the news today is:

> The initial sale brought in about $18m. At the time, Hirst said of the project: “It comprises of 10,000 NFTs, each corresponding to a unique physical artwork made in 2016.”
> 
> The paintings were sold via a single authorised seller, Heni, run by Hirst’s business manager. It said at the time that the works were “created by hand in 2016”. 
> 
> However, five sources familiar with the creation of the works, including some of the painters who put the dots to paper, told the Guardian many of them were mass-produced in 2018 and 2019.

I gather that early-career Damien Hirst works are worth more than later-career Damien Hirst factory products, though I am not sure why the difference between 2016 and 2019 would matter all that much. Surely no one was expecting that Hirst himself put all the dots on all the papers; surely, when you pay for a Damien Hirst painting, part of what you are paying for is, like, the joke that Hirst is making about the mass production and commercialization of art. 

But here specifically you were paying for the joke he was making about the blockchain! He was gonna burn the paintings! Imagine being angry that you paid Damien Hirst to burn a painting that his factory made in 2016, but then you found out that he actually burned a painting that his factory made in 2019.

Honestly this makes me like Hirst more. I think this is the first good joke that I’ve ever seen in the [“object-fire-token-money” NFT genre](https://link.mail.bloombergbusiness.com/click/35465286.278788/aHR0cHM6Ly93d3cuYmxvb21iZXJnLmNvbS9uZXdzL25ld3NsZXR0ZXJzLzIwMjEtMDktMTAvbW9uZXktc3R1ZmYtZnVuZ2libGUtc2xpY2VzLW9mLW5vbi1mdW5naWJsZS10b2tlbnM_Y21waWQ9QkJEMDUyMjI0X01PTkVZU1RVRkYmdXRtX21lZGl1bT1lbWFpbCZ1dG1fc291cmNlPW5ld3NsZXR0ZXImdXRtX3Rlcm09MjQwNTIyJnV0bV9jYW1wYWlnbj1tb25leXN0dWZm/60e87ce39a995a4b1a2deb96B53b400b9)? In particular, it is a sophisticated _blockchain_ joke. The blockchain, of course, is a tamper-proof record of provenance. Whatever bad things you can say about NFTs, one thing that is surely true of an NFT is that you can tell when it was created. The creation date of these NFTs — 2021, of course! — is permanently and immutably inscribed in the blockchain. The paintings’ creation date, man, who knows; he burned those. You _can’t_ backdate the creation of a crypto artwork; immutable provable time sequencing is in some deep sense the _point_ of crypto. But Hirst found a way to do it.
