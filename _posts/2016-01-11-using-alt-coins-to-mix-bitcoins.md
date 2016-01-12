---
layout: post
title: Using alt coins to mix bitcoins
comments: true
---

If you're wondering why mixing bitcoins is important you should read the following link:

[bitcoin.org/en/protect-your-privacy](https://bitcoin.org/en/protect-your-privacy)

For those who don't have time all you need to know about Bitcoin and Privacy is:

>Anyone can see the balance and all transactions of any address

You might be wondering, why use an alternative coin to mix bitcoins when you can just use bitcoins?

Because Bitcoin's blockchain can be more easily analysed with blockchain analysis tools like [Wallet Explorer](https://www.walletexplorer.com/), [Coinalytics](http://coinalytics.co/) and [QuantaBytes](http://www.quantabytes.com/).

Mixing bitcoins can also take a long time. So while there are many ways to mix bitcoins, I wanted to compare two alternative coins that are touted to make your transaction activity private and untraceable; [Dash](https://www.dash.org/) & [Monero](https://getmonero.org/home).

- - -

####My goal was to mix the relatively small sum of 0.02 bitcoins (just under $10 USD worth)

- - -
**The process:**

1. Buy the alt coin with Bitcoin
2. Use the alt coin's mixing function
3. Sell the alt coin back for Bitcoin



---

###Results table

*Note:* **XBT** = Bitcoin
**XMR** = Monero

|                                  |*Monero*                 |*Dash*                                        |
|----------------------------------|-------------------------|----------------------------------------------|
|**Sync blockchain**               |~ 2 – 24 hours           |~ 1 – 2 hours                                 |
|**Protocol confirmation time**    |~ 1 minute               |~ 2 minutes                                   |
|**0.02 XBT bought:**              |18.2033312 XMR           |2.91 DASH                                          |
|**Price of alternative coin**     |0.0010987 XBT            |0.00673189 DASH                               |
|**Withdrawal fee (Poloniex)**     |0.2 XMR                  |0.05 DASH                                     |
|**Coin amount after withdrawal**  |18.0033312               |2.86                                          |
|**Minimum mixing amount**         |None                     |1.49 DASH                                     |
|**Maximum mixing amount**         |1 bitcoin if using xmr.to|limited to 1000 DASH per session              |
|**Requires multiple sessions**    |No                       |Yes, for large amounts and when 'Dark Sending'|
|**Mixing transaction fees**       |0.105 XMR                |Unable to ascertain                           |
|**Mixing time including blocks**  |9 minutes 50 seconds     |Didn't complete                               |
|**Buy back XBT price**            |0.001063                 |0.00696206                                    |
|**Total fees as a percentage**    |4.942 %                  |                                              |
|**Total XBT after Mixing**        |0.0191735                |                                              |

*NB.* *'Total fees as a percentage'* may seem a bit off because I paid the mixing transaction fee from additional Monero funds.

- - -

##Time to mix
With alt coin prices being volatile, the time it takes to mix is a critical factor to consider when transferring out of and back into Bitcoin.

---

##Dash

Dash's mixing system is currently called *Dark Send*. For a detailed overview [read the documentation](https://dashpay.atlassian.net/wiki/display/DOC/Introduction+To+Darksend).

A quick description of the process is you press the *'Start Darksend Mixing'* button and this is like a premixing step. Every **10** blocks *Master Nodes* mix your coins and break them down into homogenous denominations, giving you back other people's (or liquidity providers) mixed coins of the same denominations.

The catch is though, the process has a percentage status bar and if it doesn't reach 100% then the mix is tainted with your original coins.

Initially I wanted to do this experiment with only 0.01 bitcoin, but as I found out the hard way - Dash has a minimum threshold requirement of 1.49 Dash (and my 0.01 bitcoin only got me 1.43!)

*I only counted one of the withdrawal fees in the Dash column*.

After 4 hours and 5 minutes of mixing with Dash I realised it was 6am and should probably get some sleep. It was at 84% and I clicked 'Stop Darksend Mixing'.

*The reason I stopped the mixing process is because I wanted to accurately time how long the mix took and be there to stop the timer when it reached 100%.*

The next day, I clicked 'Start Darksend Mixing' – at this stage the completion box showed 90%. After waiting another 70 minutes the completion box still showed 90%. I ran out of patience at this point and concluded the coins were stuck as a result of interrupting the mixing process.

My Darksend Balance showed that I had 2.4 Dash with some dust available to spend. So I try to Dark Send my 2.4, but got this error:
![errorMsgUnableToAnonymise](/images/unableToAnonymise.png)

A quick read of the [Dash support forum section on dark send](https://dashtalk.org/forums/darksend-questions-and-help.77/) shows I'm not alone with my struggle to mix Dash.

I gave up trying to anonymously send Dash because I thought Dark Sending again would take another 5 hours on top of the time for debugging the stuck coins issue. It turns out though, you only have to wait for the initial premixing to complete 100% once.

However, debugging the stuck coins issue not knowing whether or not I'd need to wait another 5 hours to 100% complete the premix was not an appealing prospect so I sent the coins back only 90% mixed to the exchange (thus destroying any anonymity those coins would have gained).

The creator of Dash is working on changing the way Dark Send works 'a bit' by removing the mixing role from the Master Nodes. Just as well because Dark Send in its current state didn't work at all.

Perhaps if I hadn't interrupted the mixing process, it may have worked. But the inability to pause a Dark Send seems like a pretty major bug to me. What if you were mixing coins at a public location on a laptop and you had to close the lid for a few minutes?

Still, even if it had worked, waiting ~ 5 hours to mix under $10 worth of bitcoins doesn't feel like the future of untraceable digital cash..

##Monero
Monero mixes instantly by using [ring signatures](https://getmonero.org/knowledge-base/moneropedia/ringsignatures) and [stealth addresses](https://getmonero.org/knowledge-base/moneropedia/stealthaddress).

>A ring signature is a group of cryptographic signatures with at least one real participant, but there is no way to tell which in the group is the real one as they all appear valid

>Stealth addresses let the recipient publish just one address, yet have all of his/her incoming payments go to unique addresses on the blockchain, where they cannot be linked back to either the recipient's published address or any other transactions' addresses

Poloniex doesn't let you mix Monero from their wallet, so I used two other Monero wallet/exchange services:

- - -
[![Mymonero](/images/mymonero.png)](https://mymonero.com) MyMonero is a wallet that let me send the coins with a configurable privacy level.

- - -
[![xmr.to](/images/xmrto.png)](https://xmr.to) XMR.TO is a one-way Monero to Bitcoin exchange which I used to buy back the bitcoins with the *moneroj* (term for Monero coins) I bought from [Poloniex](https://poloniex.com).

- - -

##Conclusion
[Monero](https://getmonero.org/home) is the clear winner with its no minimum, hassle free and ultra-fast mixing!

Keep in mind though that it's generally a good idea to wait some random amount of time when you mix to prevent attackers correlating your transactions with [timing analysis](https://bitcoinmagazine.com/articles/is-bitcoin-anonymous-a-complete-beginner-s-guide-1447875283).
