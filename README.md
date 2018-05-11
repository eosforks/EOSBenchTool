# About


**EOSBenchTool** is a PC cross-platform, EOS pressure testing tool, which is developed by [OracleChain.io](https://oraclechain.io).

------------------------------

# Menu
* [Overview](#1)
* [Environment](#2)
* [Functions](#3)
* [bout OracleChain](#4)
* [Liecnse](#4)

------------------------------

<h2 id="1">Overview</h2>


The EOSBenchTool program is a benchmark testing tool build on EOSIO ecology. It provides a stress testing method based on account creation, transfer and other functions, to test the TPS of EOS node. 

EOSBenchTool client prepares a batch of transactions, then uses the pushTransactions to sends transactions to EOS node to save the client's packaging, signature time, use the limited client to maximize the pressure test on the server as far as possible!


------------------------------
<h2 id="2">ENVIRONMENT</h2>

**ENVIRONMENT：**

> MACOS、WINDOWS、UBUNTU

> [QT](https://www.qt.io/download) >= 5.8 just need to import and build the project with [QT](https://www.qt.io/download))

**依赖库/DEPENDENCYS:**

> our ECDSA is based on micro-ecc

> https://github.com/kmackay/micro-ecc

> We build a Publicly Verifiable Secret Sharing on secp256k1 which is published by Schoenmakers on crypto99 conference.

> https://github.com/songgeng87/PubliclyVerifiableSecretSharing


**Any questions pls join our official Telegram Group below**

> 中文群：https://t.me/OracleChainChatCN

> ENGLISH GROUP：https://t.me/OracleChainChat


<h2 id="3">Functions</h2>

### Settings
![](https://github.com/OracleChain/EOSBenchTool/blob/master/screenshots/setting.PNG)
>You should first set contract, create token, issue token, then you can use this tool to testing nodeos' performance.

>Thread number recommended to be your computer's kernel number minus 1.

>Contract account and Token name are which you created and set contract.

>Total tokens is NOT token numbers you just created, this recommended to be 10000, because it just send 0.00001 token per time during testing.

>Super account is the account hold enough tokens.

>Transaction pool size is the bottle size which all threads saving packed transactions. When the packed transactions size reach to pool size, this means it's ready to sending packed transactions.

>Transaction batch size is the array number of `push_transactions`.

### Test
![](https://github.com/OracleChain/EOSBenchTool/blob/master/screenshots/testing.png)
>After setting done, you switch page to testing, click `Prepare` button and wait to finish, and then click `Start` button to transfer packed transactions, when everything done, you should see testing result on the right of tool.

> Max tps means the max tps during testing duration.

>Average tps is just average tps during duration.

>ATTENTION: You should always reopen EOSBenchTool to restart a new testing.

------------------------------
<h2 id="4">About OracleChain</h2>


As the world’s first application built on an EOS ecosphere, OracleChain needs to meet the demands of the Oracle (oracle machine) ecosystem by efficiently linking blockchain technology services with various real-life scenarios, thereby delving into this immense tens of billions of dollars valuation market.


As a decentralized Oracle technology platform based on the EOS platform, the autonomous Proof-of-Reputation & Deposit mechanism is adopted and used as a fundamental service for other blockchain applications.In addition to Oracle services that provide real-world data to the blockchain, Oracle services that provide cross-chain data are also offered. Given that OracleChain can accomplish the functions of several prediction market applications, such as Augur and Gnosis, OracleChain can also support smart contract businesses that require high-frequency access to outside data in certain scenarios, such as Robo-Advisor.


OracleChain will nurture and serve those blockchain applications that change the real world. Our mission is to “Link Data, Link World,” with the aim of becoming the infrastructure linking the real world with the blockchain world.


By achieving intra-chain and extra-chain data connectivity, we aspire to create a service provisioning platform that can most efficiently gain access to extra-chain data in the future blockchain world.

<h2 id="5">LICENSE</h2>

**License**

Released under GNU/LGPL Version 3
