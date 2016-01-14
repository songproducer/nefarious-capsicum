---
layout: post
title: 用山寨幣來混合比特幣
comments: true
name: using-alt-coins
---

如果你在想為什麼混合比特幣是重要的，你可以讀以下的文章：

[bitcoin.org/en/protect-your-privacy](https://bitcoin.org/zh_TW/protect-your-privacy)

如果你沒太多時間，你只需要知道比特幣和隱私是：

>任何人都可以看到任何地址裡有多少錢和所有的交易紀錄

你也許在想為什麼當我可以直接用比特幣來混合了卻還需要用別種數字貨幣來混合比特幣？

因為比特幣的區塊練較容易被解讀分析，可用以下的工具： [Wallet Explorer](https://www.walletexplorer.com/), [Coinalytics](http://coinalytics.co/) and [QuantaBytes](http://www.quantabytes.com/).

混合比特幣也相當耗時，所以我想從多種混合的方式中選出兩個可以讓你的交易記錄很私密又不會被追溯：達世幣和瑪諾幣 [Dash](https://www.dash.org/) & [Monero](https://getmonero.org/home).

- - -

####我的目標是用相對下較小金額0.02顆比特幣（約小於十美元的價值）來做混合

- - -
**程序：**

1. 用比特幣買山寨幣
2. 用山寨幣來混合
3. 賣出山寨幣換回比特幣



---

### 結果表

**XBT** = 比特幣 Bitcoin
**XMR** = 瑪諾幣 Monero

|                                           |*Monero瑪諾幣*            |*Dash達世幣*                                   |
|-------------------------------------------|-------------------------|----------------------------------------------|
|**同步區塊練**                              |~ 2 – 24 小時              |~ 1 – 2 小時                                  |
|**協議確認時間**                             |~ 1 分鐘                  |~ 2 分鐘                                      |
|**0.02 XBT 買進:**                        |18.2033312 XMR             |2.91 DASH                                    |
|**山寨幣的價格**                            |0.0010987 XBT            |0.00673189 XBT                                 |
|**領出手續費(Poloniex)**                   |0.2 XMR                  |0.05 DASH                                       |
|**領出後的幣量**                           |18.0033312                |2.86                                           |
|**最小混合量**                             |無                        |1.49 DASH                                      |
|**最大混合量**                               |如果用xmr.to 1個最多比特幣 |每個區間限制最多1000個達世幣                       |
|**需要多次區間**                              |不需要                   |需要，大量和當使用'Dark Sending'時                |
|**混合手續費**                                |0.105 XMR                |無法查證                                       |
|**混合進區塊練的時間**                          |9 分鐘 50 秒                |未完成                             |
|**買回比特幣的價錢**                          |0.001063                 |0.00696206                                    |
|**手續費的比例**                             |4.942 %                  |                                             |
|**混合後比特幣剩餘量**                        |0.0191735                |                                             |



- - -

##開始混合 （Dash）
因為山寨幣價格波動大，所以混合的時間長短是一個賣出和買回比特幣非常重要的考慮因素

---

##達世幣

達世幣的混合系統現在叫做 *Dark Send*. 詳細資訊 [請讀此文件](https://dashpay.atlassian.net/wiki/display/DOC/Introduction+To+Darksend).

簡要的解釋一下混合程序：點*'Start Darksend Mixing'*鈕（這是一個混合前的步驟）。每**10**個區塊*Master Nodes*會將欲混合的幣拆成等量的金額，再將他人（或是水位提供者）已混合過等值的幣傳回給你。

然而，這整個程序有一個完成百分比，如果未達到百分百那麼混合就會失敗。

本來我打算只用0.01個比特幣來實驗，但是我發現至少需要1.49達世幣才能混合（0.01比特幣只夠我換到1.43個達世幣！）

在四小時五分鐘過後我發現已經是早上六點，我應該去睡覺了。但是只完成了84%，我點了停止混合（Stop Darksend Mixing）鈕。

＊我停止混合的原因是因為我想要測試準確的混合時間，在達到百分百時停止計時器*

隔天，我重啟混合，點選'Start Darksend Mixing'鈕。此時完成度為90%。等了七十分鐘後，完成度仍然是90%。此時我已失去耐心，並做出因為干擾混合程序所以卡住的結論。

我的Darksend餘額顯示我有2.4個達世幣，所以我試著傳送那2.4個達世幣然而我得到以下個錯誤訊息:
![errorMsgUnableToAnonymise](/images/unableToAnonymise.png)

無法找到適合此筆大小交易的Darksend。Darksend要完全一樣大小的金額來做，你可能需要混合更多的幣。

我快速地看了一下[達世幣的論壇](https://dashtalk.org/forums/darksend-questions-and-help.77/) 發現我不是唯一一個想要混合達世幣卻有困難的人。

我放棄嘗試匿名的傳送達世幣因為我如果再試一次要再花五個小時加上抓出那些被卡住的幣的原因。

因為我不知道如果我再測一次會不會需要另外五個小時來完成，所以我將那些完成90%的達世幣傳回交易所（所以那些幣的匿名性被摧毀了）。

達世幣的創造者正在改變'一點'Dark Send的方法，將必須用Master Nodes來混合的方式移除。Dark Send現在的狀態根本不能用。

也許我若沒有干擾混合的程序可能就會成功。但是不能暫停對我來說是一個主要的bug。如果你用你的筆電在公共場合來混合，而你需要將電腦關起來幾分鐘呢？

然而，如果她真的成功了，等多餘五個小時來混合少於十美元價值的比特幣聽起來一點都不像‘未來不可追遡的數字現金’

##瑪諾幣（Monero）
瑪諾幣使用 [環簽章ring signatures](https://getmonero.org/knowledge-base/moneropedia/ringsignatures) 來即時混合和 [隱身地址stealth addresses](https://getmonero.org/knowledge-base/moneropedia/stealthaddress).

>環簽章是一組密碼簽章內含至少一個真正的參與者，但是你沒辦法得知在這群組內哪一個是真正做簽章的人，因為他們都是有效的。

>隱身地址讓接收者只須使用一個地址，即便其他交易者知道此地址也無法在區塊練上查出這個地址的其他交易記錄。

[Poloniex](https://poloniex.com) 不讓你用他們的錢包混合瑪諾幣，所以我用了以下兩個瑪諾幣錢包/交易所服務:

- - -
[![Mymonero](/images/mymonero.png)](https://mymonero.com) MyMonero 是一個讓我有一定隱私等級的傳送瑪諾幣錢包

- - -
[![xmr.to](/images/xmrto.png)](https://xmr.to) XMR.TO 是一個單向瑪諾幣換比特幣的交易所，我用它來買回比特幣

- - -

##結論
[瑪諾幣](https://getmonero.org/home) 很顯然的是贏家，他沒有最低限額，不麻煩而且非常快速的混合！

但要記住當你要混合時，不要在短時間內混合以防有心人士用 [時間分析](https://bitcoinmagazine.com/articles/is-bitcoin-anonymous-a-complete-beginner-s-guide-1447875283)來分析區塊練。
