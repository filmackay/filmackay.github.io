---
layout: post
title: "ABC Radio National: Attack of the algorithms"
date: 2012-09-14
author: Fil
categories:
- blog
- hft
img: hft-chart.gif
thumb: hft-chart.gif
---
Last Sunday the [ABC](http://www.abc.net.au/) broadcast a reasonable review on HFT: [Attack of the algorithms](http://www.abc.net.au/radionational/programs/backgroundbriefing/2012-09-09/4242538). A little sensationalist and populist in broad assertions (we've got used to far worse!), but there was a *lot* of good content. However, what it lacks I think is the ability to communicate the magnitude of the problem. In other words: how much is predatory HFT "costing" other investors.

## What I liked

Some great points were made:

> And then you’ve got to ask yourself, ‘Well, who funds this?’ And at the end of the day, some of the high-frequency trading gains have got to be made from the more traditional participants in the market such as the superannuation funds.

Great point - not that we should automatically think that HFT is 100% 'drag' on the market. You should expect to pay something for liquidity, ie. for the ability to trade what you want when you want. I think we are paying for liquidity, which is fine; but in other cases we are also just paying - for no benefit in return.

> High-frequency trading, HFT, makes the public uncertain of the integrity of the Australian Securities Exchange. Professional stockbrokers such as myself have reduced confidence in the ASX as a result of observing HFT. If an operator manually entered HFT trade types, we would be penalised for manipulative trading. There should not be one rule for man and another for machines programmed by man.

Exactly! One major inconsistency has been the fact that humans seem to be able to be accused of things that machines can't. I remember discussing with the ASX some time back that central to the definition of market manipulation is: what is in the mind of the person placing the order? What if there is no person, and therefore no mind.. just an algorithm trained to look for profit generating feedback loops. There you have it - a technology driven pump-and-dump module!

Human traders now have a perfect excuse when getting a 'please explain' on some orders (perhaps too aggressive in posting/deleting orders): 'oh that's an algorithm'.

> Stan Correy: The most common criticism of high-frequency traders is that with state-of-the-art technology plugged into the stock exchange data centre they can manipulate the market; by getting information about share orders milliseconds before anyone else they can manipulate prices. In the market, it’s called front running.
> Paul Hilgers (Optiver): Front running means that I have an information before anyone else has an information. Front running means I have access to order flow other people don’t have. Well, I can only speak for my firm here—but I know a lot of my competitors—we don’t have any clients. We use our own money, our own capital, to trade and provide liquidity. So how can I front run order flow I don’t actually have? The information we use is available to everyone.

Exactly - doing things very fast is not front-running; go Paul!

I any case, I would not even categorise Optiver as an HFT. Depending your level of cynicism, they are either too slow (specialist HFT's are 10x faster), or too useful to the market to be HFT. Optiver are a market maker, and as such add valuable liquidity to the market as a whole. Optiver are more prey than predator in the speed game, as the sophistication of their models are too complex to be implemented in the super-fast [FPGA](http://en.wikipedia.org/wiki/Field-programmable_gate_array) technology employed at specialist houses.

It's a common misconception (to think Optiver is HFT), but it goes to heart of the issue: the mantle of HFT goes to the fastest in the market. Get consistently overtaken by others, and you are no longer HFT.

There is a way that algorithmic traders ('slow' and HFT alike) can, in Australia, carry out a sort of front-running in Australia. It is where algorithms specifically sniff-out those looking to execute large trades in the market, by identifying the patterns. I think this is what many people are really talking about, rather than the technical definition of front-running. This is obviously pretty grey, but my view would be that traders (usually other algorithms!) shouldn't be so predictable if they don't want to be read.

## Points of clarification?

> "Alan McGrath was watching high-frequency traders at work. Each transaction of 30,000 shares was a blink and you’ll miss it moment, generated by algorithmic computer programs, also known as robot traders."

These emerging items on FKP are orders, not transactions (trades). They were not arriving in rapid succession (a small batch once per second), and were easy for a human to comprehend and respond to. This example cannot be categorised as HFT - but instead a badly behaved (buggy) algorithmic trading program.

Remember: all HFT is algorithmic trading (usually really simple algos), but not all algorithmic trading is HFT.

> "The share market is a place where businesses are valued. It should be a place where people have confidence that the businesses are fairly valued, based on events—macro and micro. That’s all that should be affecting markets. It should not be affected by computer programs and mathematicians. When you turn on the stock market and make it a game, a casino, you are creating havoc."

Share markets are more than a place where businesses are valued - they are also a place where liquidity is valued. That is the price you pay for being able to trade at the time you want to. Remove computer software and mathematics from the market and you'll find it a very lonely place waiting for natural counter-parties to arrive. Whilst HFT may not always improve the process of valuing of businesses, it can help in improving liquidity. Just remember that HFT is like bacteria: it's not all bad. Overdose on antibiotics and you may regret it.

> Before Usain Bolt has even lifted his feet off the blocks, the trading algorithm has already bought and sold millions of shares, or flooded a market with false offers to buy and sell. Then they’re gone.

The orders that HFT (or algorithms) generate are never 'false'. They are just generated by people who can move very swiftly in the market, and probably withdraw the orders before anyone can execute against them. They are the equivalent of jockeying in football, where players shift their body to create an impression of movement, only to do something else. The movements are real, just like the orders.

Given that the market rules in the US (unlike Australia) allow cost-free creation and deletion of orders is it any surprise that, like with email, there is a lot of spam? These 'spam' orders are certainly a problem, but not because they are 'false'. They are a problem because everyone else in the market (actually, it's mainly directed at other HFT firms trying to keep up) must sift through this information to figure out what is really going on.

> In the US, on the New York stock exchange, about 70 per cent of all trading is high-frequency trading by these computers and algorithms and these are not going away.

This is a widely quoted statistic, as it on the face of it, quite shocking. While it is technically true, it is hiding what is really going on. The reason this number is so high, is not because the proportion of HFT is actually that big - but because almost all the non-HFT orders have been stripped away by the time it gets to the NYSE. It demonstrates NYSE's lack of non-HFT market share (or [[[blog:order-flow |toxic order-flow]]]), not the fact that the overall market is dominated to this degree by HFT.

> So their business model relies on using better computer technology, which is better predictive algorithms, faster line speeds, effectively trading in nanoseconds to take small amounts of profit on what is billions of dollars of trade. And then you’ve got to ask yourself, ‘Well, who funds this?’.

Great question, but nobody trades in nanoseconds. Sorry, it takes a nanosecond for light/electricity to travel about 30cm - and takes the Australian exchanges (who are very fast) about 100,000 nanoseconds just to match a trade.

> The impact of HFT, high-frequency trading, on Australian super funds is an emerging issue, with the potential to make our retirement savings more vulnerable.

HFT does not make your savings more vulnerable, it makes you more share trading more vulnerable. Whilst you could argue that concerns over HFT impact the perceived integrity of the asset class, it is really only going to be an issue when you buy and sell. Hopefully your superannuation is not being day traded, if so I hope you know what you're doing.

> Some of them are very good for the market and play an important economic role. They provide liquidity; they provide what we call price discovery, or price improvement.

A small point, but HFT certainly does not provide price improvement. Price improvement is where you give a trader a better price than he was expecting, or prepared to trade at. A successful HFT strategy is one that gets the trade before anyone else does, and giving the dubious benefit to the counter-party of executing his order 1 microsecond faster than your competitors (who all gave it a shot) - not paying any price improvement.

> But regulators are increasingly aware of the risks posed by these so-called [HFT] bad guys, which I’ll call parasitic traders. In the regulator community they call them ‘robots gone mad’.*

'Robots gone mad' is a good title to give to a buggy trading algorithm; but it's not necessarily anything to do with HFT. A dodgy algorithm doesn't have to be fast to cause damage.

'Parasitic traders' are HFT traders that use their speed to leech out profit by sitting in-between two counter-parties that would have otherwise traded together, and extracting a profit in the process. They don't add any value to the market (since the counter-parties would have traded anyway) but forced their way into the value chain.

Whilst I understand why you might associate parasitic traders and HFT, they are distinct from 'robots gone mad'. The idea that anyone such as a regulator could confuse these two is of concern.

> Now, we had a flash crash and a flash rise in a stock called David Jones in Australia on 30 June. And no one thought on that day to turn the stock off. It went up on speculation which was later denied, yet the stock market let it trade: money was made, money was lost. No one thought about turning that little stock’s market off—just one stock, not the market—no one thought about it.

What happened to David Jones is not new. Remember the AMP float in 1998? What happened was an sharp irrational rally (read: flash rise) and it was driven by humans. The price spiked up to $45 just after listing in a buying panic, only for the price to just as quickly crash and close the day at $23. Markets are sometimes chaotic beasts, with so many participants responding to the actions of other participants in tight feedback loops. We need to be careful to keep things in perspective and not blame algos/HFT for every market aberration. Prices can be unstable in times of uncertain supply/demand.

> Alan McGrath: "I don’t not what [colocating in ASX's Liquidity Centre] costs, but I’m sure it costs, you know, in the tens of thousands of dollars to have your server there. And I know there’s articles that they’re all on exactly the same length’s cables, so that one doesn’t get an advantage from the other. And, yeah, it’s a level playing field for those that want to spend the money to go that way, but certainly from a private trader that’s not an option.

It costs under $10k/month to have access to the top-tier price feeds in the ALC, and locate some of your own servers here. ASX has done a great job at providing genuine equal-access to this key infrastructure.

The question is: what would the private trader do with a price feed that was able to process prices a few milliseconds faster at the ALC, than the private trader does at their desk? The answer is of course: nothing. The reason the algorithms colocated in the ALC can respond to price action faster than the private trader is that they are computer programs that can act faster than humans. In fact the reason the algos move to the ALC is not to beat other private traders (they achieve that in any case), but it is simply to beat other algos that they compete with.

Put the private trader in the ALC, and it won't make any difference. However, give the private trader some algo tools to trade on their behalf, that are co-located in the ALC etc. and you might be onto something. But is it the HFT firms 'fault' that the private trader is not doing this? There is a need for the brokers to provide tools to private traders like Alan McGrath, allowing them to compete. Is this not a shortcoming of private traders and their brokers initiative?
