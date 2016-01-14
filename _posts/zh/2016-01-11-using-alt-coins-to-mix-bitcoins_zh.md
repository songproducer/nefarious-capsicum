---
layout: post
title: 用山寨币来混合比特币
comments: true
name: using-alt-coins
---

如果你在想为什么混合比特币是重要的，你可以读以下的文章：

[bitcoin.org/en/protect-your-privacy](https://bitcoin.org/zh_TW/protect-your-privacy)

如果你没太多时间，你只需要知道比特币和隐私是：

>任何人都可以看到任何地址里有多少钱和所有的交易纪录

你也许在想为什么当我可以直接用比特币来混合了却还需要用别种数字货币来混合比特币？

因为比特币的区块练较容易被解读分析，可用以下的工具： [Wallet Explorer](https://www.walletexplorer.com/), [Coinalytics](http://coinalytics.co/) and [ QuantaBytes](http://www.quantabytes.com/).

混合比特币也相当耗时，所以我想从多种混合的方式中选出两个可以让你的交易记录很私密又不会被追溯：达世币和玛诺币[Dash](https://www .dash.org/) & [Monero](https://getmonero.org/home).

- - -

####我的目标是用相对下较小金额0.02颗比特币（约小于十美元的价值）来做混合

- - -
**程序：**

1. 用比特币买山寨币
2. 用山寨币来混合
3. 卖出山寨币换回比特币



---

### 结果表

**XBT** = 比特币 Bitcoin
**XMR** = 玛诺币 Monero

| |*Monero玛诺币* |*Dash达世币* |
|-------------------------------------------|----- --------------------|----------------------------- -----------------|
|**同步区块练** |~ 2 – 24 小时|~ 1 – 2 小时 |
|**协议确认时间** |~ 1 分钟|~ 2 分钟 |
|**0.02 XBT 买进:** |18.2033312 XMR |2.91 DASH |
|**山寨币的价格** |0.0010987 XBT |0.00673189 XBT |
|**领出手续费(Poloniex)** |0.2 XMR |0.05 DASH |
|**领出后的币量** |18.0033312 |2.86 |
|**最小混合量** |无|1.49 DASH |
|**最大混合量** |如果用xmr.to 1个最多比特币|每个区间限制最多1000个达世币 |
|**需要多次区间** |不需要|需要，大量和当使用'Dark Sending'时 |
|**混合手续费** |0.105 XMR |无法查证 |
|**混合进区块练的时间** |9 分钟50 秒|未完成 |
|**买回比特币的价钱** |0.001063 |0.00696206 |
|**手续费的比例** |4.942 % | |
|**混合后比特币剩余量** |0.0191735 | |



- - -

##开始混合 （Dash）
因为山寨币价格波动大，所以混合的时间长短是一个卖出和买回比特币非常重要的考虑因素

---

##达世币

达世币的混合系统现在叫做*Dark Send*. 详细资讯[请读此文件](https://dashpay.atlassian.net/wiki/display/DOC/Introduction+To+Darksend).

简要的解释一下混合程序：点*'Start Darksend Mixing'*钮（这是一个混合前的步骤）。每**10**个区块*Master Nodes*会将欲混合的币拆成等量的金额，再将他人（或是水位提供者）已混合过等值的币传回给你。

然而，这整个程序有一个完成百分比，如果未达到百分百那么混合就会失败。

本来我打算只用0.01个比特币来实验，但是我发现至少需要1.49达世币才能混合（0.01比特币只够我换到1.43个达世币！）

在四小时五分钟过后我发现已经是早上六点，我应该去睡觉了。但是只完成了84%，我点了停止混合（Stop Darksend Mixing）钮。

＊我停止混合的原因是因为我想要测试准确的混合时间，在达到百分百时停止计时器*

隔天，我重启混合，点选'Start Darksend Mixing'钮。此时完成度为90%。等了七十分钟后，完成度仍然是90%。此时我已失去耐心，并做出因为干扰混合程序所以卡住的结论。

我的Darksend余额显示我有2.4个达世币，所以我试着传送那2.4个达世币然而我得到以下个错误讯息:
![errorMsgUnableToAnonymise](/images/unableToAnonymise.png)

无法找到适合此笔大小交易的Darksend。 Darksend要完全一样大小的金额来做，你可能需要混合更多的币。

我快速地看了一下[达世币的论坛](https://dashtalk.org/forums/darksend-questions-and-help.77/) 发现我不是唯一一个想要混合达世币却有困难的人。

我放弃尝试匿名的传送达世币因为我如果再试一次要再花五个小时加上抓出那些被卡住的币的原因。

因为我不知道如果我再测一次会不会需要另外五个小时来完成，所以我将那些完成90%的达世币传回交易所（所以那些币的匿名性被摧毁了）。

达世币的创造者正在改变'一点'Dark Send的方法，将必须用Master Nodes来混合的方式移除。 Dark Send现在的状态根本不能用。

也许我若没有干扰混合的程序可能就会成功。但是不能暂停对我来说是一个主要的bug。如果你用你的笔电在公共场合来混合，而你需要将电脑关起来几分钟呢？

然而，如果她真的成功了，等多余五个小时来混合少于十美元价值的比特币听起来一点都不像'未来不可追遡的数字现金'

##玛诺币（Monero）
玛诺币使用[环签章ring signatures](https://getmonero.org/knowledge-base/moneropedia/ringsignatures) 来即时混合和[隐身地址stealth addresses](https://getmonero.org/knowledge-base /moneropedia/stealthaddress).

>环签章是一组密码签章内含至少一个真正的参与者，但是你没办法得知在这群组内哪一个是真正做签章的人，因为他们都是有效的。

>隐身地址让接收者只须使用一个地址，即便其他交易者知道此地址也无法在区块练上查出这个地址的其他交易记录。

[Poloniex](https://poloniex.com) 不让你用他们的钱包混合玛诺币，所以我用了以下两个玛诺币钱包/交易所服务:

- - -
[![Mymonero](/images/mymonero.png)](https://mymonero.com) MyMonero 是一个​​让我有一定隐私等级的传送玛诺币钱包

- - -
[![xmr.to](/images/xmrto.png)](https://xmr.to) XMR.TO 是一个单向玛诺币换比特币的交易所，我用它来买回比特币

- - -

##结论
[玛诺币](https://getmonero.org/home) 很显然的是赢家，他没有最低限额，不麻烦而且非常快速的混合！

但要记住当你要混合时，不要在短时间内混合以防有心人士用[时间分析](https://bitcoinmagazine.com/articles/is-bitcoin-anonymous-a-complete-beginner-s- guide-1447875283)来分析区块练。
