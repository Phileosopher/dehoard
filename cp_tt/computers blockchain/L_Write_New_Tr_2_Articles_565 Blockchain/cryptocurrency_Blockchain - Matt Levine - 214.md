
[When Is a Token Not a Security? - Bloomberg](https://www.bloomberg.com/opinion/articles/2023-06-07/when-is-a-token-not-a-security)

At a high level, the blockchain solution is to confirm transactions by letting everyone keep a copy of the transaction ledger. And then the official ledger is based on consensus among people who have some demonstrated stake in the system. What that has often meant in practice - [what it means in Bitcoin](https://bitcoin.org/bitcoin.pdf) and what it [originally meant in Ethereum](https://ethereum.org/en/whitepaper/) - is "proof of work." What you do is, you buy a bunch of computers, and you set them to work solving meaningless math problems, and whoever solves the most math problems the fastest gets to confirm a block of Bitcoin transactions, and they are rewarded with some newly minted Bitcoins and then everyone starts over solving more math problems to confirm more transactions. Buying the computers, and paying for the electricity to run them to solve the math problems, demonstrates your commitment to Bitcoin: It would be crazy to spend all that money on computers and electricity to confirm _fake_ transactions, which would undermine the value of Bitcoin and thus of your investment.

This is called "mining": You spend money on computers and electricity, and then you are rewarded with newly created Bitcoins. And there are people, and publicly traded companies, who are in the business of Bitcoin mining and thus of maintaining the Bitcoin network. The inputs are electricity and the outputs are Bitcoin.

This was a clever innovation and has some important benefits. It lets you have a ledger that is maintained by people with incentives to do the right thing - people you can trust - without knowing who they are. There is no pre-approved list of people who are allowed to maintain the Bitcoin ledger; anyone who buys enough computers and electricity can participate. It is [permissionless](https://www.bloomberg.com/opinion/articles/2022-09-13/crypto-wants-some-sec-rules). But because they have to buy all those computers and electricity, they have good incentives to maintain the ledger in a good way.

But there are some problems. The biggest is that it uses a ton of electricity solving pointless math problems, which seems wasteful both in environmental terms (you're emitting a lot of carbon to generate all that electricity) and [also in economic terms](https://vitalik.ca/general/2020/11/06/pos2020.html) (the Bitcoin system is effectively paying utility companies a lot of money to maintain its ledger). Developers of later blockchains realized that, if the point here is to have transactions confirmed by people with a demonstrated stake in the system, there are easier ways to demonstrate a stake in the system. (https://www.bloomberg.com/opinion/articles/2022-09-14/ethereum-is-merging#footnote-2) Most simply: If you have a lot of Bitcoins, you will want Bitcoin to be valuable, and so you will want to confirm transactions honestly in order to keep Bitcoin valuable. Instead of proving that you have an economic stake in the system by spending a lot of money on computers and electricity, you could prove that you have an economic stake in the system by spending a lot of money _on Bitcoin_. If you have a lot of Bitcoin, that proves that you care about Bitcoin, so you get to participate in confirming transactions.

Ethereum's new process, instead of Bitcoin, will rely instead on what's called proof of stake. It consumes very little power, because it doesn't depend on miners. It does require entities called validators to put some skin in the game in the form of Ether coins. Staking, or putting coins in the pot, gives large Ether owners the right to add a block of transactions to the ledger; they're rewarded with new Ether when they do so. All Ether tokens will now pay interest when placed into staking wallets. The software upgrade is called the Merge because the existing Ethereum blockchain will combine with a parallel network that's been running for almost two years to test the proof-of-stake concept.

## Do Kwon: not atoning

Do Kwon, the founder of the Terra blockchain, which vaporized tens of billions of dollars of investor money when its TerraUSD algorithmic stablecoin death-spiraled, remains "[obviously on the run](https://www.bloomberg.com/news/articles/2022-09-17/luna-and-terra-s-do-kwon-not-in-singapore-local-police-say)" (in the words of South Korean authorities) or "not on the run" (in his words), but he is committed to tweeting through it. Yesterday he [tweeted](https://twitter.com/stablekwon/status/1577639160692854784) some [mean things](https://twitter.com/stablekwon/status/1577644770859491328) about the South Korean government, [including](https://twitter.com/stablekwon/status/1577645322662076417):

> It's no surprise that crypto is most popular in countries that weaponize state institutions against their own people for political gain.
>
> Reap what you sow - revolutions start from within.

There was a time when this sort of rhetoric - about how crypto was a revolution, about how states and laws were obsolete, about how crypto was a force for freedom against the oppression of the state, about how crypto moguls like Kwon are the future and politicians are the past - was pretty common and triumphalist. And then Terra incinerated tens of billions of dollars that ordinary people entrusted to it! Come on! If you lost all your money on Terra and are nonetheless planning to take up arms in Do Kwon's revolution, I would love to know why.

## Crypto custody

I [used](https://www.bloomberg.com/opinion/articles/2019-05-08/uber-is-already-a-little-public) to [say](https://www.bloomberg.com/opinion/articles/2021-02-25/gamestop-is-happening-again) that the fate of all crypto exchanges was to be hacked, but in fairness that has stopped being true. Big modern crypto exchanges tend to be serious professional companies that care a lot about information security, and when one is hacked and [loses $570 million of crypto](https://www.cnbc.com/2022/10/07/more-than-100-million-worth-of-binances-bnb-token-stolen-in-another-major-crypto-hack.html), that is _news_, as opposed to just, you know, Thursday. It still happens though. There is some combination of factors that makes exchanges' pots of customer crypto just irresistible to hackers, something like:

- Cryptocurrencies are more or less bearer instruments, so if you steal a bunch of Bitcoin you can use them more easily than if you steal a bunch of Treasury bonds or whatever.
- Computer hackers tend to be intellectually and aesthetically interested in crypto, so they focus their hacking energies on crypto exchanges rather than banks.
- Crypto is pretty thinly regulated, so you are somewhat less likely to attract law-enforcement attention for hacking a crypto exchange than for hacking a bank.
- Crypto is all pretty new, so there is less in the way of best practices around information security.
- Crypto exchanges mostly aren't just one guy with a laptop anymore, but they are still _more_ likely to be _closer_ to "one guy with a laptop" than the average bankis.

I say "crypto exchanges" because, historically, crypto exchanges have been leaders in the business of keeping custody of crypto assets. But now crypto custody is increasingly the business of traditional financial institutions. And I guess the question is: Wouldn't it be very, very funny if Bank of New York Mellon Corp. gets hacked and loses [its customers' Bitcoin](https://www.wsj.com/articles/americas-oldest-bank-bny-mellon-will-hold-that-crypto-now-11665460354)?

> The nation's oldest bank said it would begin receiving clients' cryptocurrencies on Tuesday, becoming the first large U.S. bank to safeguard digital assets alongside traditional investments on the same platform.  
>
> BNY Mellon won the approval of New York's financial regulator earlier this fall to begin receiving select customers' bitcoin and ether starting this week. The bank will store the keys required to access and transfer those assets, and provide the same bookkeeping services on those digital currencies that it offers to fund managers for their portfolios of stocks, bonds, commodities and other assets. …
>
> Money managers have long relied on BNY Mellon and other custody banks for an array of vital, if humdrum, back-office functions such as tracking changes to the value of their assets. Founded by Alexander Hamilton more than two centuries ago, BNY Mellon is the world's biggest custody bank. 
>
> Until now, fund managers would have had to custody their digital currencies with a crypto specialist. BNY Mellon said it is the first of the eight systemically important U.S. banks to store digital currencies and allow customers to use one custody platform for both its traditional and crypto holdings. 
>
> "We are excited to help drive the financial industry forward," Robin Vince, BNY Mellon's president and chief executive, said in a statement. 

It probably won't happen, right? The point of doing crypto custody with BNY Mellon, as opposed to "a crypto specialist," is that you are expecting the security, regulation, and not-being-hacked-too-much of traditional finance. Still you might worry: BNY Mellon's pot of crypto will be as attractive to hackers as any crypto exchange's pot of crypto, and it might have _less_ experience and expertise in securing crypto than "a crypto specialist" would. The question is whether being hacked constantly is a feature of crypto _exchanges_, or just a feature of _crypto_.

Elsewhere in [crypto custody](https://www.theguardian.com/technology/2022/oct/11/crypto-com-accidental-transfer-10-5-million-trial-australia-couple-cryptocurrency):

> A Victorian woman accused of theft over a $10.5m mistaken cryptocurrency refund has been released on bail as she awaits trial, despite claims she allegedly tried to flee the country.
>
> Thevamanogari Manivel and her partner, Jatinder Singh, appeared by video link from prison in Melbourne magistrates court on Tuesday when they were committed to stand trial on theft and other charges.
>
> In May 2021, Crypto.com intended to refund Manivel $100 but she was erroneously transferred $10.47m. The company did not notice the mistake until an audit was conducted in December.
>
> A worker in Bulgaria, who processed the refund, had entered the wrong numbers into an Excel spreadsheet, Michi Chan Fores, a Crypto.com compliance officer, told the court.

It would be funny if "the blockchain" was just a euphemism for "an Excel spreadsheet."

## NFT Stuff

I guess you have three options:

1. Pay Damien Hirst £2,000 and get one of his dot paintings; 
2. Pay Damien Hirst £2,000 and _not_ get one of his dot paintings; or
3. Don't pay Damien Hirst £2,000 at all.

I know what I would choose (what I have chosen), but the market seems [pretty evenly divided between Options 1 and 2](https://web.archive.org/web/20221012050322/https://www.msn.com/en-gb/money/other/damien-hirst-to-burn-thousands-of-his-paintings-after-owners-refuse-to-switch-to-nfts/ar-AA12NM6t):

> Damien Hirst will burn thousands of his artworks on Tuesday after owners refused to exchange their paintings for a non-fungible token (NFT).
>
> The British artist and art collector created 10,000 unique dot paintings in 2016 which corresponded with a collection of 10,000 NFTs, a unique digital token that can be traded online.
>
> In "The Currency", Hirst's first NFT collection, he gave his buyers the choice to exchange their NFT version - worth £2,000 - for the physical artwork.
>
> After the exchange period closed in July it was revealed that just over half the collectors chose to exchange for the real artwork, created by enamel paint on handmade paper, while 4,851 decided to keep the NFT version.
>
> Hirst, reportedly the UK's wealthiest living artist, pledged to destroy all the original artworks that people decided not to exchange their virtual token for.
>
> As a result, he will torch thousands of paintings - collectively worth almost £10 million - starting on Tuesday afternoon at the Newport Street Gallery in London.

The advantages of not exchanging your NFT for the physical artwork are (1) this way you don't have to find a place to hang a Damien Hirst dot painting in your house and (2) the image of Damien Hirst lighting thousands of his paintings on fire because nobody wants them is in fact very funny, and you have contributed to that act of comedy. The disadvantages are (1) you paid him £2,000 and (2) now you have nothing. Oh you have an NFT, you have an NFT, you have an NFT.

Anyway the conflagration is today; [here's how it's going](https://www.bbc.com/news/entertainment-arts-63218704):

> Asked how he felt to be burning the works, Hirst said: "It feels good, better than I expected."
>
> The artist was dressed in silver metallic boiler-suit trousers and matching fire safety gloves as he collected each piece and burned it in a contained fire box. …
>
> Livestreaming the event, the Turner Prize winner and assistants used tongs to deposit individual pieces stacked in piles into fireplaces in the gallery as onlookers watched.
>
> "A lot of people think I'm burning millions of dollars of art but I'm not," Hirst said. "I'm completing the transformation of these physical artworks into NFTs by burning the physical versions."

The market for NFTs [has collapsed](https://www.reuters.com/technology/nft-sales-plunge-q3-down-by-60-q2-2022-10-03/), but in the bull market of 2021 thousands of artists and hucksters had this exact same idea, which was "I will make or acquire some art object, light it on fire, and sell an NFT 'of' the incinerated object to crypto people." Hirst, being an art industrialist, introduced mass production into the mix, but his basic idea was an exact copy of everyone else's. The "object-fire-token-money NFT cycle," [I have called it](https://www.bloomberg.com/opinion/articles/2021-05-24/merrill-lynch-puts-down-the-phone).

As a matter of finance, I cannot fault this: If you can identify a bubble, and you have some free time, the right move is to sell into the bubble. But as art I hate it. [It's so stupid](https://www.bloomberg.com/news/newsletters/2021-09-10/money-stuff-fungible-slices-of-non-fungible-tokens)! Everyone involved should be incredibly embarrassed! What an absolute lack of creativity! Everything about this is the opposite of art! If you find yourself lighting thousands of your paintings on fire because nobody wants them, the obvious conclusion to take from that is that you are a bad artist, and that conclusion is correct!

---
There are three classic problems that you might encounter if you try to use Bitcoin to pay for goods and services. The first problem is that your Bitcoins might go astray: Bitcoin transactions are irreversible and involve sending money to long complicated addresses, and people are constantly trying to steal them. So if you send someone Bitcoin to pay for something, there will probably be a typo in the address and the person won't get it and you'll have to send it again and your first payment will just be permanently lost.
The second problem is that Bitcoin is very volatile, and even people who accept payment in Bitcoin tend not to _denominate_ it in Bitcoin. So if you send someone $100 worth of Bitcoin to buy a $100 thing, the price of Bitcoin might drop 10% while you're sending it, and then they'll say "you only sent me $90" and you'll have to top them up with more Bitcoin.
The third classic problem is that, if you are using Bitcoin to pay for goods and services, there is a good chance that you are paying for something illegal, and Bitcoin payments are traceable. So if you send someone $16,000 worth of Bitcoin to buy a $16,000 thing, (1) some of your money will go missing in transit, (2) the Bitcoins you send won't be worth $16,000 and you'll have to send some more, and (3) the $16,000 thing was a murder and now you are in prison.

## Grayscale premia

A lot of people, it turns out, want exposure to crypto _prices_ without exposure to crypto _infrastructure_. Like: Bitcoin was created as sort of an alternative financial infrastructure, a new kind of money that dispenses with the need for banks and other intermediaries. But in fact Bitcoin is not a particularly good form of money (its value is volatile, it is not widely used for payments in a lot of places), but it is a very good sort of financial asset (its value has gone up a lot over the last 14 years, and also recently). So a lot of people want to _own Bitcoin_ (because they think the price will go up) without believing in, or caring about, its underlying philosophy of decentralization and disintermediation. So they go to their (traditional) bank or (traditional) brokerage and say "buy me some Bitcoin."

And there are lots of products designed to satisfy that desire: Bitcoin futures and, soon, probably, [spot Bitcoin exchange-traded funds](https://www.bloomberg.com/opinion/articles/2023-08-29/grayscale-can-be-a-bitcoin-etf) that let you buy exposure to Bitcoin without ever leaving the traditional financial system. Someone else will do the arbitrage for you, buying Bitcoins to sell you Bitcoin futures or ETFs, and you'll just have a thing in your regular brokerage account that moves up and down with the price of Bitcoin.

I have [written](https://www.bloomberg.com/view/articles/2017-12-19/bitcoin-futures-are-a-great-way-to-not-own-bitcoin) about this [before](https://www.bloomberg.com/opinion/articles/2023-11-01/trade-the-news-then-publish-it) and it seems fine to me? If the _only_ possible thesis for buying Bitcoin was "this is the future of money and the entire traditional financial system will be replaced by crypto," then buying Bitcoin in an ETF would be a little contradictory. But in the actual world of 2023 it's fine.

I don't really get the case for a Filecoin ETF? The Financial Times reports:

> Some cryptocurrency funds run by the world's largest crypto manager are trading at as much as eight times their underlying value amid an unprecedented buying frenzy. ...
>
> The mania has spread to a host of private trusts operated by Grayscale. The company's Filecoin Trust is trading at $34.25, 721 per cent above its net asset value of $4.17, having hit a premium of more than 1,000 per cent in November.
>
> Its trust tracking solana, the third-largest cryptocurrency after bitcoin and ether, is at a premium of 302 per cent, while those investing in chainlink, livepeer, lumens and Decentraland's mana token are priced at between twice and four times their NAV.
>
> "It's absurd. I feel the investor doesn't really understand what they are getting into," said Bradley Duke, chief strategist of ETC Group, which runs more than $1bn in European-listed crypto exchange traded products.
>
> "I wouldn't know what [investors] could be thinking buying at these prices," said Bryan Armour, director of passive strategies research, North America, at Morningstar. "A lack of understanding can easily be part of it."
>
> The funds can only be traded via the over-the-counter "pink sheets" market, where secondary trading in pre-existing shares takes place. Shares cannot be redeemed, while new shares can only be created if Grayscale carries out a private placement exercise, meaning there is no arbitrage mechanism to bring prices back in line with the underlying holdings.

To be clear, these Grayscale trusts are _not_ ETFs, because you can't create or redeem them; if they were ETFs they probably wouldn't trade at those crazy premiums. (You'd go buy a ton of Filecoins and give them to Grayscale to get back trust shares, etc.) But Grayscale's biggest trust is the one tracking Bitcoin; it has traded at a discount for a long time, but that discount has closed significantly now that everyone expects the trust to convert into an ETF (and thus allow redemptions). That optimism has been good for the price of Bitcoin too, and for the prices of crypto generally, and also apparently for the prices of Grayscale altcoin trusts. 

Bitcoin is a popular financial asset, "digital gold," a possible diversifier for retail and institutional investors. Filecoin is … the payment currency for a [peer-to-peer file storage system](https://docs.filecoin.io/basics/what-is-filecoin)? Why would you buy it in a pink-sheet wrapper? The [Grayscale Filecoin Trust](https://www.grayscale.com/crypto-products/grayscale-filecoin-trust) is tiny (half a million dollars under management), but owning Filecoin that way is (1) less useful and (2) vastly more expensive than owning it directly. 

One possible answer is of course "a lack of understanding"; again, this stuff is very small. I suppose another answer is, like, "crypto projects like Filecoin are good and valuable, and their tokens are sort of like stock in those projects, but the _stock exchange for trading those stocks_ will be the regular stock exchange, not decentralized finance." Last year it was almost plausible to think that the crypto financial system might consume the regular financial system, that in the future all the stocks will be tokenized. Now it's more plausible to think the reverse, that the regular financial system will consume the crypto one, that in the future all tokens will be stock-ized.

## Spot Bitcoin ETFs

One claim that you sometimes hear about crypto is that it gets rid of middlemen: Instead of relying on a bank to hold your money for you, you can hold it directly on the blockchain. But one reason that crypto is _actually popular_ - a reason that it has gotten a lot of attention, and that a lot of people from the financial and tech industries have gotten into crypto - is that it is [insanely lucrative for middlemen](https://www.bloomberg.com/opinion/articles/2021-02-25/gamestop-is-happening-again). A lot (not all) of the basic products of traditional finance are old and well understood and heavily regulated and fiercely competitive; margins are low and bid/ask spreads are slim. Whereas crypto is relatively new and poorly understood and complicated and illiquid and you can charge 2% on every trade. Sam Bankman-Fried did not briefly become the world's richest young person because crypto _got rid of middlemen_. Quite the opposite.

Meanwhile it is probably a positive for crypto if it becomes mainstream, if it is widely adopted by ordinary investors and traditional institutions. That would lead to a lot of money flowing into crypto, which is probably good for the crypto middlemen. On the other hand it would probably lead to a collapse in _margins_ for crypto middlemen: They got fat by charging 2% on every trade, but you can't do that forever if the product becomes mainstream. Some middlemen may have trouble adapting.

So [Bloomberg's Katie Greifeld reports](https://www.bloomberg.com/news/articles/2024-01-08/grayscale-s-1-5-fee-for-gbtc-would-be-highest-among-proposed-spot-bitcoin-etfs):

> As spot Bitcoin ETF hopefuls rush to file their final documents with US regulators, a key difference is emerging among the applicants in their proposed fee structures.
> 
> At the top end: The Grayscale Bitcoin Trust, which would carry a 1.5% fee if the US Securities and Exchange Commission approves its conversion into an exchange-traded fund. While that would be lower than GBTC's current 2% fee, it comes well above its competitors.
> 
> The race-to-the-bottom on fees is a feature of the highly competitive $8 trillion US ETF industry, where even a couple of basis points of difference can translate into millions of dollars worth of inflows.
> 
> While GBTC has an enormous advantage in existing assets - it boasts $27 billion in assets as a trust since its 2013 inception - its competitors will charge a fraction of its proposed expense ratio. … BlackRock intends to charge 0.2% for the first year or until it reaches $5 billion in assets, with 0.3% as its eventual fee.

Yeah look the fees for [keeping Bitcoins in a pot](https://www.bloomberg.com/opinion/articles/2024-01-04/put-the-bitcoins-in-the-box) can be decomposed into: 

1. There is a cost to actually keeping the Bitcoins in a pot. You gotta worry about custody and security, and set up the trading mechanics for Bitcoins to come in and out of the pot. This costs real money; a spot Bitcoin exchange-traded fund won't have the near-zero fees of an S&P 500 index fund.
2. If you are the first person to offer "Bitcoins in a pot" as a product, you can charge a huge premium.

But eventually, like, BlackRock will catch up, and then you probably can't.

## SEC Bitcoin ETF hack

I kind of don't understand [the trade here](https://www.bloomberg.com/news/articles/2024-01-09/sec-says-has-not-yet-granted-approval-of-spot-bitcoin-etfs)?

> A highly anticipated decision by the US Securities and Exchange Commission on whether to approve a spot-Bitcoin exchange-traded fund quickly morphed into a major cybersecurity incident on Tuesday.
> 
> The SEC's X account was compromised and a fake post claiming that the agency had green lit plans for the products fueled a brief surge in the price of the world's biggest cryptocurrency. It also has sparked an investigation by US authorities into how a social media account at Wall Street's main regulator was compromised. …
> 
> The breach gave fodder to crypto faithful who have long viewed the commission's chair, Gary Gensler, as an enemy due to his zeal to rein in the industry. The irony of a cybersecurity incident befalling a regulator that's repeatedly warned of crypto's online vulnerabilities was not lost on critics who have spent years waiting for the SEC to approve a Bitcoin ETF. Traders have been speculating for weeks that the agency could approve several of the products as soon as Wednesday.
> 
> In statements late Tuesday, the regulator said that it would work with law enforcement to investigate the incident, the unauthorized access had been terminated, and that the post wasn't made by the SEC or its staff. In a separate statement, Gensler clarified that no decision on ETFs had been made.

Look, I have no inside information, but most of the reporting I have read about spot Bitcoin ETFs has said that 

1. the SEC is going to approve them,
2. by the end of today, and
3. this is public knowledge that everyone believes.

So you would think it would be pretty priced in? It just does not seem to me like there would be a ton of alpha in (1) constantly refreshing the SEC's Twitter account, (2) looking for a tweet saying "okay spot Bitcoin ETFs are cool now," and (3) buying Bitcoin on the news. Which implies there would not be a ton of alpha in (1) buying a bunch of Bitcoin, (2) _hacking_ the SEC's Twitter account, (3) _tweeting_ "okay spot Bitcoin ETFs are cool now" and (4) selling your Bitcoin into the resulting enthusiasm.

[There was a little though](https://www.bloomberg.com/news/articles/2024-01-09/bitcoin-fluctuates-after-debunked-post-claimed-etfs-won-approval):

> The false post on the SEC's X account was up for a number of minutes before the agency clarified that it was inaccurate. In that period, Bitcoin posted a relatively modest jump to almost $48,000 from about $46,700 before falling back toward $45,000.

Eh? If you bought Bitcoin at $48,000 upon seeing that tweet, and then sold it at $45,000 after realizing that the tweet was fake, I would love to hear from you. Why? Why not just wait? If you think Bitcoin is worth $48,000 when the SEC approves spot Bitcoin ETFs, then … I mean … the tweet was fake, but if the contents of the tweet turn out to be true _today_, won't you regret selling yesterday?

Fine, yes, probably someone hacked the SEC's Twitter to do some market manipulation here: They wanted to bet on, what, a 2.5% short-term move in Bitcoin prices, and they made that bet pay off with a fake SEC tweet. But I have [suggested before](https://www.bloomberg.com/opinion/articles/2023-11-15/wework-s-rescue-wasn-t-real) that there are two possible reasons to issue fake announcements that move asset prices:

1. Market manipulation: You buy the asset, you issue the fake announcement, the price moves, you sell it at a profit; or
2. General trolling and hijinks: You don't buy the asset, you issue the fake announcement, the price moves, you have a laugh and high-five your online friends.

Doesn't it seem at least _possible_ that this hack was just trolling? It didn't move Bitcoin prices that much, and it _shouldn't have:_ The fake announcement was something that everyone expects to actually be true today. But it is very funny? The key element of online trolling is irony, and there is plenty of irony here. Like: 

1. The crypto community and the SEC do not particularly like each other: Gensler's SEC has launched a [broad](https://www.bloomberg.com/opinion/articles/2023-06-06/the-sec-comes-for-crypto) and [aggressive](https://www.bloomberg.com/opinion/articles/2023-07-14/ripple-is-a-security-and-it-isn-t) crackdown on crypto, and it is only going to (probably!) approve spot Bitcoin ETFs today because [a court forced it to](https://www.bloomberg.com/opinion/articles/2023-08-29/grayscale-can-be-a-bitcoin-etf). If you're a Bitcoin enthusiast with the skills to hack the SEC's Twitter, you might want to manipulate the price of Bitcoin, but you might also just want to make the SEC look bad.
2. Having the SEC (1) announce that Bitcoin ETFS are approved, (2) walk back that announcement, and then (3) announce it again, for real this time, _the next day_, really is quite embarrassing. Like if the hacker made the SEC say something outlandish and false, that would be a little funny. But making the SEC _say something true a day early_ is extremely funny.
3. In addition to cracking down on crypto, one of the SEC's big regulatory priorities under Gensler has been [punishing companies](https://www.bloomberg.com/opinion/articles/2023-11-16/hackers-know-everything-is-securities-fraud) for [cybersecurity incidents](https://www.sec.gov/news/press-release/2023-139). The SEC once [sued a company for using weak passwords](https://www.bloomberg.com/opinion/articles/2023-10-31/bad-passwords-are-securities-fraud), and its enforcement director said that the case "underscores our message to issuers: implement strong controls calibrated to your risk environments." But apparently the SEC's Twitter was compromised because it [didn't turn on two-factor authentication](https://www.ft.com/content/60efd3f4-62c9-42e5-8b32-4761eaa19b5a). Nyah nyah nyah nyah nyah!

I don't know, the whole thing works better as trolling than as market manipulation. 

A few further ironies. First, it does bear mentioning that X, formerly Twitter, is owned by Elon Musk, who (1) [loves trolling](https://www.bloomberg.com/opinion/articles/2021-05-17/elon-musk-controls-bitcoin-and-dogecoin-prices-with-pure-magic) and (2) hates the SEC. "I want to be clear. I do not respect the SEC. I do not respect them," is one of the nicer things Musk has [said in public](https://www.bloomberg.com/opinion/articles/2019-02-26/elon-musk-keeps-tweeting) about the SEC. It is … convenient and funny … that Musk's Twitter was used yesterday to make the SEC look stupid. I mean, it's not necessarily great for Twitter/X/Musk [as a business matter](https://www.bloomberg.com/news/articles/2024-01-10/sec-s-compromised-account-amplifies-x-trust-security-concerns):

> The high-profile breach comes at a time when X and billionaire owner Elon Musk are seeking to win back trust from both users and advertisers, many of which have been dismayed by Musk's free-for-all style of leadership since his 2022 takeover. Musk has pivoted away from some of the prior regime's efforts to rein in offensive or harmful content, and has severely scaled back staff to save on costs. Those cuts have led to regular bugs and outages.
> 
> "This has to be the most sophisticated use of a stolen Twitter account ever," said Alex Stamos, chief trust officer at SentinelOne and former security chief at Meta Platforms Inc. "At a minimum, this indicates that the hollowed-out X team can't keep up with advances in account takeover techniques."

But it's definitely a point for Musk in his long dumb game of trolling the SEC.

To be clear, I am not saying it is _likely_ that Elon Musk, who controls Twitter, took over the SEC's account in order to tweet a fake announcement to troll the SEC. I think the likelihood of that is close to zero. I am just saying that it would be the absolute funniest Money Stuff story of all time. Just all of my interests, right there.

Another irony: I like to say around here that "everything is securities fraud," and so of course when this story came out people emailed me to say "is this securities fraud yuk yuk yuk." But: no? I mean, nothing here is legal advice, and everything is securities fraud, but let's say that someone hacked the SEC to manipulate the price of Bitcoin. Bitcoin is not a security? The SEC [thinks that almost every crypto asset is a security](https://www.bloomberg.com/opinion/articles/2023-06-07/when-is-a-token-not-a-security), but it really does make a single explicit exception for Bitcoin. So if the SEC figures out who hacked its Twitter account, and if it figures out that that person did it to make a quick profit on Bitcoin by manipulating the market and deceiving investors, that's still not securities fraud. It's regular fraud, it's wire fraud, maybe it's commodities fraud, but whatever it is is not under the SEC's jurisdiction. The SEC "said that it would work with law enforcement to investigate the incident," but it has no power _itself_ to bring charges against anyone for manipulating Bitcoin.

Still, there are securities that are tied to the price of Bitcoin, and whose prices would be influenced by news about Bitcoin ETFs, and which were arguably manipulated by this fake tweet. The most obvious examples would be  … spot Bitcoin ETFs? Those don't trade yet. Because the SEC hasn't approved them. So the fake tweet couldn't have manipulated them. But Bitcoin _futures_ ETFs _do_ trade, as does the Grayscale Bitcoin Trust (GBTC), a pot of Bitcoins that hopes to convert into an ETF. I suppose you could have manipulated their prices with this tweet. The tweet went out after 4 p.m. so the stock market was closed, but the price of the ProShares Bitcoin Strategy ETF did in fact bounce around a bit in after-hours trading yesterday; it closed at $22.72 and spiked as high as $23.50 at 4:12 p.m., after the tweet. So, sure, securities fraud, fine.

Anyway, the great counter-troll here would be for the SEC to [announce today](https://www.wsj.com/finance/regulation/secs-decision-on-spot-bitcoin-etfs-could-go-a-few-different-ways-96d76589) "you know what, all the Bitcoin ETF applications are rejected, we'll see you in court again. We _were_ going to approve them, but it turns out that the Bitcoin market is still too vulnerable to manipulation, as you can tell by the fact that someone hacked our Twitter to manipulate Bitcoin."

## Elsewhere in Bitcoin ETFs

One rude but not entirely inaccurate way to describe the business model of Grayscale Investments LLC is:

1. Grayscale operates a pot, the Grayscale Bitcoin Trust (GBTC), into which people can put Bitcoins.
2. They cannot take them out.
3. Grayscale pays itself 2% of the value of the pot every year in fees.

This is not a good business model, when you describe it that way - who would put Bitcoins into the pot? - but it is an _extremely_ good business model if you _don't_ describe it that way. There's like [$29 billion in the pot](https://etfs.grayscale.com/gbtc). The fees are good. Meanwhile people whose Bitcoins are in the pot sometimes [sue to get them out](https://www.bloomberg.com/opinion/articles/2023-03-07/ftx-wants-its-bitcoins-back-from-grayscale), or at least to cut the fees, but that doesn't work.

This description is very rude because Grayscale does _want_ people to be able to get their Bitcoins out: It has [filed to convert GBTC into an exchange-traded fund](https://www.sec.gov/Archives/edgar/data/1588489/000119312524003901/d144925ds3a.htm), which would allow for efficient creations (putting more Bitcoins in) and redemptions (taking Bitcoins out). And Grayscale sued SEC to force it to allow this conversion, and [last year it won](https://www.bloomberg.com/opinion/articles/2023-08-29/grayscale-can-be-a-bitcoin-etf), and everyone expects the SEC to approve Grayscale's application to turn GBTC into an ETF [by today](https://www.bloomberg.com/news/articles/2024-01-09/bitcoin-btc-rally-cools-near-47-000-in-countdown-to-sec-etf-decision). And a bunch of other issuers have filed to launch Bitcoin ETFs, and the SEC will probably approve them too, and GBTC will have competition.

We [talked a bit on Monday](https://www.bloomberg.com/opinion/articles/2024-01-08/elon-musk-isn-t-getting-enough-sleep) about how this will affect Grayscale's business model. One problem is: The ETF structure will allow investors to take Bitcoins out of GBTC. Another problem is: All those _other_ Bitcoin ETFs will charge _[much lower fees](hhttps://www.bloomberg.com/news/articles/2024-01-09/four-bitcoin-etf-hopefuls-slash-fees-before-funds-even-launch)_ than Grayscale. Grayscale has already said that its fees will go down to 1.5% once it converts into an ETF, which is less than the current 2%, but still way more than the 0.3% that BlackRock plans to charge. I wrote:

> If you are the first person to offer "Bitcoins in a pot" as a product, you can charge a huge premium.
> 
> But eventually, like, BlackRock will catch up, and then you probably can't.

A reader emailed to point out that this isn't necessarily the whole story. If you are the first person to offer "Bitcoins in a pot," people will put Bitcoins in your pot, and GBTC does have $29 billion of Bitcoins. And those Bitcoins have appreciated in value: Most of them were put in the pot at considerably lower Bitcoin prices than today's $46,000-ish, and Grayscale [stopped putting new Bitcoins in](https://www.coindesk.com/markets/2021/03/10/grayscale-halts-new-investments-in-gbtc/) the pot [in 2021](https://fintel.io/fg/us/gbtc/CommonSharesOutstanding). If you bought GBTC shares in 2019, or most of 2022 or 2023 for that matter, your shares are worth much more than you paid for them.

This is good for you, generally, but it is a tax problem: If you _sell_ your GBTC shares, you'll have a big gain and have to pay taxes on it. If you just keep those shares, you don't pay taxes (yet). That is a reason not to sell.

Soon, probably, you will have your choice of Bitcoin ETFs. They will all be about the same, and you might prefer to buy one with 0.2% fees rather than one with 1.5% fees. But if you _already own_ shares in Grayscale's Bitcoin trust when it converts to an ETF, the math isn't so simple. If you _sell_ the Grayscale ETF and _buy_ a cheap one, you will save on annual fees - but you'll probably pay a lot of taxes on your gains. Paying 15% or 20% capital gains taxes on 50% or 80% gains on your GBTC shares might look a lot more expensive than paying an extra 1.3% per year in fees.

## Bitcoin ETF

Taking a step back here, there is something really cool about what Bitcoin has accomplished, in some ways much cooler than [Satoshi Nakamoto's original vision](https://bitcoin.org/bitcoin.pdf) for it. The original vision of Bitcoin was that it would be "electronic cash," a way for people to send payments to each other without involving a bank or other intermediary. Fifteen years later, I mean, there has been _some_ progress along those lines; _some_ people sometimes do pay for some goods and services using Bitcoin. But it has not exactly taken over the world of payments. El Salvador made Bitcoin legal tender and required all businesses to accept it, and even there it is [not that widely used](https://www.nber.org/digest/202207/el-salvadors-experiment-bitcoin-legal-tender). In big developed economies, despite years of crypto proselytizing, people still much prefer fiat currency and traditional banks.

And yet the price of Bitcoin has gone from zero in 2009 to $46,000-ish today, not on widespread adoption as a _payments_ mechanism, but because people - lots of people, crypto evangelists but also regular retail investors and quite traditional investment strategists at big institutional investment firms - view it as a "store of value." Which means that they think its price will go up, or at least not go down, robustly and for the long term. They buy Bitcoin at $46,000 not because they plan to use it as digital cash, but because they think other people will buy it at $47,000, or $470,000 or whatever. 

Which is why people buy Apple Inc. stock, or Treasury bonds or oil futures or whatever: They think other people will buy them, so the price will go up. You know [what Keynes said](https://en.wikipedia.org/wiki/Keynesian_beauty_contest). But those things have cash flows or industrial uses; those things are claims on economic activity. Bitcoin is just a thing a guy made up 15 years ago. Its function as a store of value is almost purely self-referential: Not "this is worth $X because other people will buy it for $X because other people will buy it for $X because … [etc.] … other people think its cash flows have a present value of $X," but "this is worth $X because other people will buy it for $X because other people will buy it for $X" all the way down.

Bitcoin is an astonishing _social technology._ It would, in the abstract, be useful for the world if there was just an entry in a computer database that we all agreed was valuable _just because_, with no reference to any underlying commodity or series of cash flows or industrial activity. Just a number that was valuable. And so someone invented it. Traditionally _currency_ works sort of like that: The US dollar is this sort of social technology; it has value because it has value, not because it has cash flows. But there's a whole ton of complex and long-standing social technology that goes into that; the US has a government and an army and an income tax and a debt stock and a trade balance, which help to preserve the value of the dollar.

Bitcoin expresses the thesis that it would be good to have a valuable database entry _without_ that, just something was valuable because people on the internet voluntarily agreed it was valuable, with no government or army or taxes or anything else. And it worked! That did happen. It has value due to a broad voluntary market consensus based almost entirely on itself. In some sense that consensus is fragile - if a thing is valuable only because people think that it is valuable, it could stop being valuable when they stop thinking that - but in another sense that is true of any social fact: The dollar is valuable, the King of England is the King of England, the US is a liberal democracy, etc., exactly as long as those facts command social consensus. Bitcoin got to what seems like a pretty robust consensus in 15 years. That's just neat.

Anyway, [as expected](https://www.bloomberg.com/news/articles/2024-01-10/spot-bitcoin-etfs-approved-to-launch-in-us-by-gensler-s-sec):

> US regulators for the first time approved exchange-traded funds that invest directly in Bitcoin, a move heralded as a landmark event for the roughly $1.7 trillion digital-asset sector that will broaden access to the largest cryptocurrency on Wall Street and beyond.
> 
> The Securities and Exchange Commission, whose three-part mandate includes investor protection, authorized funds from industry heavyweights BlackRock, Invesco and Fidelity to smaller competitors including Valkyrie to begin trading Thursday.
> 
> The approvals mark a rare capitulation by the SEC following opposition that lasted for more than a decade, ever since Tyler and Cameron Winklevoss first proposed a Bitcoin ETF in 2013. BlackRock Inc.'s surprise application last June, followed by an appeals court ruling that called the denial of a different application "arbitrary and capricious," triggered a blistering rally in the cryptocurrency amid speculation that US regulators would finally give their blessing to the structure.

There is something pure about this, as Bitcoin news. A Bitcoin ETF is vastly _less_ useful, as a payments mechanism or a way to supplant the traditional financial system, than just buying Bitcoin: Instead of an alternative peer-to-peer payments system in which everyone can hold their Bitcoins directly and transfer them to each other without middlemen, this is a crypto thing that you can hold in your traditional brokerage account and not use for payments at all. But it is _more_ useful as a store of value: You can hold it in your brokerage account, where you hold your stores of value. You don't have to mess around with an alternative financial system; you can just isolate the store-of-value component of Bitcoin and hold it directly. And so the price of Bitcoin ran up in anticipation of the ETF approvals, because everyone expected that the ETFs would lead to more people holding Bitcoin as a store of value. Which is the best reason for Bitcoin to go up.

## Sell the news

The SEC approved the spot Bitcoin ETFs a little after the close yesterday (Wednesday) afternoon. A little after the close on _Tuesday_ afternoon, the SEC's account on X (formerly Twitter) tweeted that it had approved spot Bitcoin ETFs. That turned out to be fake; the SEC's Twitter got hacked. The SEC had to walk back that statement on Tuesday, and then walk it forward again on Wednesday. We [talked about this yesterday](https://www.bloomberg.com/opinion/articles/2024-01-10/the-sec-got-trolled-on-bitcoin-etfs). "Nyah nyah nyah nyah nyah," I wrote.

When the Bitcoin ETFs got fake-approved on Tuesday, the [price of Bitcoin](https://www.bloomberg.com/opinion/articles/2024-01-10/the-sec-got-trolled-on-bitcoin-etfs) "posted a relatively modest jump to almost $48,000 from about $46,700 before falling back toward $45,000" when it turned out to be fake. I was a little perplexed - everyone expected the ETFs to be approved by today, so the fake tweet didn't add much fake information, and the retraction didn't add much real information - but whatever. The fun fact is that, when Bitcoin ETFs got approved for real on Wednesday, the price of Bitcoin … jumped to a bit more than $49,000, from a bit more than $46,000, [before falling back](https://www.bloomberg.com/news/articles/2024-01-11/bitcoin-btc-volume-jumps-as-first-us-spot-etfs-begin-trading):

> Bitcoin pared gains after surging past $49,000 for the first time since December 2021 with trading commencing for the first US exchange-traded funds that invest directly in the biggest cryptocurrency.
> 
> The token had advanced as much as 6.7% to $49,021, buoyed by the approval of spot Bitcoin ETFs by the US Securities and Exchange Commission after markets closed on Wednesday. It was recently trading at around $46,000. Most smaller tokens, such as Ether, Cardano and Polkadot were higher.
> 
> All of the 11 ETFs are trading, and over $2.6 billion has changed hands in just the first few hours of trading. 

The market reaction to the SEC's fake approval of Bitcoin ETFs - a quick modest spike followed by a disappointed modest fall - is remarkably similar to the market reaction to the SEC's _real_ approval of Bitcoin ETFs.

Also, I wrote yesterday that, while it is possible that someone hacked the SEC's Twitter to make money by manipulating the price of Bitcoin, it was also possible that whoever did the hack was just trolling for fun, and did _not_ make any money by manipulating Bitcoin. Several readers emailed to point out the strongest argument for that possibility: If you wanted to manipulate the market, you would _short_ Bitcoin and then hack the SEC to tweet "we're once again _declining_ to approve Bitcoin ETFs, too many problems, we're confident we'll win in court this time." The market really expected the SEC to approve the ETFs, so there was not a ton of information in Tuesday's fake tweet, and it didn't move the price of Bitcoin that much. But if the fake tweet had _confounded_ expectations, _that_ would have moved the market. If you were a ruthless hacker/manipulator looking to maximize profits, that's what you'd do. If you were a crypto enthusiast looking to troll the SEC for fun, though, you'd fake-tweet that the ETFs were approved.

Also, by the way, the SEC's approval is hilariously grudging. Here's SEC Chair [Gary Gensler's statement](https://www.sec.gov/news/statement/gensler-statement-spot-bitcoin-011023):

> Though we're merit neutral, I'd note that ... bitcoin is primarily a speculative, volatile asset that's also used for illicit activity including ransomware, money laundering, sanction evasion, and terrorist financing.
> 
> While we approved the listing and trading of certain spot bitcoin ETP shares today, we did not approve or endorse bitcoin. Investors should remain cautious about the myriad risks associated with bitcoin and products whose value is tied to crypto.

And here is Commissioner [Caroline Crenshaw's dissent from the approval](https://www.sec.gov/news/statement/crenshaw-statement-spot-bitcoin-011023):

> Spot bitcoin markets are subject to fraud and manipulation. One form of manipulation that appears to be pervasive in the crypto markets (and specifically bitcoin markets), is wash trading, a practice whereby traders seek to increase the appearance of high trading interest by both selling and buying the same products at the same time, often driving up prices, and then selling to unwitting third party market participants at inflated values. Wash trading distorts price and volume, causes volatility, reduces investor confidence and participation in financial markets, and of course, results in investor harm. One analysis of 29 major crypto exchanges found that wash trading was, on average, as high as 77.5% of the total trading volume on unregulated exchanges. ...
> 
> Specifically with regard to bitcoin, an analysis of 157 crypto exchanges found that 51% of the reported daily bitcoin trading volume was likely bogus. In fact, though reporting regarding bitcoin frequently discusses the enormous size of the market, one market participant who now seeks to sponsor a spot bitcoin ETP has admitted that "approximately 95%" of the data used by many participants are "fake and/or non-economic." … In short, prices and demand for bitcoin may not actually be what they appear to be.

I joked yesterday that the SEC should deny all of these applications, saying "We _were_ going to approve them, but it turns out that the Bitcoin market is still too vulnerable to manipulation, as you can tell by the fact that someone hacked our Twitter to manipulate Bitcoin." Crenshaw makes that argument!

> Indeed, just yesterday, prior to the issuance of our approval Order, one of the SEC's social media accounts was compromised, and an unauthorized post falsely indicated that we had approved spot bitcoin ETFs. Unsurprisingly, the price of spot bitcoin suffered "whiplash" in the minutes and hours following the false tweet. While the facts underlying this misconduct hopefully will be uncovered by law enforcement in the future, I will be monitoring what may be yet another attempt to profit from wrongdoing in this market.

## Interest

You could imagine, I suppose, a "physical dollar ETF" that worked like this:

1. You send money to the ETF issuer.
2. The issuer uses your money to buy crisp $100 bills.
3. The issuer keeps the $100 bills in a nice safe vault.
4. The issuer charges fees to cover things like its marketing cost, its cost of renting the vault, etc.

In some rough sense that's how a physical gold ETF works, and it's how a spot Bitcoin ETF works: There's some stuff, the stuff is a store of value, and the ETF keeps the stuff in a physical or cryptographic vault, not doing anything with it.

But in fact there'd be something a bit crazy about doing that with dollars. There are ["cash" ETFs](https://www.ishares.com/us/products/258806/ishares-liquidity-income-etf?cid=ppc:ish_us:ish_us_nb_fixed_income_product_exact:google:nonbrand_prod:ei), in some sense. But everyone understands that these ETFs don't hold _crisp $100 bills_. They hold extremely safe interest-bearing short-term debt instruments. If you invest your money in one of those ETFs, it will "hold" your "cash" for you in roughly the sense that a bank would: It will lend out your cash, as safely as possible, give it back to you on demand, and _pay you interest_. 

This is the natural way of the world, in finance. Even a _stock_ ETF will probably do this: Stock ETFs often take their investors' money, use it to buy stocks, and then _lend out some of those stocks to earn a bit of extra interest_. Modern finance is very interested in efficiency, and abhors the idea of buying anything, putting it in a box, and _doing nothing with it_. You've got some stuff in a box, you take it out of the box, you _lend_ it to someone who wants to do something with it, and you earn interest.

The Satoshi Nakamoto vision of crypto was very different: This idea of building opaque leverage into every part of the system, of constructing everything on webs of debt, is part of what Bitcoin was reacting against.

But the modern vision of crypto, or at least the 2022 vision of crypto, was like everything else in finance. You could hold Bitcoins in your digital wallet, like holding $100 bills in your regular wallet, but the action was in depositing your Bitcoins with some quasi-bank that would lend them out, earn interest, and pay some of the interest to you. This led to various terrible problems, chiefly:

1. Those quasi-banks were [very highly leveraged](https://www.bloomberg.com/opinion/articles/2022-12-05/crypto-had-a-credit-bubble), and when crypto prices fell many of them collapsed and took their quasi-depositors' money with them.
2. The _lending_ done by these platforms was pretty much all in support of speculative trading rather than real-world economic activity: People didn't borrow Bitcoins to buy houses; they borrowed Bitcoins to make bets on Bitcoin prices. So the collapse was pretty sharp.
3. Also a fair amount of fraud.
4. The US Securities and Exchange Commission is [quite convinced](https://www.bloomberg.com/opinion/articles/2021-09-08/lending-bitcoins-is-tricky), for fairly good reasons, that all of those crypto lending platforms were _securities_, subject to securities regulation, and that everyone running those platforms was doing so illegally.

Still, in the long run, if you have a giant pot full of electronic financial assets, and if there is demand to borrow those assets, won't you want to lend them? Ten years from now, if Bitcoin ETFs are still around, is it more likely that they will be "physical" ETFs, just holding inert Bitcoins in a pot, or that they will be money-market-ish ETFs, lending out their Bitcoins to earn interest and passing it along to their investors? 

Of course _today_ the answer is "physical"; the prospectuses for today's Bitcoin ETFs say that they will hold the Bitcoins in custody, not that they will lend them. (Here is [Grayscale's](https://www.sec.gov/Archives/edgar/data/1588489/000119312524006300/d264170d424b3.htm), and here's [BlackRock's](https://www.sec.gov/Archives/edgar/data/1980994/000143774924001125/bit20240109_424b3.htm).) And [SEC Chair Gary Gensler's statement](https://www.sec.gov/news/statement/gensler-statement-spot-bitcoin-011023) on the Bitcoin ETF approvals says: "Importantly, today's Commission action is cabined to ETPs holding one non-security commodity, bitcoin. It should in no way signal the Commission's willingness to approve listing standards for crypto asset securities." Bitcoin lending is a security, in Gensler's view, and not something he wants to approve at this point. 

## Cash vs. in-kind

One other what-will-the-future-bring sort of point about Bitcoin ETFs. The normal way that, say, a stock index ETF works is:

1. Normal people buy and sell shares of the ETF on the exchange: They don't actually give any money to the ETF issuer; they just trade in the secondary market.
2. Arbitrageurs make sure that the price of the ETF and the price of the index stay in line: If the price of ETF shares gets too high, arbs will sell ETF shares and buy the underlying index.
3. To complete the arbitrage, a few big banks or trading firms, called "authorized participants," can _exchange_ the ETF shares for the underlying index: They can collect a basket of all the stocks in the index, deliver them to the ETF issuer, and get back some new ETF shares (this is called "creation), or they can collect some ETF shares, deliver them to the ETF issuer for retirement, and get back a basket of the underlying stocks (this is called "redemption").

ETFs work this way in part for price efficiency reasons (in-kind creation and redemption makes it easier to arbitrage the ETF against its underlying index), in part for operational efficiency reasons (it means the ETF doesn't have to do much trading for itself), and in large part for tax efficiency reasons (it means that the ETF [doesn't have taxable gains](https://www.bloomberg.com/opinion/articles/2019-03-29/deals-on-the-train-are-everyone-s-business) from selling its underlying stocks).

Similarly with a spot Bitcoin ETF, the straightforward mechanism would be to have authorized participants hand Bitcoins to the ETF issuer to get back ETF shares, or hand ETF shares to the issuer to get back Bitcoins. But in fact none of the ETFs approved yesterday work that way. They all use only [cash creation and redemptions](https://www.bloomberg.com/news/articles/2024-01-03/bitcoin-spot-market-still-little-weird-proshares-strategist-says): Authorized participants give the ETF issuer _dollars_ and get back shares, and then the ETF goes and buys new Bitcoins with those dollars. (The main authorized participant for the Bitcoin ETFs [is Jane Street Capital](https://www.bloomberg.com/news/articles/2023-12-29/blackrock-names-jane-street-jpmorgan-as-bitcoin-etf-authorized-participants), though there are a few others.) 

The reason for this [seems to be](https://davidgerard.co.uk/blockchain/2023/12/22/bitcoin-etfs-coming-soon-but-in-cash-only/) that [the SEC doesn't like](https://www.reuters.com/business/finance/blackrock-updates-spot-bitcoin-etf-proposal-allow-cash-redemptions-2023-12-19/) in-kind creation/redemption for Bitcoin ETFs. Grayscale Bitcoin Trust, [in its ETF prospectus](https://www.sec.gov/Archives/edgar/data/1588489/000119312524006300/d264170d424b3.htm), says:

> in common with other spot Bitcoin exchange-traded products, the Trust is not at this time able to create and redeem shares via in-kind transactions with Authorized Participants, and there has yet to be definitive regulatory guidance on whether and how registered broker-dealers can hold and deal in Bitcoin in compliance with the federal securities laws. To the extent further regulatory clarity emerges, the Sponsor expects NYSE Arca to seek the necessary regulatory approval to amend its listing rules to permit the Trust to do so (the "In-Kind Regulatory Approval"). Subject to NYSE Arca seeking and obtaining In-Kind Regulatory Approval, in the future the Trust may also create and redeem Shares via in-kind transactions with Authorized Participants or their designees (any such designee, an "AP Designee") in exchange for Bitcoin. There can be no assurance as to when such regulatory clarity will emerge, or when NYSE Arca will seek or obtain such regulatory approval, if at all.

The problem is that, to be an authorized participant in the ETF, you have to be an SEC-registered broker-dealer, since you are effectively distributing the ETF shares. And the SEC is very skeptical of registered broker-dealers trading in Bitcoin. From an SEC perspective, you can trade ETF shares (as a broker-dealer), or you can trade the underlying Bitcoins (as an unregistered Bitcoin-y trader), but it's tricky to do both. That makes the Bitcoin ETF arbitrage - where you trade the ETF shares _against_ the Bitcoins - tricky.

## BTFP carry trade

Last year the Federal Reserve [created a program](https://www.bloomberg.com/opinion/articles/2023-03-13/svb-couldn-t-ignore-its-losses-but-the-fed-can) to allow banks to borrow short-term at long-term rates? I mean, sort of. What it did was create the [Bank Term Funding Program](https://www.federalreserve.gov/financial-stability/bank-term-funding-program.htm), which has [the following features](https://www.federalreserve.gov/newsevents/pressreleases/files/monetary20230312a1.pdf):

1. Banks can borrow "for a term of up to one year," prepayable without penalty.
2. The interest rate is the one-year overnight index swap rate plus 10 basis points, fixed at the time of borrowing.

So you could borrow for a term of one day to one year, in any case at the one-year interest rate (plus 10 basis points). Ordinarily, longer-term interest rates are higher than shorter-term interest rates: It is usually cheaper to borrow money overnight than it is to borrow it for a year. And so this program was, arguably, very mildly punitive, a classic lender-of-last-resort program along the lines of "lend freely against good collateral at penalty rates," or at least not _subsidized_ rates.

But right now, the reverse is true: The overnight rate is fairly high, because the Fed has raised rates a lot over the past few years, but the one-year rate is lower, because the market expects the Fed to lower rates over the next year. And so the BTFP creates a weird carry trade: Banks can borrow at the BTFP's low one-year rate ([4.87%, today](https://www.frbdiscountwindow.org/)), lend at the higher overnight rate, and match the maturities. You can even match the counterparties: You borrow _from_ the Fed (using BTFP) and lend _to_ the Fed (as reserves, [at 5.40%, today](https://www.federalreserve.gov/monetarypolicy/reserve-balances.htm)) and just get free money. The [Wall Street Journal reports](https://www.wsj.com/finance/banking/the-fed-launched-a-bank-rescue-program-last-year-now-banks-are-gaming-it-43e9cee3):

> Borrowing from the Fed's bank term funding program has increased to new highs in recent weeks, a strange consequence of the market's flip to forecasting multiple Fed rate cuts over the coming 12 months.
> 
> The rate banks pay to use the program, BTFP for short, is tied to future interest-rate expectations. Now that investors have priced in a series of rate cuts later this year, banks are able to pocket the difference between what they pay to borrow the funds and what they can earn from parking the funds at the central bank as overnight deposits. …
> 
> While the Fed offers financing below 5% through its rescue program, it is currently paying banks 5.4% on parked reserve balances.
> 
> Lending in the program hit $141.2 billion this past Wednesday, a new high, up 4% from the prior week and up 25% since the middle of November when forecasts started changing. Most of the volume is still loans from the crisis, and the number didn't move much from July to November.
> 
> The increases don't seem to be a sign of new stress on banks, especially since deposits have ticked up at banks over the same period. It appears more likely the banks are just taking the easy money.
> 
> "We think banks are exploiting a positive arbitrage," Janney Montgomery Scott analyst Christopher Marinac wrote in a note this week.
> 
> The benefit will eventually shrink, if not evaporate completely. The program is set to expire on March 11, barring an extension. On Tuesday, Michael Barr, the Fed's vice chairman for banking supervision, suggested the facility wouldn't be extended.

Good trade!

## Beanie Babies

Let's say you want to start an internet business, and you need money. Here are two ways to raise the money:

1. You incorporate your business and sell stock. This is a pretty traditional way to raise money, and people know how it works. It has some downsides, for you. The main one is that you are giving up some control and ownership of your business: If you sell stock to outsiders, then you will have fiduciary duties to them, you will have to manage the company with their best interests in mind, they might get voting shares and board seats, and they will own a portion of the value of the business. Another downside is that you will be subject to securities regulation. If you sell stock to the public, in the US, the US Securities and Exchange Commission will make you register your offering and disclose a lot of stuff about your business. Even if you only sell stock to sophisticated venture capitalists, and thus avoid registration, you will still be subject to securities _fraud_ rules: If you lie to investors to get them to buy your stock, the investors can sue you, or the SEC can.
2. You can sell _crypto tokens_ that are in some way linked to your business. This is a pretty new way to raise money for a business, one that [had a vogue](https://www.bloomberg.com/opinion/articles/2019-10-14/the-sec-really-doesn-t-like-icos) in the late 2010s and early 2020s. But it is much less standardized than stock, and it is not even obvious what I mean by "crypto tokens that are in some way linked to your business." Perhaps you start some internet business, you issue some crypto tokens, and you promise to use a portion of the revenue from your business to _buy back_ some of those tokens and retire them, to "buy and burn" the tokens. Then if you make a lot of profits, you will buy a lot of tokens, so there will be demand for the tokens and they will be valuable. People buy the tokens today to speculate on your future profitability. This is a common approach taken by actual crypto companies; we have [talked](https://www.bloomberg.com/opinion/articles/2022-11-09/bankman-fried-s-ftx-had-a-death-spiral-before-binance-deal) a few [times](https://www.bloomberg.com/opinion/articles/2022-11-14/ftx-s-balance-sheet-was-bad) about FTT, the stock-like token that FTX Trading Ltd. issued in connection with its crypto exchange. But you could imagine other approaches. You could make the link between your business and the token quite tenuous; you could just start a business called Gloobzorp Inc. and issue tokens with the _name_ Gloobzorp and not promise anything, just hoping that people will buy the tokens to bet, incoherently, on the success of your business.

Which approach should you choose? Well, in, like, 2021, the crypto token approach had some really powerful things to recommend it:

- The rules and norms around fiduciary duties, ownership sharing, etc., were much less developed in crypto than they are in stocks. You could issue Gloobzorp tokens to investors, and raise money, and _not_ give up much in the way of control or profits or ownership interests or anything else. You could sell shares in the business without selling shares in the business - or rather, you could raise money by selling things that looked a little bit like shares in the business, without selling shares in the business.
- Relatedly, the _securities laws_ … arguably? … did not apply to this sort of thing. I mean! There is a lot of argument about that, and we'll discuss some of it. But you could at least _imagine_ that these tokens were not securities, which meant things like (1) you could sell them, broadly, to the public, to raise money to build your business, without registering with the SEC or providing much disclosure, and (2) if you were doing fraud maybe the SEC wouldn't come after you.
- There was a huge boom in crypto, money was pouring in, people weren't asking too many questions, and there was a lot of willingness to believe that every business with "crypto" in the description would revolutionize economics and make all of its investors rich. So you could raise a lot of money on pretty good terms, without much disclosure, without giving up much control or ownership.

If you had the _free choice_ between (1) raising money subject to a lot of rules about disclosure and honesty and fiduciary duties and (2) raising _more_ money with _no_ rules or obligations, wouldn't you take the second option?

But of course, of course, of course, this is not a long-term equilibrium. All the downsides of stock - the fiduciary duties, the sharing of the value of the business, the disclosure obligations - are not _incidental_; they are not just arbitrary punishments visited on entrepreneurs who issue stock. _They're the point_. The _reason_ that entrepreneurs can raise money by issuing stock - they can get real dollars in exchange for pieces of paper saying "this is a share of a business that doesn't exist yet" - is that there is a highly developed system of obligations that reassures investors that those pieces of paper have value. The investors get some rights, some control, some economic ownership, some legal and regulatory protections, in exchange for their money. And that is why they are willing to part with their money. 

And the particular set of rights that exist in the US - Delaware corporate law, SEC disclosure regulation, etc. - generally works pretty well, to the point that lots of foreign companies come to the US to raise money, because subjecting themselves to the burdens of US regulation makes them attractive to investors. Investors trust the US capital markets, because they have a long tradition of being pretty well regulated, which means that they are an attractive place for companies to raise money.

Meanwhile, in _2024_, my description of raising money for a business by issuing a crypto token sounds fake and embarrassing. "What on earth," you probably said as you read it, "nobody does this, this is not a thing." I can only say: It really was, in 2021! But now nobody believes that every business with the word "crypto" in its description will revolutionize economics, people who invested in the earlier crypto offerings [got burned](https://www.bloomberg.com/opinion/articles/2023-06-07/when-is-a-token-not-a-security) when crypto crashed, and crypto fund-raising is a fraction of what it was a few years ago.

If people are willing to give your business money in exchange for _nothing_ then, by all means, take it! But they won't be willing to do that for long.

Meanwhile, these days, the SEC is _quite sure_ that US securities laws _do_, and always did, apply to this sort of thing. If you issued a crypto token to fund a business, with vague promises that the token would participate in the upside of the business, the SEC thinks that that's just the same as issuing stock, and you should be held to the same standards (of disclosure, of not doing fraud) as stock issuers. I [think](https://www.bloomberg.com/opinion/articles/2023-07-14/ripple-is-a-security-and-it-isn-t) they're [right](https://www.bloomberg.com/opinion/articles/2023-08-03/terra-is-usually-a-security) but that's not important right now. 

The SEC is effecting its crackdown on crypto mostly by going after crypto exchanges. The [thinking is roughly](https://www.bloomberg.com/opinion/articles/2023-06-07/when-is-a-token-not-a-security):

1. If all of these crypto tokens are securities, then not only were they all _issued_ illegally (by issuers that didn't register them with the SEC), but they all _trade_ illegally (on crypto exchanges that have not registered with the SEC as national securities exchanges).
2. There are fewer crypto exchanges than crypto issuers, and they are bigger, and shutting them down will shut down crypto much more efficiently than going after all the issuers one by one.

One of the SEC's main targets is Coinbase Global Inc., the big US exchange. The SEC [sued Coinbase in June](https://www.bloomberg.com/opinion/articles/2023-06-06/the-sec-comes-for-crypto), and Coinbase is fighting the case hard. Yesterday a New York federal judge held a hearing on Coinbase's motion to dismiss the SEC's case, and it sounds like it went pretty well for Coinbase. [The Wall Street Journal reports](https://www.wsj.com/finance/regulation/judge-questions-secs-claim-to-regulate-coinbase-ae2f240c):

> A federal judge on Wednesday questioned whether allowing the Securities and Exchange Commission to impose its regulations on Coinbase would give the agency sway over markets it doesn't have authority to supervise. 
> 
> "I want to understand how your standard does not sweep in the collectible market or commodities," U.S. District Judge Katherine Polk Failla told SEC lawyers in the courtroom. "It is a real fear that I have that your argument is just sweeping too broadly." 
> 
> Failla is considering Coinbase's request to dismiss the SEC's civil lawsuit against it filed in Manhattan federal court. She didn't rule at the end of Wednesday's five-hour hearing but is expected to decide in the coming months. 

But even if Coinbase wins, there's something a little hollow about the victory. [Bloomberg News reports](https://www.bloomberg.com/news/articles/2024-01-17/coinbase-argues-crypto-like-beanie-babies-in-sec-case-hearing):

> William Savitt, a lawyer for Coinbase, told US District Judge Katherine Polk Failla that tokens trading on the exchange aren't securities subject to SEC jurisdiction because buyers don't gain any rights as a part of their purchases, as they do with stocks or bonds.
> 
> "It's the difference between buying Beanie Babies Inc. and buying Beanie Babies," Savitt said. …
> 
> Lawyers for the government responded that buying an item like a baseball card or a figurine doesn't mean that someone is buying a stake in the enterprise that makes such items.
> 
> But they said that wasn't the case with tokens sold on Coinbase.
> 
> "When they buy this token, they are investing into the network behind it," SEC lawyer Patrick Costello said. "One cannot be separated from the other."

The SEC's argument here is that crypto tokens are an investment, promising some upside from some business building some network with some potential to do good things. Coinbase's argument _is that they aren't_, that it lists tokens that give investors no rights and that have no claim on any economic activity. Coinbase's argument is that crypto is a trillion-dollar market for Beanie Babies, that it is not a way to raise money to fund real business ideas but simply a way to gamble on collectibles. "No, see, if you buy a crypto token, you get nothing, so there's nothing for the SEC to regulate." A good legal argument! But weird _marketing_!

The problem for crypto is that, to have a big attractive financial market in the long term, you need to have obligations. You need to have some system for ensuring that investors get what they pay for, that entrepreneurs have duties to the investors who give them money, that people deal honestly, that investors get disclosure. And Coinbase, to be clear, has called for those things: It _wants_ regulation of crypto, because in the long run that is good for its business; it has [begged the SEC](https://www.sec.gov/files/rules/petitions/2022/petn4-789.pdf) to write new rules for crypto. And I [have sympathized with its view](https://www.bloomberg.com/opinion/articles/2022-09-13/crypto-wants-some-sec-rules) that some new rules would be nice.

But the SEC [rejected that request](https://www.sec.gov/news/statement/gensler-coinbase-petition-121523), saying, no, actually, the _existing_ rules apply to crypto, and are fine. But the crypto market mostly _doesn't_ want existing SEC regulations - the disclosure and anti-fraud rules that apply to stock - to apply to crypto, because they would be too restrictive. (That's why Coinbase is fighting the SEC in court, arguing that the SEC has no jurisdiction over crypto at all.) It would be good for crypto to have some rules to eliminate some frauds and make the market more trustworthy, but if you have too many rules and eliminate too many frauds … well, you might worry, what will be left?

When Coinbase itself went public in 2021, its chief executive officer, Brian Armstrong, wrote [a letter to investors](https://www.sec.gov/Archives/edgar/data/1679788/000162828021006850/coinbaseglobalinc424b.htm#ieaae362603cf40bfa0bef8a383bacd66_31). It was full of big claims:

> Coinbase is a company with an ambitious vision: to create more economic freedom for every person and business. Everyone deserves access to financial services that can help empower them to create a better life for themselves and their families, but today we are a long way from this vision. …
> 
> What started with Bitcoin has spawned an entire industry with countless different blockchains and tokens. We now have stablecoins, privacy coins, security tokens, reward tokens, governance tokens, and smart contracts. We're seeing the digitization of all types of value in a new economy that we call the cryptoeconomy.
> 
> Trading and speculation were the first major use cases to take off in cryptocurrency, just like people rushed to buy domain names in the early days of the internet. But we're now seeing cryptocurrency evolve into something much more important. People are using cryptocurrency to earn, spend, save, stake, borrow, lend, vote, and perform many other types of economic activity. Companies are being funded, getting early customers, and will eventually go public, all on the blockchain. The cryptoeconomy is just getting started. It is not intended to replace the traditional economy, but instead to be a complement to it, much like email was to paper mail. The cryptoeconomy offers a more global, free, and fair alternative to traditional economies that is native to the internet.

Now it's Beanie Babies.

## BOXX

For a while now people have emailed me occasionally about [BOXX](https://etfsite.alphaarchitect.com/boxx/), the Alpha Architect 1-3 Month Box ETF, which is, loosely speaking, a money-market exchange-traded fund whose holders get paid Treasury bill interest rates but _don't pay taxes_. I mean, that's what it looks like on the outside. On the inside it's a pile of stock options. "Isn't this cool," is how these emails often go. Or, "what is going on here?"

Today Bloomberg's Zachary Mider [has an article explaining BOXX's magic](https://www.bloomberg.com/news/articles/2024-02-22/this-exchange-traded-fund-mimics-t-bill-returns-without-tax-bills), and it is very fun, and very much  up my alley, and if you are reading this column it's probably very much up your alley as well:

> A year-old investment fund offers returns that closely track short-term Treasuries, with starkly lower tax bills. The fund, Alpha Architect 1-3 Month Box ETF, uses a complex options strategy and a longstanding tax loophole that favors exchange-traded funds.
> 
> "We spent seven years figuring out how to do this," said Wesley Gray, the ex-Marine and chief executive officer of Alpha Architect. "My job is just to deliver all the value I possibly can to my shareholders, within the law."
> 
> The fund, known by its ticker BOXX, surpassed $1 billion in assets this month. It is one of a number of efforts to use the ETF loophole in creative new ways, said Jeffrey Colon, a tax professor at Fordham University's School of Law in New York. He called BOXX "the poster child for tax arbitrage."

I can't _not_ write about the poster child for tax arbitrage, can I? 

The goal is pretty simple. You want something close to a Treasury money-market fund: You want a place to park your money that pays roughly the current short-term Treasury interest rate, that is roughly as safe as short-term Treasury bills, and that will give you your money back whenever you need it. You want it to be in the form of an exchange-traded fund, so you can buy and sell shares on the stock exchange. And you want the tax treatment to be better than Treasury bills. Specifically, you want the tax treatment that you'd typically get from a stock ETF: You don't want to pay taxes until you sell your shares, and when you do, you want to pay capital gains taxes.

So the first thing you want to do is turn interest income into capital gains. In the US, interest income - the interest you get paid on bonds or savings accounts or money market funds - is mostly taxed as ordinary income, at (federal) rates of [up to 37%](https://www.irs.gov/filing/federal-income-tax-rates-and-brackets). Long-term capital gains - your profits on selling assets that you've held for more than a year - are taxed at lower rates, [up to 20%](https://www.irs.gov/taxtopics/tc409). Turning interest income into capital gains is, therefore, good.

In some sense this should be _easy_. Interest is what you get paid for giving up the present use of your money. If you put your money in a savings account, the bank pays you interest every month for the use of your money. But if you buy, like, Nvidia Corp. stock, or Bitcoin, nobody pays you any interest. Instead, you expect the value of those things to go up over time, to compensate you for the use of your money. If you put $100 into Nvidia today and sell it for $150 in a year, part of that $50 is in some rough sense "interest," compensation to you for giving up the use of your money for that year. Most of it, though, is "risk premium," compensation to you for taking the risk that Nvidia might go _down_ instead. But there's no actual division; it's just $50 of capital gains.

But of course Nvidia really might go down instead. (Thus the risk premium.) So the job is to buy some asset that will appreciate, but only by the risk-free amount, and without risk: Instead of buying a stock that might go up 100% or down 50%, you want to buy an asset that will definitely go up exactly 5%. (I assume here that the short-term risk-free interest rate in the US is about 5%.)

Here is the simplest way you might imagine turning interest into capital gains. You give me $100 today, I promise to pay you back $105 in a year and a day, and I _don't_ pay you any interest along the way. "No interest income," you say to the Internal Revenue Service. And then in a year I give you back $105 and you say, well, I bought a bond for $100 and sold it for $105 after a year and a day, so I have $5 of long-term capital gains. 

This doesn't work, though. It's too obvious, and [the US tax code specifically says](https://www.law.cornell.edu/uscode/text/26/1272) that this sort of substitute for interest - called "original issue discount" - gets counted as interest income, not capital gains.

So you have to get away from debt. You can do this with stock, but stock doesn't have a guaranteed return. What you want is to (1) buy a stock today, (2) _hedge the risk of the stock price_ and (3) sell it in a year for 5% more than you paid for it.

This can be done! Classically it is called a "forward contract." You buy a share of stock today for $100. You agree to sell it to me, for a fixed price (the "strike price" or "forward price"), in a year. In a year, I give you the cash and you give me the stock.

How much should I pay you in a year? Well, I should pay you enough to compensate you for locking up your money for a year. If the risk-free interest rate is 5% and the stock doesn't pay a dividend, I should pay you $105. You put $100 into the stock today, I give you $105 in a year, you give me the stock. You have hedged out the stock-price risk - even if the stock goes up to $200 or down to $20, you're selling it for $105 in a year - so you don't need any compensation for risk. You just get paid a risk-free interest rate. But the transaction here is not "you put in $100 today and get back your money with $5 interest in a year"; it's "you buy stock today and sell it for a profit in a year." So, plausibly, capital gains. (Not tax or legal advice!) 

Stock forwards are not particularly usual contracts. But you can _build_ them. The way to build a stock forward is by buying a put option and selling a call option. So:

1. Today, you buy a share of stock for $100.
2. Today, you sell me a call option giving me the right (but not the obligation) to buy the stock from you for $105 in a year.
3. Today, you buy from me a put option giving you the right (but not the obligation) to sell me the stock for $105 in a year.
4. It is a convenient feature of financial markets - called "[put-call parity](https://en.wikipedia.org/wiki/Put%E2%80%93call_parity)" - that the price of the call option you sell equals the price of the put option you buy, making your net outlay in Steps 2 and 3 zero, or close to it. (The _reason_ for this is that the combination of the put and the call is equivalent to a forward contract, struck at the fair forward price, so the price of that forward - or the options that make it up - should be zero.)
5. In a year, if the stock is above $105, I exercise the call option and buy the stock from you for $105. If it's below $105, you exercise the put option and sell me the stock for $105. 
6. In any case, you put in $100 today ($100 for the stock, plus the price of the put, minus the offsetting price of the call) and get back $105 in a year. 
7. In other words, you got 5% interest on your $100.

Buying the stock makes you long the stock. Buying the put and selling the call make you "synthetically short" the stock: Owning a put and selling a call is economically equivalent to selling the stock forward. If you are long the stock and short the forward, then you have no stock price risk. You're just locking up your money in a risk-free trade for a year, and you get paid the risk-free interest rate.

Here's a variation that is more complicated visually but a bit simpler operationally:

1. You don't buy any stock.
2. You buy a put option and sell a call option, each with a strike price of $105. The net cost of these options is zero, just as it was above.
3. You sell a put option and buy a call option, each with a strike price of, say, $55. This gives you the right to buy the stock for $55 in a year, and it gives me the right to sell you the stock for $55 in a year.
4. The net cost of those options (the ones in Step 3) is, let's say, $47.60.
5. In a year, if the stock is above $105, then I exercise my $105 call option (and buy the stock from you at $105), and you exercise your call option (and buy the stock from me at $55), and the net result is that you get $50 (and no stock).
6. If the stock is below $55, then I exercise my put option (and sell you the stock at $55), and you exercise your put option (and sell me the stock at $105), and the net result is that you get $50 (and no stock).
7. If the stock is between $55 and $105, then you exercise your put option (and sell me the stock at $105) _and_ your call option (and buy the stock from me at $55), and the net result is that you get $50 (and no stock).
8. In any case, you paid $47.60 today (for the options in Step 3) and got back $50 in a year.
9. In other words, you got 5% interest on your $47.60.

The actual prices don't matter much; the point is that you have put in some money today in exchange for a fixed amount of money in the future, using options. You get synthetically short (in Step 2), just like in the previous example. But instead of getting long by buying the stock, you get synthetically long by buying the call and selling the put (in Step 3). You are long _and_ short the stock using options. This is neater because rather than buying stock _and_ options, you do everything in one place, in the options market. This is called a "box spread."

Does it turn interest income into capital gains? Sure, [more or less](https://www.morningstar.com/portfolios/tax-aware-alternative-cash). Not legal advice!  [Alpha Architect says](https://alphaarchitect.com/2023/05/box-spreads-an-alternative-to-treasury-bills/):

> The taxation of box spreads is complex; the tax rates (e.g., 25% or 40%) and tax character (e.g., income vs. capital gain) of options can differ from the taxation of treasury bills. The situation can get even more complex for index options, such as SPX, which are considered 1256 contracts, meaning 60% of their gains are taxed at long-term capital gains rates, and 40% are taxed at short-term capital gains rates. 

But let's just loosely say that, yes, this transmutes a thing called "interest" into capital gains on some equity derivatives. And in fact [derivatives traders](https://moontowermeta.com/boxx-access-options-funding-rates-in-an-etf/) think of box spreads as a way to lend money in the options market and get paid roughly the risk-free interest rate. And that's what BOXX does: It mostly buys box spreads on the S&P 500 index, earning Treasury-like interest through equity index derivatives. 

There is one other nice feature of box spreads using US listed options. I talked above about you trading options with me. But of course if you buy a put option from me today, and then in a year you exercise the option and demand that I pay you for the stock, there is some risk that I won't have the money. Trading US listed options solves this problem, because in listed options your counterparty is not me - some guy whose credit is risky - but rather the Options Clearing Corp., which backs all US listed options trades. The OCC is not actually an agency of the US government, and its credit is not exactly identical to that of US Treasury bills. But you might nonetheless feel pretty confident in its credit: It is a too-big-to-fail financial-markets utility with a strong credit rating and a lot of regulatory interest. "The OCC is a SIFMU, or systematically important financial market utility, which means the federal reserve will (most likely) get involved if something is amiss at the OCC," [Gray writes](https://alphaarchitect.com/2023/05/box-spreads-an-alternative-to-treasury-bills/) on Alpha Architect's blog. Lending money in the box spread market pays roughly Treasury-like interest, and has roughly Treasury-like credit risk. Which is what you wanted.

So far, so good, you have turned interest income into capital gains. But that only does so much. If you know that you want to lock up your money for 18 months and get paid the risk-free interest rate on it, then, yes, you can buy an 18-month box spread and (perhaps) turn your interest income into long-term capital gains. But that's not a great _product_. What you want in a product is something more flexible:

1. The product lasts forever and is constantly earning the short-term risk-free interest rate on whatever money it holds.
2. Anyone can put money in or take money out at any time.
3. They pay taxes only when they take their money out, and only on their gains (the difference between what they take out and what they put in).

For that you need some ETF technology. Mider writes:

> ETFs' tax advantage stems from their ability to avoid capital gains. That's the kind of taxable event that happens when you sell something for more than you paid. A 1969 law allows a certain type of investment fund to avoid those events if it hands appreciated securities, rather than cash, to an investor withdrawing from the fund - a transaction known as in-kind redemption. The tax break was rarely used until ETFs were invented two decades later.
> 
> Thanks to the tax treatment of in-kind redemptions, ETFs typically record no gains at all. That means the tax hit from winning stock bets is postponed until the investor sells the ETF, a perk holders of mutual funds, hedge funds and individual brokerage accounts don't typically enjoy.

We have [talked about this treatment](https://www.bloomberg.com/opinion/articles/2019-03-29/deals-on-the-train-are-everyone-s-business) in the past: US exchange-traded funds ordinarily do not buy or sell stocks. Instead, when you want to buy shares of (say) an S&P 500 index ETF, you buy the shares from an arbitrageur, who buys them from an "authorized participant," a big bank or trading firm, who then _creates_ them with the ETF: The authorized participant buys all the stocks in the underlying index and delivers them to the ETF in exchange for some new shares of the ETF. And when you want to sell, you sell to an arbitrageur, who sells to an authorized participant, who _redeems_ the shares from the ETF: The authorized participant hands the shares back to the ETF and gets back the basket of underlying stocks, which it then sells.

The key advantage of this is that those _in-kind redemptions_ - when the ETF takes back shares and gives out its underlying holdings - are not taxable events under US law. So a well-run stock index ETF might never have any taxable gains, which means that its holders never have any taxable income from holding the ETF. (Unlike a regular mutual fund, which will have gains whenever it sells appreciated stocks, and which will pass those gains on to its holders.) When the holders sell their ETF shares, that is a taxable transaction for them; if the ETF shares have gone up, then they pay capital gains taxes on their gains. But just _holding_ the ETF shouldn't generate taxes.

I suppose in theory BOXX could work something like that: It could never buy or sell box spreads, but instead have an authorized participant buy the box spreads and exchange them for new ETF shares. In practice, that seems more challenging to pull off with index options than it is with stocks, and BOXX does something different. Mider:

> Earning bond-like returns but recording them as capital gains from options bets, rather than interest, gives BOXX a chance to deploy the tax magic of ETFs. It does that by turning a single stock into a perpetual tax-loss-generating machine.
> 
> The stock that BOXX uses for this task is usually Booking Holdings Inc., the owner of reservation websites like Priceline, OpenTable and Booking.com. In addition to placing box spreads on the S&P 500, from time to time BOXX will also buy one on Booking shares. Booking's unusually high price, which hasn't dipped below $3,000 this year, makes it an attractive stock for these trades, Gray said.
> 
> Although Booking spreads typically represent less than 1% of BOXX's holdings, they play a key role in its tax planning. A box spread is akin to making two bets, one that a stock or index will go up, and one that it will go down. Since the bets are symmetrical, the overall value of the spread is unaffected by market movements. But the individual components are: If Booking rises, the long bet will gain in value, and the short one will lose.
> 
> Whenever BOXX wants to cancel out some capital gains, it uses an in-kind redemption to hand off the winning leg of the Booking trade to a market maker, Gray said. It keeps the losing leg on its own books, generating a tax loss. ...
> 
> A relatively small investment in Booking, combined with the ETF loophole, can easily generate large tax losses. Last May, BOXX bought a box spread on Booking for about $1 million. Three months later, the long side of the trade had gained more than $30 million and the short side had lost almost the same amount.
> 
> Then BOXX shed the winning part of the trade through an in-kind redemption and kept the losing part on its books. The fund's daily holding reports show that the maneuver positioned BOXX to book a tax loss of about $32 million, even though its overall bets on Booking made a few thousand dollars. That loss is more than all the actual returns the fund earned last year.

A box spread is a synthetic long position in a stock plus a synthetic short position in the stock. If the stock goes up, you make money on the long and lose money on the short; if it goes down, you lose money on the long and make money on the short. You sell the losing leg - generating a tax loss - and redeem the winning leg in-kind, avoiding a taxable gain. You do that with your weird little side trade in Booking, and you can generate enough tax losses to shield all of your actual (net) gains on your S&P 500 box spreads. And then you have a money-market fund whose interest is not taxable. Pretty good!

## Celsius

When I worked as a mergers-and-acquisitions lawyer and then as an investment banker, I thought that you could trade stocks in the US from 9:30 a.m. to 4 p.m. New York time, Monday through Friday. Was that completely accurate? No, of course not: There were, and still are, early morning and after-hours trading sessions, and I knew that. But it was close to true: There was, and still is, much more trading during normal market hours than in the extended sessions.

And it was a very _useful_ approximation of the truth. In particular, here are two stylized facts that are sort of true and that work very nicely together:

1. "The market is closed evenings, early mornings and weekends."
2. "Public companies have an obligation to keep their investors informed about material stuff that is going on."

For example: Public-company mergers and acquisitions tend to be intensively negotiated over the weekend, and are often announced on Monday mornings. Why? Well, because if a public company reaches an agreement to sell itself, that is an extremely material fact, and it should really announce that right away. You do not want people blithely buying and selling the stock at $35 when the company has already signed a merger agreement to sell itself for $50 per share. If you sign that deal at 11:46 a.m. on a Wednesday, first of all, every second that you spend drafting the press release is precious, and second, whenever that press release _does_ come out, it's going to be disruptive: The stock will spike up, people will make and lose fortunes, people who see the press release a millisecond before everyone else will have a huge advantage, and you will generally have disorderly and unpleasant trading. In fact, if you _do_ find yourself needing to announce a merger at 11:46 a.m. on a Wednesday, you will ordinarily ask the stock exchange to halt trading in the stock first, and reopen it only after the announcement has gone out and everyone has had a few minutes to read it.

But that is stressful and disruptive too, and it's much better to just get everything buttoned up on Sunday evening, get the press release ready to go, and put it out first thing Monday morning, well before the market opens. [[5]](imap://dave%40stucky%2Etech@mail.stucky.tech:993/fetch%3EUID%3E.INBOX%3E3854#footnote-5)  Give everyone plenty of nontrading time to digest and understand the news, so that when trading starts everyone is on a level playing field. Also, if for some reason there is a glitch in the system when you hit publish on the press release at 6 a.m., you have time to fix it: If it goes out at 6:20, that's fine too.

(To be clear, this stylized fact is good and useful from the abstract perspective of the public company, but it was very bad from my perspective as a young M&A lawyer. Terrible hours!)

Anyway, I mostly still think that

- "market hours" are 9:30 to 4, Monday through Friday,
- you are supposed to put out material news "outside of market hours," and
- it doesn't matter all _that_ much exactly when you do that, as long as you leave plenty of time before the market opens.

And I think a lot of other people still think that too, in part out of old habit, and in part because it is still sort of true, and in part because it remains very useful.

But there [has been some creep]([Robinhood Will Stay Open Late - Bloomberg](https://www.bloomberg.com/opinion/articles/2022-03-30/robinhood-will-stay-open-late)) toward always-on financial markets - we [talked last week](https://www.bloomberg.com/opinion/articles/2024-02-28/trading-stock-takes-time) about a proposed 23-hour-a-day stock exchange - and I worry that this stylized fact is no longer true. We [talked a few weeks ago](https://www.bloomberg.com/opinion/articles/2024-02-14/lyft-had-a-typo) about a typo in Lyft Inc.'s earnings release. Lyft put out the release right after the market closed on a Tuesday, there was a material typo, Lyft did an earnings call at 4:30 p.m., it verbally corrected the typo, and it filed a corrected earnings release at 5:51 p.m. Absolutely no harm, no foul, on the traditional way of thinking: All of this happened after hours, and by 9:30 the next morning everyone had had plenty of time to digest it. 

But in fact $700 million worth of Lyft stock traded in the after-hours extended session that Tuesday, roughly three times as much as Lyft usually trades in the _regular_ trading session. And there were news stories about it, and readers emailed me to be like "is this securities fraud," and Lyft's CEO had to [go on television](https://www.bloomberg.com/news/articles/2024-02-14/lyft-s-risher-says-my-bad-on-margin-error-it-was-one-zero) to say he was sorry. I forgive him! I wrote:

> It is customary to do these things after market hours for - well, not exactly for this reason, but kind of for this reason? You put out the press release just after the market's regular trading session closes at 4 p.m., and investors have 17.5 hours to think about it before the market opens again at 9:30 a.m. the next day. They can ponder the earnings release at their leisure, update their models, ask questions on the earnings call, and generally take their time to digest the new information and formulate a price view before the market opens and they have to trade on it. If there's anything ambiguous or surprising in the earnings release - or a typo! - the company and the investors have time to clarify it, and they can trade the next day with well informed views. …
> 
> Lyft can't stop its shareholders from trading after hours, but in some rough sense that's not its responsibility. If you want to trade in the after-hours market the second the press release hits the tape, the risk of typos is on you.

And then last week Celsius [did this](https://www.bloomberg.com/news/articles/2024-02-29/celsius-snafu-gave-a-sneak-peek-to-rally-fueling-earnings-report):

> Celsius Holdings Inc.'s quarterly results were sitting online, waiting to give anyone who looked a sneak peek at the earnings that would set off a 20% rally in the energy-drink company's stock price.
> 
> Not many people, it seems, knew they were there.
> 
> The company, which has a market value of about $19 billion, was scheduled to release its fourth-quarter and full-year results at 6 a.m. New York time on Thursday.
> 
> But they appeared on Celsius's website Wednesday night shortly after 7 p.m., with screenshots later circulating on X. The stock edged higher around that time, but on featherweight volumes. Trading picked up right at 6 a.m. Thursday, with shares falling more than 5% premarket before surging during the regular session by the most since August. They ended the day at an all-time high. …
> 
> It appears to be the latest blunder of what's been a fairly gaffe-heavy earnings season, with notable clerical errors in reports from Lyft Inc., Planet Fitness Inc., Mister Car Wash Inc. and Rivian Automotive Inc. ...
> 
> Of course, even if investors did see Celsius's report when it became available Wednesday night, they may not have been able to trade on it at the time and would've waited until Thursday's premarket session, said Kenneth Polcari, chief market strategist at Slatestone Wealth LLC.
> 
> "I think it's just sloppy," Polcari said of the early release. "But I don't think anyone was disadvantaged."

It's fine! This is how it's supposed to work! There are two sorts of time in the stock market:

1. From 9:30 a.m. to 4 p.m., people are trading and every millisecond counts.
2. From 4 p.m. to 9:30 a.m., and all weekend, time stops mattering: That whole stretch of 17.5 or 65.5 hours is effectively a single point, and there is no meaningful difference between 7 in the evening and 6 the next morning.

If you put your earnings up on your website at 7 p.m. and then put them out on a news wire at 6 a.m., that's fine! Those times are the same time! You did exactly what you are supposed to do; you got the information out there in the quiet time between when the market closed and when it opened again. Except the market was kind of open the whole time.

## Slerfed!

Here are some statistics from [Bloomberg's Olga Kharif](https://www.bloomberg.com/news/articles/2024-03-16/want-to-be-certified-crypto-expert-you-need-11-hours-and-229):

> To pass the chartered financial analyst exams and put the "CFA" letters on your résumé, at least 900 hours of study are recommended. Hitting the books for 300 to 400 hours is advised for the certified public accountant exam, which is usually taken by prospective CPAs who have completed an undergraduate degree in the subject.
> 
> However, to become a "Certified Cryptocurrency Expert," or CCE, all you need is $229 and time for 11 hours of online coursework offered by Blockchain Council. If that's too much of a time commitment, you can receive a "Cryptocurrency and Blockchain Certificate" elsewhere by taking just four hours of coursework, passing a 20-question test and shelling out $795.

Well. Sure. Look, I myself have spent at least [11 hours online](https://www.bloomberg.com/features/2022-the-crypto-story/) learning about crypto, and I do not want to be _too_ skeptical about crypto education. But these numbers strike me as reasonable. Of course the CFA program should be harder than the crypto program. One model that you could have for crypto is that it is _finance_ without the _content_.

So: A share of stock is an electronic token that you can buy or sell for money. Sometimes a lot of people want to buy a stock, and its price goes up. Other times, people want to sell it, and its price goes down. Why do they want to buy or sell it? Various reasons: Perhaps they got tax refunds or stimulus checks, perhaps the chief executive officer of the company that issued the stock did something interesting or got arrested, perhaps the company announced good earnings or bad earnings or a new product or a computer hack. But the _traditional_ reason is that a share of stock represents a partial ownership interest in a company, and the long-term value of the stock is the present value of its future cash flows. You can estimate that value by projecting those future cash flows and performing math to compute their present value. Different people will have different estimates, so there will be trades, and those estimates will change over time - with the company's prospects, with discount rates, with macroeconomic conditions - so there will be volatility. And if you want to make money trading stocks, traditionally, you go and learn about companies and products and business models and accounting and discounted cash flow modeling and all the other things that go into estimating the values of stocks, either because you want to get good at estimating values or because you want to know what _other_ people, the ones you are trading against, are up to.

A crypto token is also an electronic token that you can buy or sell for money, but in a purified form. There's no company, no product, no earnings, no cash flow. Sometimes a lot of people want to buy the token, and its price goes up; other times, they want to sell, and its price goes down. You have the most salient feature of finance - a volatile electronic token that you can trade - without any of the other features. There is less to learn!

Oh this is unfair and oversimplified, _your_ crypto project is different, _your_ crypto project is empowering communities with real products and not just an empty vessel for financial speculation. But Bloomberg's Muyao Shen [reported last week](https://www.bloomberg.com/news/articles/2024-03-13/memecoin-trading-volume-rises-to-levels-last-seen-before-crypto-bubble-burst):

> The memecoin frenzy in the digital-asset market shows no signs of stopping, with trading volumes now at levels last seen just before the burst of the last crypto bubble more than two years ago.
> 
> Considered as some of the most speculative and volatile cryptocurrencies, memecoins such as Dogwifhat and Pepe are far outstripping the gains registered by market bellwether Bitcoin that has dominated the headlines. Trading volume for the top memecoins, which often trade for a fraction of a cent, reached nearly $80 billion in the past week, according to data compiled by blockchain data firm Kaiko. That's the highest since October 2021. …
> 
> Memecoins have been a long-existing phenomenon in crypto, as small investors and promoters see the microscopic prices of memecoins as an opportunity to quick post huge returns despite the lack of traditional fundamentals. ...
> 
> A group of dogwifhat token holders announced last week a public fundraising campaign to put the dogwifhat meme on the Las Vegas Sphere. The group has already reached its target goal of $650,000 in the USDC stablecoin, based on the transaction history of the digital wallet for the fundraise. But it's unclear whether and when the fund will be used to promote the meme in Las Vegas.

What are dogwifhat's fundamentals? Well:

1. Its logo is a dog, with a hat.
2. If people kick in enough money, maybe they can put a picture of the dog with the hat on the Las Vegas Sphere, which might encourage more people to kick in more money.

What does the multiple-choice exam question about this look like? Or [today we got the story of Slerf](https://www.theblock.co/post/283025/solana-memecoin-slerf-burn):

> A new Solana-based memecoin, Slerf, has faced significant challenges after the project's developer accidentally burnt a major portion of the token supply - effectively losing $10 million, or the entirety, of presale participants' money.
> 
> "Guys I f-ed up," the project's official X account wrote. "I burned the LP and the tokens that were set aside for the airdrop. Mint authority is already revoked so I can not mint them. There is nothing I can do to fix this. I am so f-ing sorry."
> 
> The Slerf team later went to an X Spaces to elaborate further on the situation. "I'm sick to my stomach," team member Slorg said in a Space on X. "I'm literally about to throw up."
> 
> "I'm lost for words," they added. "I don't know what to do."

Poor Slorg. Basically the way crypto works is that a guy named Slorg [makes up a token named Slerf](https://www.slerf.wtf/#about), which is distinguished from other tokens by having a cartoon sloth logo. You send $10 million of Solana crypto tokens to Slorg, and he makes a note to himself that he owes you some Slerfs. Then he accidentally flushes that note down the toilet and, due to the irreversible nature of the blockchain, you get no Slerfs and your money is permanently gone, though Slorg is very sorry. 

If this were a _company_, and Slerf was a _stock_, this would all be _bad:_ It is bad for a company to lose all of the money it raises in a stock offering. (Also, though, it would probably be _reversible._ If a company just lost its list of shareholders, it could probably, like, go back through its emails and reconstruct the list.)

But Slerf is not a company or a stock: It is a crypto token, so absolutely nothing matters. Except that this is all sort of _funny_, and attention-grabbing, so of course Slerf went _up_. [Arnold](https://twitter.com/jdotarnold/status/1769698114603008382): "This mistake was very good for attention, and attention is the true value of any memecoin. So the obvious thing happened and the new tokens that were released shot up around 5,000%." You could spend another 10 hours and 55 minutes pondering this but I do not recommend it.
