![[Pasted image 20260518003148.png]]



A blockchain is a distributed ledger 
![[Pasted image 20260518003224.png]]
Each node has its own copy of the blockchain
![[Pasted image 20260518003320.png]]
so when a new transaction is executed
![[Pasted image 20260518003525.png]]
then each node will update its copy 
![[Pasted image 20260518003601.png]]



Trustless Transaction means organizations no longer need intermediary such as banks to verify transactions. Immutable means that contents inside the blockchain cannot be changed/altered and any update needs the consensus of most of the network or all of them![[Pasted image 20260518003659.png]]
A Dishonest actor needs 51% control of the network to be successful![[Pasted image 20260518004449.png]]


![[Pasted image 20260518004626.png]]

Secure and immutable
![[Pasted image 20260518004729.png]]


The Blockchain Trilemma has three aspects and it only can satisfy two of the three elements:
![[Pasted image 20260518004808.png]]


Three main types of the blockchain (PPF):
![[Pasted image 20260518004943.png]]
The Public blockchain: Anyone can participate with no restrictions, most cryptocurrencies run on public blockchain governed by rules and consensus algorithms

The Private blockchain: Entity dictates who has access

Federated/consortium blockchain: where consensus are controlled by preselected set of nodes

Note: The public blockchain is the focus of this course (Blockchain Fundamentals Course by Cardano Academy)


Quiz question:
![[Pasted image 20260518005727.png]]
![[Pasted image 20260518005746.png]]



topic finished under the text is the separation line

---


# Distributed Ledger Technology (DLT)

A blockchain is a specific type of DLT![[Pasted image 20260518010150.png]]

A blockchain is a chronological secure data and it is append which means you only can add data as a part of a block
![[Pasted image 20260518010258.png]]
and each block contains a transaction lists, a reference of the previous metadata about the transactions
![[Pasted image 20260518010400.png]]


Hashing is taking an input of data
![[Pasted image 20260518010854.png]]
And output of fix sized string![[Pasted image 20260518010917.png]]

The inputs can be text, images, or videos
![[Pasted image 20260518010949.png]]
And the output hash will always be a set length
![[Pasted image 20260518011022.png]]

Each hash has its own unique identifier
![[Pasted image 20260518011124.png]]
Each time a new block is created its hash is produced based in the hash of the previous block
![[Pasted image 20260518011200.png]]


Blocks are connected through cryptographic hashes![[Pasted image 20260518011325.png]]
Every block hash is unique as the odds of finding two different pieces of data, which produce the identical hashes is practically impossible
![[Pasted image 20260518011421.png]]

Such a scenario where two separate inputs produce the same hash output is known as hash collision. This is why blockchain is a temper-proof where it can reduce hash collision
![[Pasted image 20260518011828.png]]


Blockchain relies on cryptography and game theory to function correctly
![[Pasted image 20260518012001.png]]
Game theory is about creating the right incentives that enough rational actors will behave honestly![[Pasted image 20260518012117.png]]
otherwise their stake will be at risk![[Pasted image 20260518012131.png]]



The public key can be generated from the private key but we cannot retrieve the process. That's why there is no risk of compromise when sharing the public key, it is like when someone shares his email publicly while keeping his login password privately
![[Pasted image 20260518012407.png]]

Private key holder can digitally sign a message with their private key
![[Pasted image 20260518012732.png]]
The receiver then can compare the public key with a signature, and rest assured the message is from who it's supposed to be from.![[Pasted image 20260518012838.png]]


Anyone who knows your private key can generate the signature to spend your Funds or reject a transaction or otherwise impersonate you. So it's critical this key remains private. The different options to protect your credentials are covered in later courses.![[Pasted image 20260518013113.png]]


Blockchains typically leverage a distributed peer-to-peer network for fault tolerance and transparency.
![[Pasted image 20260518013350.png]]
The goal is for each peer to have the same blockchain data. If not, a peer can reach out to another peer for an update. Some networks are configured slightly differently. For example, Cardona's network protocol only uses a pull communication method for security reasons. 
![[Pasted image 20260518013503.png]]
If a node tries to push information, it is automatically disconnected![[Pasted image 20260518013724.png]]
Peer-to-peer networking ensures that a network outage impacting some of the peers won't bring down everyone everywhere. The blockchain will continue to function and when the disruption is resolved, the impacted peers can reach out to other peers and get updated with the latest blockchain data.
![[Pasted image 20260518014123.png]]



A consensus mechanism is a protocol that brings all nodes of a distributed blockchain network into agreement (consensus) around a single dataset. You can think of them as the verification standards through which each, each block gets added to the blockchain.
![[Pasted image 20260518014241.png]]
There are various consensus mechanisms functioning on different blockchains today that can be configured for certain requirements with most having trade-offs around the blockchain trilemma.![[Pasted image 20260518014427.png]]



Proof of work and proof of stake are the two most common consensus mechanisms and the focus of this course. The Cardano Blockchain Certified Associate CBCA course goes into greater depth on alternative proof if you are interested![[Pasted image 20260518014529.png]]

The real USP of blockchain is that it guarantees integrity and trust in a distributed system, even when participants are untrustworthy. In doing so, blockchain solves an old computer science which we'll talk about next
![[Pasted image 20260518014715.png]]


Quiz question
![[Pasted image 20260518014912.png]]
![[Pasted image 20260518015057.png]]

topic finished under the text is the separation line

---

# **What is Byzantine Fault Tolerance?**

Banking and traditional payment systems are built on trusting a central entity.
![[Pasted image 20260518015200.png]]


Cryptocurrencies offer an alternative running on top of trustless blockchain technology. Just like any payment systems, users of a cryptocurrency network also need to agree on the current state of the blockchain. They must reach consensus, but achieving consensus in a distributed system securely and efficiently is not a trivial feat.
![[Pasted image 20260518015510.png]]



How can a distributed network of participants agree on a course of action if we know there are some bad actors behaving dishonestly?
![[Pasted image 20260518015634.png]]
This is the challenge posed by the thought experiment described in the 1982 paper known as the Byzantine General's Problem.![[Pasted image 20260518015651.png]]
The conundrum is about Byzantine generals attacking a walled city who face communication problems when trying to agree on their next move.![[Pasted image 20260518015806.png]]
Each general has his own army![[Pasted image 20260518020009.png]]
and each army is deployed in different locations surrounding the target city. ![[Pasted image 20260518020030.png]]
The generals need to decide together whether to attack or retreat.![[Pasted image 20260518020247.png]]
It is impossible to know in advance, which is the right option, but their chances will be much better if they reach consensus and move forward in a coordinated manner.
![[Pasted image 20260518020349.png]]
Note that each general must vote to attack or retreat. Votes are irreversible. All generals must agree to the same decision.
![[Pasted image 20260518020439.png]]
The generals can only communicate through messages, which may not make it to all other generals, could be misinterpreted or misspoken along the way.![[Pasted image 20260518020617.png]]
Assuming they reach the intended recipient, any of the other generals may still go rogue.![[Pasted image 20260518020650.png]]

If we apply the same dilemma to computer science, specifically blockchains, you can think of each general as a node or a peer on the network and the nodes need to achieve consensus on the current state of the system.![[Pasted image 20260518020846.png]]
The majority of the nodes in a distributed network agree and execute the same action in order to avoid catastrophic failure. This is where the property Byzantine Fault Tolerance comes from.![[Pasted image 20260518020923.png]]
If a system is described as Byzantine Fault Tolerant BFT, it is robust enough to achieve consensus in adverse conditions. It will continue functioning even if some of its nodes stop communicating or act maliciously.![[Pasted image 20260518021132.png]]

Different blockchains use various consensus algorithms to achieve Byzantine Fault Tolerance. The most common ones are Proof of Work, POW, and Proof of Stake, POS, but there are others too.
![[Pasted image 20260518014529.png]]

The primary difference between a consensus mechanism and a consensus algorithm is that the mechanism is the rules and incentives of the network, and the algorithm is the actual implementation of those rules.![[Pasted image 20260518021647.png]]

Quiz Question
![[Pasted image 20260518021749.png]]
![[Pasted image 20260518022123.png]]


The whole Chapter is finished under the text is the separation line for the new module

---
New chapter is down (Bitcoin & Ethereum)
# Bitcoin & Ethereum
We have seven topics
![[Pasted image 20260518022322.png]]
 Course Modules (Icons 1–7)
1. **What is Bitcoin?**
2. **How Does Bitcoin Work?**
3. **Scalability Case Study: The Lightning Network**
4. **What is Ethereum?**
5. **Proof of Stake**
6. **Hard Forks & Soft Forks**
7. **The 3 Generations of Blockchain**
## ## **What is Bitcoin?**
In the previous unit, we said Bitcoin was the first cryptocurrency. It wasn't the first attempt at digital money. In fact, it built on elements of previous efforts. Blockchain's origins and the birth of Bitcoin are summarized in this condensed timeline.![[Pasted image 20260518022712.png]]
1991, researchers Stuart Haber and W Scott Stornetta introduced a method to securely timestamp digital documents, chaining them together cryptographically to prevent tampering. This technology, though innovative, didn't gain traction and the patent expired in 2004.![[Pasted image 20260518023034.png]]
2004, Hal Finney won a veterans of the original Cipher Punk movement built upon earlier ideas with reusable proof of work, RPOW. This system tackles double spending, but relies on a central server for verification. RPOW serves as an important stepping stone for future cryptocurrencies.![[Pasted image 20260518023231.png]]
2008, amidst a global financial crisis, the Pseudonymous Satoshi Nakamoto released a revolutionary white paper Bitcoin, a peer-to-peer electronic cash system, inspired by an earlier project called Hash cash. Bitcoin introduces a decentralized solution for verifying transactions, eliminating the need for a central authority. this marked the true birth of blockchain technology.![[Pasted image 20260518023418.png]]



Many people will have heard of Bitcoin without knowing what blockchain is. The terms are often used interchangeably. To be clear, blockchain is the technology and Bitcoin is just one implementation of blockchain![[Pasted image 20260518023655.png]]





Bitcoin's big breakthrough was that it solved what's known as the double spend problem, where a bad actor might spend a cryptocurrency twice before the recipients is aware that only one of the transactions was valid.
![[Pasted image 20260518024235.png]]
The Bitcoin White paper proposes a solution to the double spending problem using a peer-to-peer distributed timestamp server to generate computational proof of the chronological order of transactions![[Pasted image 20260518024335.png]]
The cipher punk movement played a crucial role in shaping Bitcoin's early development and philosophy. Their values, technical expertise, and active participation laid the foundation![[Pasted image 20260518024501.png]]





Fiat money is issued and controlled by governments and central banks with seemingly endless supply. Most transactions are scrutinized and sometimes bank accounts are censored and even frozen. As most central banks are transitioning to completely digital systems. Freedoms and privacy are at risk of being sacrificed.![[Pasted image 20260518024748.png]]
While good old fashioned hard cash still allows for private and anonymous transacting, it is less and less accepted in everyday life. With many businesses now operating as card only.![[Pasted image 20260518024822.png]]





Bitcoin is the antithesis to such regimes. It is decentralized peer-to-peer censorship resistant, And not backed by any government or institution. Each Bitcoin transaction resides on a public ledger accessible by anyone with an internet connection. Bitcoin is a deflationary asset with a limited fixed supply of 21 million expected to be mined by 2,140. This mitigates inflation to some degree and ensures there is no uncertainty about its current and future supply.
![[Pasted image 20260518025114.png]]
The creation of new Bitcoins is determined by a protocol and a predefined set of rules. A process known as mining verifies and validates blockchain transactions as well as the creation of new Bitcoin in return for a reward.![[Pasted image 20260518025257.png]]
Furthermore, Bitcoin was released as open source code with anyone welcome to contribute and participate in its development. In contrast, traditional financial systems are typically written in proprietary code, privately controlled by authorities and central banks.![[Pasted image 20260518025405.png]]
On the 3rd of January, 2009, Satoshi Nakamoto mined the first Bitcoin block, which had a reward of 50 Bitcoins. Bitcoin's Genesis block contained a message that Satoshi Nakamoto added the times. Third January, 2009, chancellor on brink![[Pasted image 20260518025427.png]]
The first recipient of Bitcoin was Hal Finney, who received 10 Bitcoins from Satoshi Nakamoto in the first Bitcoin transaction on the 12th of January, 2009. Every 10 minutes since then, the Bitcoin supply increases as miners are rewarded by the system for validating transactions every four years ![[Pasted image 20260518025710.png]]
There is the famous Bitcoin halving which cuts the rewards in two and Bitcoin's inflation goes down. So in 2009, rewards started at 50 BTC halving subsequently to 25 BTC in 2012, 12.5 BTC in 2016, 6.25 Bitcoin in 2020 and became 3.125 Bitcoin on April 19th, 2024.![[Pasted image 20260518030031.png]]
You may be asking yourself, does anyone use Bitcoin for anything? How is it useful? An increasing pool of investors view Bitcoin as digital gold, a viable alternative investment to diversify their portfolio, especially in times of market volatility. The fees and transaction times of Bitcoin are negligible compared to the traditional financial system, which sometimes takes several business days for a money transfer. Bitcoin is especially appealing for international remittance where some services can charge extortion rates.![[Pasted image 20260518030212.png]]
Some notable transactions include the purchase of two pizzas on May 22nd, 2010 for 10,000, Bitcoin $40 equivalent at the time. May 22nd is celebrated each year as Bitcoin Pizza Day on April 10th, 2021, Bitcoin wallet belonging to the Bitfinex Crypto Exchange moved 161,500 BTC worth $1.1 billion at the time for a fee of approximately $0.68![[Pasted image 20260518030403.png]]
Bitcoin has its limitations. For example, transaction times can vary from 10 minutes to up to one day to times of increased network traffic. Critics argue Bitcoin is not as decentralized as Satoshi once envisioned. As the network is made up mostly of professional mining pools who are the only ones who can afford to pay for the required hardware and accompanying electricity bills. Bitcoin has attracted criticism in the past, notably with some of its senior developers leaving the project, citing concerns over centralization and lack of governance. Some feel a small core section of the Bitcoin community wields too much power over the currency's direction. While Bitcoin does have programmability, it has limited expressiveness by design. Bitcoin is resistant to drastic change, mainly due to security reasons. This can also be viewed as a reluctance or inability to innovate. For some, this is its great strength for others, it is its greatest weakness.![[Pasted image 20260518030614.png]]
Bitcoin has received criticism over its high energy consumption. The more computation required, the more miners must spend on hardware to realistically compete. For mining rewards, the barrier to entry rises and participation becomes more exclusive. Another drawback to consider is ever increasing storage requirements. As the size of the blockchain grows, sync times and transaction settlement times increase. Fewer machines in the distributed system are able to participate, which may result in the network being less![[Pasted image 20260518030921.png]]

Quiz question
![[Pasted image 20260518031022.png]]
![[Pasted image 20260518031047.png]]



topic finished under the text is the separation line

---

## ## **How Does Bitcoin Work?**
Let's dig a little deeper to understand how Bitcoin achieves Byzantine Fault Tolerance by allowing all network participants to validate blocks and transactions.![[Pasted image 20260518031315.png]]
As mentioned earlier, Bitcoin leverages proof of work as a consensus mechanism.![[Pasted image 20260518031342.png]]



The Bitcoin network relies on a mining process, which works as follows: in a vast distributed network of nodes, new transactions are sent out to all miners who collect these transactions and bundle them into potential blocks.
![[Pasted image 20260518031440.png]]
Each miner competes to solve a complex puzzle for their block, creating a unique identifier called a block hash. This process proves they invested effort, hence proof of work.![[Pasted image 20260518031519.png]]
The first minor to solve the puzzle shares their block with everyone else. If everyone agrees that the block is valid, it becomes part of the permanent record, the blockchain. This cycle repeats as miners create new blocks, each referencing the previous one, forming a secure cryptographically linked chain of blocks, hence the blockchain.![[Pasted image 20260518031601.png]]






Let's take a closer look at some of the key features on the Bitcoin protocol. A Bitcoin transaction is a transfer of value between users. The sender in the transaction is referencing the previous transaction received into their account, proving that they are allowed to spend the value they are sending. A transaction can have several different inputs to make up the value to be transferred. If the total output value is higher than the amount a sender wants to transfer, the Bitcoin protocol sends the difference back to the sender. A common analogy is cash in cash out.![[Pasted image 20260518031710.png]]
If you buy a book that costs eight coins and you send 10 coins, you get two coins back. As change. The value of the input(s) in a transaction must always match the value of the output(s). In other words, sum of inputs equals sum of outputs minus transaction fee.![[Pasted image 20260518031829.png]]



Proof of work, PoW, is based on mining nodes competing to guess. A pseudorandom number known as a nonce (number used once).![[Pasted image 20260518031910.png]]
The maths problem is solved, by combining this number with block data and passing it through a hash function until you get the desired output, which matches certain criteria. For example, a hash starting with nine zeros.![[Pasted image 20260518031943.png]]
This desired output can be tweaked with what's called a difficulty level. So if there are more miners with advanced mining equipment competing for the next block, the desired output hash might now have 12 leading zeros. The goal is to have a block mind every 10 minutes, whichever minor guesses, this nonce first is rewarded with a set amount of Bitcoin. These maths puzzles are said to be difficult to solve but easy to verify.![[Pasted image 20260518032034.png]]
When a minor solves the puzzle, they then share the block with the network. All the other miners then verify that the solution is legitimate. This is the concept of inclusive accountability in that everyone can check each other's homework.![[Pasted image 20260518032112.png]]
The miner can then add the block to their copy of the blockchain and the transaction is considered complete. The miner also includes in the block the output hash from the previous block, so all blocks are chained together. Each miner has a copy of the blockchain on their computer. Everyone trusts the blockchain, which has the most computational work gone into it. This is where the term longest blockchain comes from.![[Pasted image 20260518032145.png]]
Each valid block contains a block hash representing the work done by the miner, hence the name, Proof of Work. Trust in blockchain is derived from the fact that even a small change in the input hash will change (Invalidate) the output hash.![[Pasted image 20260518032237.png]]
Proof of Work has been resilient to all manner of different attacks since 2009. Generally, a successful attack would involve a malicious attacker acquiring 51% of the network's mining power. This would require so much time and computational power that it would not be viable as the cost incurred would be greater than any potential rewards for attacking the network.![[Pasted image 20260518032324.png]]





A miner's chances of finding the desired hash and solving the puzzle is equal to their mining power relative to their competitors.![[Pasted image 20260518032402.png]]
A mining pool is when smaller miners pool their resources, so together they have a better chance of mining the next block. They then split any Bitcoin Mining Rewards in relation to how much processing power each![[Pasted image 20260518032432.png]]


Quiz question
![[Pasted image 20260518032501.png]]
Correct Answer: **The ‘difficulty level’**


topic finished under the text is the separation line

---


## **Scalability Case Study: The Lightning Network**
The Lightning Network is a 'Layer 2' payment protocol that functions on top of a 'Layer 1' blockchain, in this case, Bitcoin.![[Pasted image 20260518033025.png]]
Joseph Poon and Thaddeus Dryja published the Lightning Network White Paper in February, 2015![[Pasted image 20260518033045.png]]



As Bitcoin can only process seven transactions per second today, the paper proposes a solution to this scalability challenge by executing transactions away from the main chain, or 'off chain'. The Lightning Network leverages user-generated bi-directional payment channels to enable almost instantaneous transactions with smaller transaction fees.![[Pasted image 20260518033125.png]]




So how does Lightning Network work? A payment channel is created with an on chain transaction. Then the channel facilitates unlimited off chain transactions without requiring consensus on chain. This means transactions can be executed much faster for lower fees. When opening a payment channel, two parties set up a multi-signature wallet and add some funds to it. You can think of it like a safe, where funds are traded back and forth, but only accessible when both parties confirm their private keys. Each party signs and updates their records after each transaction. When they finish doing business, the payment channel is closed and the latest updated balance is shared with the entire Bitcoin network. In case of disagreement, either party can revert to their updated records and recover their funds.
![[Pasted image 20260518033208.png]]
![[Pasted image 20260518033215.png]]



You may be wondering how does a single payment channel between two parties solve Bitcoin's scalability problem? This was just a simplification as these single payment channels are the building blocks for a vast network. Even if Bob doesn't have a direct payment channel with Alice, he can find an interconnected payment route via other channels. For example, if Alice wants to pay Bob but doesn't have a direct channel, she can leverage Fred's channel, who is a mutual friend. The smart contract will automatically find the shortest route, even if it must traverse several payment channels. Otherwise, it wouldn't live up to its name as the Lightning Network. The Lightning Network does have some drawbacks. For example, the receiving party needs to be online for a transaction to go through. Opening and closing a payment channel still requires an on chain transaction. We'll see later in the course how Cardano addresses some of these issues with a similar solution.
![[Pasted image 20260518033352.png]]



Quiz question:
![[Pasted image 20260518033444.png]]
![[Pasted image 20260518033504.png]]
Correct Answer: **The Lightning Network**








topic finished under the text is the separation line

---


## **What is Ethereum?**
"Vitalik Buterin, a developer and one of the co-founders of Bitcoin magazine wrote the Ethereum White paper in 2013. He had initially made the case for a scripting language

for Bitcoin that would enable developers to design decentralized applications or dApps as they're commonly referred to. In what was an early test of governance,

there was a failure to reach any agreement amongst the community. This led Buterin to begin development of a new blockchain called Ethereum

that would bring programmability into the space. The white paper describes an open source public permissionless, blockchain-based, distributed computing platform

that could run smart contracts. What are smart contracts? Originally, the brainchild of lawyer and computer scientist, Nick Szabo in the 1990s,

a smart contract is a self-executing program that runs on a blockchain once predetermined conditions are satisfied. Ethereum launched in 2015

and smart contracts soon gained broad adoption in the blockchain world. The most common use of smart contracts is to execute a transaction only if certain conditions are met.

Smart contracts are written in high-level programming language's code, and compiled into bytecode, which you can think of translating code into simpler code

a computer can better understand. A decentralized Turing complete virtual machine. The Ethereum virtual machine EVM then reads and runs these smart contracts using a global network

of public nodes. This is where the term world computer stems from. As an immutable, transparent blockchain running on a

resilient network ensures censorship resistance. Smart contracts on Ethereum are written using the solidity programming language. It is built specifically for Ethereum

and similar to JavaScript, offering a smooth learning curve for developers new to blockchain. On the downside, some experts believe solidity is too expressive,

whereby it is too easy for unintended side effects to creep into a dApp's code. One common bug, for example, is incorrect access control.

This is where smart contracts do not have sufficient access controls in place for code that executes critical logic. Smart contracts enable a broad spectrum of use cases,

which we'll cover later. For now, just know that developers could now create and publish dApps running on the Ethereum blockchain.

Ether (ETH) is the cryptocurrency for Ethereum. When you execute a transaction, you need to pay fees in ether known as 'gas'.

The more computation required, the more you pay. Crucially, the same transaction can cost different amounts of gas at different times, depending on network demand,

your transaction will be prioritized on how much gas you are willing to pay. We'll see later how Cardano attempts to address these issues.

Ethereum also led the way in the rise of NFTs. An NFT or non fungible token is a type of cryptographic token that represents a unique asset.

Think of them as tokenized certificates representing authenticity and ownership using a blockchain. Non fungible means tokens are not interchangeable,

and this feature introduces digital scarcity, which opens up Pandora's box of use cases we'll cover later. Fungible tokens also have their place. Fiat currencies,

and most cryptocurrencies like Bitcoin, ether, and ADA on Cardano are fungible. Fungible means assets are interchangeable and practically indistinguishable from each other in

everyday use as a medium of exchange. If you want to create an NFT on Ethereum, you must abide by the ERC or 'Ethereum

Request For Comment' standards. ERC is basically a collection of guidelines for doing different things on its blockchain. While the ERC 20 standard allows users to create

or mint indistinguishable tokens, the ERC 7 21 standard catered for the issuance and trading of non fungible assets. This standard was subsequently enhanced again with ERC 1155,

which enabled a single contract to contain both fungible and non fungible tokens, widening the scope again for new use cases.

We'll see later how Cardano innovated in the NFT"



quiz question:
![[Pasted image 20260518033625.png]]
![[Pasted image 20260518033632.png]]
Correct Answer: **Smart contracts**



topic finished under the text is the separation line

---

## **Proof of Stake**
Inevitably alternative consensus mechanisms began to emerge, exploring ways to address shortcomings with proof of work. One such alternative was the proof

of state consensus algorithm, which was first minted on the Bitcoin talk forum in 2011. Although both achieve consensus on blockchain, the means

by which they get there is quite different. There are also different implementations of proof of stake. More about that later. How does proof of stake (PoS) work?

Proof of stake algorithms use a random election method to select a node that will be the validator of the next block.

Who is chosen is based on a combination of criteria that can vary by blockchain, but generally include staking duration, amount of stake,

randomization, and node strength. A validator is a generic term, but think of it as the entity responsible for validating the next block on the chain. On Bitcoin,

this is the minor or mining pool. On Ethereum, it is the stake pool. That is the validator. Also, note that with proof of stake, blocks are said

to be 'forged', not mined. The proof of stake system usually uses transaction fees as a reward, although additional incentives can be offered.

Users participating in the 'forging' process must commit a set amount of coins in the network. This process is more commonly referred to as staking,

and these coins represent their stake. Stake size determines the chances of a node being selected as the validator to forge the next block -

the bigger the stake, the greater the chances. A little like a lottery, the more tickets you have, the greater your chances of holding the winning ticket.

Different methods are used to ensure a random selection process, such as the 'Randomized Block Selection' and 'Coin Age Selection'.

With random block selection, validators are chosen based on nodes having a combination of lowest hash value along with highest stake. Whereas

with coin age selection, nodes are selected based on how long their tokens have been held. This is calculated by multiplying the number

of days the coins are held by the number of coins. Once a node has forged a block, the age

of its coins is reset to zero and the node must wait a set period of time before it is eligible to forge another block.

This prevents a user with a large amount of coins (stake) from having too much control. Each blockchain implements proof of stake differently

with its own custom rules and configuration. For example, Algorand and Cardano rely on the Verifiable Random Function, one of crypto's most important discoveries dating back to 1999.

When you stake ETH, you are essentially supporting a validator for the network. Randomly selected validators who hold a minimum amount

of ETH are responsible for verifying transactions and adding new blocks to the blockchain. Validators, and their stakers, earn rewards through freshly minted e

and network transaction fees. The stake serves as financial incentive for the forging node to behave honestly as they have 'something at stake'.

If a forging node acts fraudulently, they may lose part or all of their stake, and also the right to participate as a forger

in future. A 51% attack works similar to what we described with proof of work, except, this time, a bad actor would require a majority stake

(51%) on the network. This is highly unlikely unless the value of the cryptocurrency is very low. The pros for proof of stake are energy

efficiency and security. It is more inclusive as usually running a node is easy and affordable. High participation, along with the randomization process,

makes the network more decentralized. As mining pools are no longer needed to mine blocks. It's important to note all proof

of stake blockchains are not created equally. For example, some things to consider before staking on Ethereum: In September, 2022,

the Ethereum 'Merge' transitioned the blockchain from proof of work to proof of stake. This is only a step on a long Ethereum 2.0 roadmap.

You require a deposit of 32 ETH to run a staking node on Ethereum. There is a lockup (bonding) period

where your funds are not accessible. Ethereum employs 'slashing', which is a penalty designed to deter dishonest validator behavior. Slashing may result in the loss of a validator staked ETH,

and even removal from the network. Delegated proof of stake (DPoS) is a consensus algorithm which extends the proof of stake idea.

It was developed originally by Daniel Larimer in 2014. Holders of coins delegate to a validator, a little like voting for your chosen politician.

You are effectively delegating staking responsibility to the validator. This is considered more efficient as many users will not have technical ability

or time to run a validator. It is also democratic as the barrier to entry is low and can be a one-time delegation.

Otherwise, a lot of the functionality is similar to proof of stake. We'll talk more about Cardano being the first provably secure

proof of stake protocol years before Ethereum

Quiz question:
![[Pasted image 20260518034131.png]]
Correct Answer: **A random election method**



topic finished under the text is the separation line

---


## **Hard Forks & Soft Forks**
You may ask yourself, if there is no central authority and nobody is in charge, then how can a blockchain be updated?

In a truly decentralized network, changes are implemented with soft forks or hard forks. It is slightly more nuanced than that,

as some chains implement these forks very differently. Any software needs regular updates to fix issues, boost performance, and protect itself from new attack types.

Anyone who uses Windows can't escape the regular updates on Patch Tuesday. The colloquial term for Microsoft's update Tuesday that pops up on the second Tuesday of every month.

In the world of blockchain, there are similar updates called forks. Since blockchains are decentralized networks, it works best when all participating nodes follow the same

rules and run the same version of the node. These rules are known as the protocol and a fork can change a protocols behavior

by different extents. There are two main types of fork in blockchain, soft and hard forks. Soft forks are backwards compatible upgrades.

They're soft in that they don't necessarily interrupt the regular functioning of the network. Think of it like an optional update on your laptop.

A hard fork is a more drastic change to a protocol. Generally, nodes that don't update to the new version will be unable to process transactions

or add new blocks to the blockchain. Hard forks are used to implement a major update to an existing protocol,

or as the name suggests, fork a blockchain in two. The old one continues functioning as before. While a new blockchain is also created

with different sometimes contentious features. A good example was the Ethereum Hard Fork, which occurred after a decentralized autonomous organization known

as a DAO was hacked due to a solidity vulnerability and approximately 3.6 million ETH was stolen. It caused a split in the Ethereum community

as there was no consensus or governance mechanism to decide on how to proceed. Eventually, Ethereum chose to reverse the hack

and refund the ETH. Ethereum classic adopted a 'code is law' stance and believed those who lost their ETH should take their medicine.

This eventually led to a contentious hard fork giving birth to two separate Ethereum chains, Ethereum and 'Ethereum Classic'. Hard forks are not

just technical events. There can be various intangibles which motivate communities. Ideally, they are planned and unanimous, but in some contexts they can be sudden

controversial and traumatic. Another example was the Bitcoin fork, where the scaling conundrum led to heated debates, which resulted in the creation of Bitcoin cash, a fork

of the original Bitcoin protocol with an increase in maximum block size to 32 megabytes. Over the years, Bitcoin has been forked over a hundred

Quiz question:
![[Pasted image 20260518034458.png]]
Correct Answer: **Hard Fork**



topic finished under the text is the separation line

---


## **The 3 Generations of Blockchain**
Now that we've covered Bitcoin and Ethereum, it is a good time to explain the three generations of blockchain. Since Satoshi's White paper in 2009,

blockchain technology has evolved over three distinct generations, each evolving with new features and innovative capabilities. Bitcoin ushered in the first generation

of blockchain using proof of work to validate transactions. Miners require by design ever increasing amounts of computing power to compete to generate new blocks.

Bitcoin is energy intensive, but also incredibly secure. It has been notoriously reluctant to implement new features for fear it will increase the attack surface

and lead to a less secure network. The second generation of blockchain was spearheaded by Ethereum. It introduced programmability to blockchains

through smart contracts written in solidity. Suddenly, blockchain was not just about moving currencies back and forth. Smart contracts led to a proliferation

of dApps facilitating a broad range of new use cases we'll discuss shortly. Ethereum started as a proof of work consensus

and transitioned to proof of stake in September, 2022. So-called third generation Blockchains extend on past projects with a new breed

of blockchains such as Cardano, Polkadot, and Algorand. This generation placed more emphasis on scalability, interoperability, and governance. Cardano was the first proof of stake blockchain

to offer the same security guarantees as Bitcoin. It has followed a research driven approach to building its blockchain with many novel features and solutions.

This leads us nicely to our next few videos, which will explore Cardano's differentiators in more detail.

Quiz question:
![[Pasted image 20260518034711.png]]
Correct Answer: **3rd generation**


The whole Chapter is finished under the text is the separation line for the new module

---
New chapter is down (Introduction to Cardano)
# Introduction to Cardano
The 6 topics for this chapter **Introduction to Cardano** are:
1. **Origins of Cardano**
2. **Cardano Development Milestones**
3. **What is Ouroboros?**
4. **Staking on Cardano**
5. **What is Cardano’s eUTXO Model?**
6. **Smart Contracts on Cardano**

##  **Origins of Cardano**
"There are three Cardano 'genesis' entities that have traditionally propped up Cardano. In 2015, Charles Hoskinson and Jeremy Wood, co-founded Input Output Global (IOG),

formerly Input Output Hong Kong. IOG is the development and science arm for Cardano. Since 2015, IOG has been focused on protocol development

and academic research. It has more recently pivoted to a venture studio business model with spinoff companies such as Lace light Wallet, RealFi,

and the Midnight Partner Chain among other critical infrastructure projects. Built on a foundation of academic peer reviewed research, it has maintained a 100% uptime since.

The Cardano Foundation (CF), based in Zug, Switzerland was set up as the legal custodian for the Cardano brand and as a contributor to the governance of Cardano.

The Cardano Foundation's statutory purpose is to generally support the adoption and the advancement of Cardano as a public digital infrastructure.

Its core activities revolve around providing utilities to the ecosystem, developing enterprise infrastructure, tooling, strengthening operational resilience and regulatory clarity,

and driving education through different initiatives. Part of these efforts is the facilitation of interactions with various stakeholders, including not only players from the immediate ecosystem,

but also international stakeholders such as standard setters, lawmakers, or regulatory bodies. Emurgo, with a focus on Asia and Africa, is the commercialization arm of Cardano.

Emurgo concentrates on FinTech infrastructure, developing the Yoroi wallet, ecosystem growth, smart contract audits, and a social network called Cardano Spot.

The ecosystem has grown and there are now dozens of companies and hundreds of projects building on Cardano. There are too many to mention here,

but visit the showcase section of the Cardano developer portal for more details. From the outset, Cardano's mission was to improve upon previous generations

and build for the long term. While Ethereum favors more heuristic arguments as it's trying to do more faster as Vitalik Buterin explained,

Cardano adopted a first principles peer reviewed academic research approach. This involves employing rigorous processes with formal methods, mathematical specs,

and proofs to deliver high assurance software, Cardano is built on solid foundations with over 200 research papers published and scrutinized at the top cryptography conferences.

One of Cardano's key tenets is an open source patent free philosophy where research papers, formal specifications and code repositories

are available to all. Anyone with the appropriate technical skills can review the claims and findings from this academic approach.

Other projects have borrowed heavily from IOG's research in their protocol design. Unlike many projects which are mere forks of existing blockchains, much

of Cadrano is custom built using a first principles approach. Cardano identified key areas as essential for mass adoption scalability.

While Bitcoin and Ethereum were landmark technical achievements, both have shortcomings. Bitcoin can handle just seven transactions per second. While Ethereum has had issues handling demand

where at a certain capacity system bloat sets in performance becomes unpredictable and transaction fees spike intermittently. The same transaction can incur different gas fees at times,

depending on network demand. Cardano seeks to address these shortcomings and mirror protocols like BitTorrent, where performance scales as new users join.

Interoperability. Most mobile devices only function because of layers of interoperability standards. At a high level, the telecoms industry relies on the global

system for mobile communications, for mobiles to talk to each other across different networks and jurisdictions. The wifi standard ensures connectivity and faster speeds.

TCP/IP is a suite of protocols that enables computers to communicate on the internet. Similarly, the future of blockchain is multi chain

and many dApps and tokens now operate cross chain. Cardano has multiple solutions that are making their way from research papers

to full implementation. Governance, sometimes referred to as sustainability. Bitcoin and Ethereum have both encountered problems as they try to scale.

They have no decision making mechanisms to manage change. When a blockchain grows to millions of users, it's not viable or healthy for a small 'one pizza' core team

to be dictating outcomes. Worse, still, it can lead to traumatic splits. For example, Bitcoin had the big blocks versus SegWit

debate, which eventually led to a hard fork resulting in two chains, Bitcoin Cash and Bitcoin. Governance is not a sexy topic

for many, but arguably essential if a blockchain is to last. Cardano is designed to enable the community to sustain its development by submitting

and voting on funding proposals in Project Catalyst. To maintain long-term viability, the community controls the treasury system, which is regularly topped up from various sources.

There is a clear plan in place to implement end-to-end on chain governance.

Quiz question:
![[Pasted image 20260518035555.png]]
Correct Answers:
1- **Scalability**  
2- **Governance**  
3- **Interoperability**



topic finished under the text is the separation line

---

## **Cardano Development Milestones**
"Cardano is named after Gerolamo Cardano, an influential mathematician during the Renaissance. The Cardano roadmap is made up of five major eras, each named

after prominent historical figures, Byron, Shelley, Goguen, Basho, and Voltaire. The eras overlap in places and there are some interdependencies as we'll see shortly.

Byron was Cardano's initial development phase named after the romantic poet, Lord Byron. This era focused on bootstrapping the network,

enabling users to transact in Ada Cardano's native cryptocurrency. Ada is named after Lord Byron's daughter, Ada Lovelace, the 19th century mathematician

and pioneering programmer. One Ada is equal to a million lovelaces. Cardano has a fixed supply of 45 billion ada.

Every ada holder is incentivized to stake the ada, which helps secure the network and participate in governance. More on this later. ADA holders use the Daedalus full node

wallet during this era storing, sending and staking their ada on the incentivized testnet (ITN). The full node wallet was important

during this bootstrapping, bringing security and stability to the network in the last few years, most people use light wallets.

A light wallet is smaller than a full node wallet and does not participate in block validation in the same way. The light wallet can query the blockchain,

but does not store the entire state of the chain. It is much faster as a result, but relies on a third party

to deliver (query) blockchain data. Shelley, named after Percy Shelley, another prominent romantic poet, was the decentralization phase that introduced state pools

to increase Cardano's security and scalability. Users were now able to earn rewards for staking their ADA to these pools.

On March 31st, 2021, Cardano hit a milestone, as block production became fully decentralized. On that day, stake pool operators (SPOs) began producing a hundred

percent of new blocks. The 'd' (decentralization) parameter was subsequently retired, which made the network irreversibly decentralized. There are currently over 3000 active pools

that are supporting Cardano's decentralization, with over 60% of ada staked, making it one of the most decentralized cryptocurrencies. The Goguen era, named after the American computer scientists

and academic, Joseph Goguen, introduced programmability with smart contract functionality. Developers could now create decentralized applications or dApps, as we'll refer to them

from here on. The Plutus Platform was introduced, which facilitates smart contracts written in Haskell to guarantee deterministic outputs. Goguen also saw improvements to the core Cardano offering,

most significantly the addition of a multi-asset ledger, which further enabled users to create (mint) new natively supported tokens. This allows for the creation of fungible

and non-fungible tokens, supporting the creation of new digital assets on card, as well as the tokenization of many types of physical

assets. The Basho era, which focuses on scalability, was named after Matsuo Basho, a famous Japanese poet. This era also focuses on improving the

interoperability of the network. Basho is about boosting performance of the Cardano network to support mass production as transaction volumes increase

and dApps require more resources. Finally, the Age of Voltaire is a governance era named after Voltaire, the renowned French philosopher.

To date, Cardano has used Cardano Improvement Proposals as a vehicle to manage change, as well as Project Catalyst, which serves an innovation fund

through which ADA holders can propose ideas, vote and receive funding. The Voltaire era brought voting and other governance mechanisms completely on chain.

More about this ambitious vision later. Although these eras appear sequentially on the roadmap, the development of some eras is taking place in parallel.

For example, although we are currently in the age of Voltaire, crucial scalability solutions like input endorsers will only be introduced

after an on chain vote, as they will require a significant change to the existing protocol. A big differentiator of Cardano is that upgrades are seamless.

With most blockchains, upgrades are done via hard folks, which are traumatic for the blockchain community. Typically the existing protocol is disabled,

new rules are introduced and the chain is restarted with all the history destroyed. Hard forks are handled very differently

and causing minimal inconvenience to users. The hard fork combinator is intended to allow the integration of many protocols without requiring major changes.

Byron and Shelley era blocks have previously been combined in the Cardano blockchain. For future 'hard fork events', Basho and Voltaire blocks will be combined as well, all

as a single property. The HFC hard fork combinator continues to prove itself with more gradual iterative upgrades planned. These events result in negligible, if any user disruption.

Quiz question:
![[Pasted image 20260518035921.png]]
Correct Answer: **Hard Fork Combinator (HFC)**

topic finished under the text is the separation line

---

## **What is Ouroboros?**
In Greek mythology, Ouroboros is a circular symbol depicting a snake swallowing its tail, representing wholeness or infinity of time flowing back into itself in an eternal cycle

of life, death and rebirth. So what is the connection with all this philosophical talk and the proof of state consensus protocol that powers Cardano?

In a blockchain context, Ouroboros represents the protocol constantly feeding itself from previous epochs and regenerating, kind of like eating its own tail.

Ourobors, the first provably secure proof of state protocol, is just one example of Cardano's meticulous peer-reviewed approach. Ouroboros offers the same strict security guarantees

as proof of work blockchains such as Bitcoin. It is based on sound foundational research papers, which found Ouroboros to be more robust

and adaptive to attacks than previous Byzantine fault tolerant (BFT) protocols. Nakamoto Consensus, named after the pseudonymous Satoshi Nakamoto, combines proof of work

with the 'longest chain' rule. Ouroboros achieves nakamoto-style consensus, but is based on proof of stake, achieving the robustness of Bitcoin, but is magnitudes more energy efficient, faster,

and with a fairer reward system. Cardano is built on an innovative game theoretic design, which discourages one entity gaining too much control

and avoids plutocracy. Time is measured on Cardano in epochs and slots. An epoch is a sequence of a fixed number

of slots currently lasting for five days. For each slot, stake pools who are randomly chosen to be the 'slot leader'

to produce one or more blocks. Blocks are then propagated to the network within the allocated slot time. There is a reliable randomness in the selection

of slot leaders, crucial in preventing network attacks, while also incentivizing honest stakeholders. In Ourobors, randomness is generated by using a Verifiable Random Function,

a major cryptographic breakthrough in 1999 and still used widely today to produce a random output, with the proof that anyone can use to verify the results.

When reviewing staKe pools performance, it's best to zoom out and note that it will generally receive more slots in some epoch

and fewer slots than others, but will average out over in the longer term. Cardano's rigorous scientific approach and proven track record make it a reliable foundation

for enterprise grade blockchain solutions. To date, Cardano has achieved a hundred percent uptime, second only to Bitcoin, which launched years ago.

This is not always the case with other chains where hacks, outages and restarts are well documented.


Quiz question:
![[Pasted image 20260518040110.png]]
Correct Answer: **A Verifiable Random Function**


topic finished under the text is the separation line

---

## **Staking on Cardano**
"Cardano is a proof of stake blockchain that requires a fraction of the power required for proof of white blockchains.

According to the Cambridge Bitcoin Electricity Consumption Index, the hardware that runs Bitcoin uses as much energy each year as a country such as Norway or Sweden.

Cardano's ethos is to be as inclusive as possible with a low barrier to entry. Cardano stake pools have been run on Rock Pi

as far back as 2019. What is staking? Staking is crucial to securing the network. It is the process where ADA holders delegate to their funds

to a stake pool and earn staking in rewards in return. Any ADA holder can run their own node, which acts

as a validator, processing transactions and adding new blocks to the chain. On Cardano, these are known as stake pool operators.

The more ADA stake, the stronger the network becomes. Stake pools receive rewards after each epoch, some of which are passed onto delegators.

When you delegate your ada, your stake becomes active two epochs later. You will then start receiving rewards directly into your

wallet every five days thereafter. Hence, stake and rewards are often referred to as passive income. Ouroboros provides a best in class staking experience.

There are no penalties such as slashing, where some or all of your stake can be revoked as punishment for dishonest behavior.

There are no lockup bonding periods. Rewards are distributed automatically every EPOCH and your funds are always accessible. any time. Staking on Cardano is described as non-custodial,

meaning you have sole custody of your ada and you alone are responsible for securing your wallet. When you delegate your ada, your stake is never at risk

of being taken by the stake pool operator or a third party. This is not always the case with other proof of stake

blockchains. Cardano's network is very decentralized with over 3000 globally distributed stake pools. Cardano's architecture is designed to prevent centralization

by using economic incentives that stimulate decentralization. Stake pools naturally want to expand as much as possible, the more delegated state they attract,

the more blocks they would produce. The network is configured to prevent single stake pools from becoming too large. There are a number of parameters that aim

to find the optimum balance of stake delegated to an ideal number of stake pools. At a high level, the protocol works by ensuring

that if a pool attracts more delegated stake than a given threshold, the pools payout will fall accordingly. If a pool is said to be saturated in this way,

attracting more delegated stake will no longer increase the rewards. The ideal result is a set number of stake pools

of approximately equal size. It rarely ends up this way exactly in practice, but it is sufficient motivation for most participants

to behave in an honest fashion out of their own self-interest and maximize their rewards. Note, nobody's stake is ever revoked,

but you may not be earning full rewards if you try to gain the system. Before we go, we should point out that state pool operators

SPOs, are the backbone of the Cardano network. The node (servers) they run add blocks to the network and validate transactions.

A stake pool operator maintains hardware that facilitates the Cardano blockchain and is rewarded accordingly based on stake in the

network and poor performance. Staking on Cardano has a very high participation rate compared to other chains. Cardano leverages the successful stake pool model

to implement some of the interoperability and governance features we'll talk about shortly. SPOs essentially become infrastructure providers for rolling out new features released in new node versions.


Quiz question:
![[Pasted image 20260518040326.png]]
Correct Answer: **Staking**


topic finished under the text is the separation line

---

## **What is Cardano’s eUTXO Model?**
"Businesses need some form of balance sheet to maintain an accurate record of cash in cash out profit and other key metrics.

Ledgers have been used in double entry bookkeeping since the 13th century. Blockchain introduced the notion of a shared distributed ledger

and immutable record of all transactions. To achieve this blockchain, networks need an accounting model to record who owns which coins, as well as

to identify which ones are spent and unspent. Let's review the two most common blockchain accounting models and how Cardano has innovated further

with the EU TXO model. A bank's bookkeeping model is often used to explain how the account model works. Your balance is a single figure updated whenever you deposit

or withdraw funds. This is analogous to the blockchain account model where your blockchain address holds a single balance that fluctuates with transactions.

Transactions are recorded as debits and credits on different user's accounts on the bank's ledger. Account-based blockchains work similarly except the ledger

that records its user's balances is distributed among many nodes on the network. Note that account-based blockchains track updates to balances, not the actual coins

and balances are stored as a global state kept by each node and updated with every transaction. The account-based model is a popular blockchain bookkeeping

method initially introduced with Ethereum. The account model is used today by many other blockchains, such as Algorand, to record transactions

and track state changes. An alternative model is UTXO, which stands for unspent transaction output. It's often explained with cash in cash out analogies.

Imagine you're in a bookshop buying goods with physical notes and coins. Every transaction involves handing over specific notes and coins, and your balance

reflects the money you have left. This is akin to the UTXO model in blockchains where individual notes and coins UT XOs are tracked to represent your balance,

Bitcoin uses the UTXO model. Cardano adds programmability to Bitcoin's proven UTXO model with its extended U-T-X-O (eUTXO) ledger model,

where smart contracts allow developers to build dApps with custom logic while still maintaining security. Transaction verification is simpler, so you can predict what's going to happen, including

how much a transaction will cost. Transactions can be verified locally off chain, and there is no dependence on the rest of the network.

A developer can focus on the transaction itself and its inputs. Unlike Ethereum, if a transaction fails, no fee is charged.

Crucially, Cardano's EU TXO model can process multiple transactions from a single transaction. This changes the entire context for metrics like transactions per second.

Users can also send multiple assets to several wallets in a single transaction, thus cutting transaction fees even more. We will look at this transactions per transaction concept

closely in a future video.

Quiz question:
![[Pasted image 20260518040536.png]]
Correct Answer: **Cardano**



topic finished under the text is the separation line

---

## **Smart Contracts on Cardano**
Plutus and Marlowe were the main programming languages for Cardano in the early years. Plutus is a platform providing the supporting infrastructure

and tools for writing smart contracts. In Haskell, plutus and Haskell are often used interchangeably. If you hear someone saying it's coded in Plutus,

they really mean they are coding in Haskell, using the Plutus framework. To be specific, the Plutus Framework enables developers to create dApps,

which interact with a distributed ledger featuring scripting capabilities. It's not just a language, it's an entire platform that supports dApp development in its entirety,

end-to-end from writing scripts to testing, runtime support and verification. Plutus is a platform made of three main components: Untyped Plutus Core (UPLC) is the 'machine code'

for the Cardano ledger. Plutus TX is a plugin for compiling Haskell into UPLC to form the on chain component renamed

to 'Plinth' in the summer of 2024. Plutus Application Framework is the collection of tools for writing smart contracts in Haskell.

It is said that to become a proficient developer on Cardano, one must understand three key concepts: The Extended Unspent Transaction Output, E-U-T-X-O model

On-chain code, Plutus Core, which runs on the blockchain Off-chain code, which runs on the user's device. Marlowe is a simple programming language

for writing financial smart contracts for Cardano. It is named after the Elizabethan poet, dramatist and spy, Christopher Marlowe. Marlowe is limited to financial applications

and is not Turing-complete. It is a DSL (domain-specific language) for people who are experts in finance rather than programming. You can code in Marlowe directly

or also utilize Blockly, a visual programming tool that allows you to design contracts by dragging and dropping connecting blocks

that represent the various components. It's important to emphasize that you do not need to know Haskell to write smart contracts on Cardano.

Let's zoom out for a moment to understand the bigger picture. As we mentioned, Haskell programs coded on the plutus

platform, compiled to un typed Plutus core UPLC, and while the Cardano ledger only understands Plutus core, this low level machine language is not something developers

code in day-to-day. You can choose from a growing list of high level languages, which compile to UPLC. Developers crave flexibility to use their favorite language

for what is typically the largest part of their dApp, the off chain component. So although Cardano is implemented in Haskell, it is UPLC

that is actually executed. There is no dependency or reliance on Haskell. Other languages can compile to UPLC too. One of those is Aiken. Named

after the mathematician, Howard Aiken, it is a functional domain, specific language (DSL) written in Rust and released under an open source license.

Unlike Haskell, it is built specifically with the Cardano blockchain in mind. It places an emphasis on the developer experience

and comes with 'batteries included' state-of-the-art tooling, taking inspiration from modern programming languages like Rust, Elm and Gleam. Aiken is a lean language which aims

to free itself from unnecessary features and instead provide a comprehensive, opinionated solution with minimal configuration needed. Everything works out of the box

and with language wide standards enforced by the compiler. Developers have remarked how Aiken is easy to learn and getting started takes just a few minutes.

Aiken adopts a 'keep it simple' approach. Compared to other languages, Aiken scripts, by design, do not support as many features

as general purpose Turing-complete languages. Aiken is a small language, not a high level general purpose language designed meticulously to produce small, efficient scripts

for on-chain Cardano smart contracts that integrate with most languages off chain. 'Aiken uses exhibit a tendency for Rust in off chain scenarios' according to the findings

of the state of the Cardano Developer Ecosystem 2023. Aiken has garnered praise from developers for its Rust-like syntax, which retains the strengths

of Haskell as a functional language in its own right. Many developers have reported substantial performance gains with faster, more efficient, smart contracts.

Aiken's thoughtful design supports blueprint stub generation, which are effectively templates for different programming languages, facilitating an effortless integration between Aiken

It is a new language built from the ground up with Cardano in mind. Helios is also a functional language,

but is very similar to TypeScript. OpShin is an implementation of Cardano smart contracts written in a strict subset of Python.

It enables you to write smart contracts in completely valid, albeit restricted Python3. Plutarch is a typed eDSL (embedded domain specific language) in Haskell

for writing efficient Plutus Core validators. It is not a new language, it's just good old Haskell with no restrictions.

plu-ts is a library to enable Cardano related software to be written entirely in TypeScript. Scalus is a Scale implementation of Plutus.

Unlike many blockchains who adopt a 'move fast and break things' approach, Cardano has always stuck to a deliberate, careful and methodical strategy.

Despite this relative conservatism, Cardano's GitHub repositories have been very active in 2021, 2022, 2023, and again in 2024. As adoption grows, there are more

and more options for newcomers, acknowledging that Java is still the preferred language for many enterprise developers, the Cardano Foundation has written various tools

and services in Java and released them under an open source license to encourage collaborations and community contributions. For example, the Identity Wallet is a W3C-compatible

mobile wallet for managing self-sovereign identities across Cardano and other blockchains. The wallet supports multiple standards, integrating key event receipt infrastructure, KERI,

for interoperability so as to fit a broad range of use cases and foster enterprise adoption

Quiz question:
![[Pasted image 20260518040749.png]]
Correct Answer: **Aiken**







The whole Chapter is finished under the text is the separation line for the new module

---
New chapter is down (Cardano Deep Dive)
# Cardano Deep Dive
the 6 topics of the **Cardano Deep Dive**:
1. **How Will Cardano Scale?**
2. **Scalability Case Study: Hydra**
3. **Cardano's Monetary Policy**
4. **NFTs on Cardano**
5. **Interoperability on Cardano**
6. **Governance on Cardano**


## **How Will Cardano Scale?**
Scalability is a blockchain's ability to handle usage or adoption. Measuring scalability is not simply measuring the TPS (transactions per second),

it is more nuanced than that. TPS is perhaps the crudest metric to use as transactions occur in a variety of sizes and formats.

Instead, we must consider a wide range of metrics. Throughput is the quantity of data that a system can process in a given length of time.

Script execution time, how long was the CPU busy for? Finality is the amount of time it takes for a transaction

to become immutable. Concurrency is the amount of work various actors can do without interfering with one another. The actual size of transaction.

Any blockchain can appear fast using tiny transaction sizes and no scripts. Some high profile blockchains have centralized characteristics, such as a minority of validators,

controlling disproportionate amounts of stake. It's easy for a blockchain to compromise on decentralization, then boast astronomical TPS figures. We should also note that throughput means something

different in a UTXO system than it does in an account-based system. TPS on Cardano is yet more nuanced due

to its native asset capability. E-U-T-X-O allows hundreds, even thousands of native assets to be transferred in a single transaction.

Nearly everything on Cardano occurs as a transaction, and generally speaking, resources are consumed from these types of activities. Transferring ADA, issuing assets,

executing smart contracts, voting and adding metadata. A more accurate metric is therefore TPT (transactions per transaction). To understand and visualize how transactions work on Cardano,

visit eUTxO.org, a blockchain explorer which presents a live view of blocks and their contents being created. There is no 'magic bullet' for scaling blockchains,

it's done by tweaking parameters and combining different solutions that generally fall into two categories: Layer one solutions: upgrades applied to the main chain, ie.

Cardano. Layer two solutions: offloading workloads, extending functionality, and integrating other blockchains with side chains, ZK roll-ups and state channels.

Scaling solutions are usually categorized as either on chain solutions, which encompass block size increases, pipelining, input endorsers, parameter adjustments, Plutus script enhancements,

node enhancements, and on-disk storage improvements. Then there are off chain solutions, including sidechains, partner chains, Hydra, off-chain computing, and Mithril.

We'll dive deeper into these solutions in future courses. There's also the actual size of the blockchain to take into account.

Blockchains can store data infinitely. All transactions recorded on the blockchain are logged regardless of relevance as the number of transactions per second increases.

A bloated blockchain leads to slower sync times for wallets, it's like flooding your basement with water. It's likely to make life difficult in the long term. Cardano's.

architecture focuses on moving a lot of the computation off chain and storing the minimum on the mainchain. Bitcoin's blockchain size passed half a terabyte in

late 2023. Ethereum, on the other hand, requires wallets to download over a terabyte of data to sync. Cardano compares favorably at 191 gigabytes

if you consider Solana has bloated to 3.8 terabytes.


Quiz question:
![[Pasted image 20260518041453.png]]
Correct Answer: **Finality**



topic finished under the text is the separation line

---
## **Scalability Case Study: Hydra**
"We talked about the Lightning Network on Bitcoin earlier. Hydra is another layer two scaling solution tailored for Cardano. Hydra introduces isomorphic state channels

to increase throughput with reduced transaction fees and storage needs. Hydra is developed using principled evidence-based research, making it easier to perform transactions off chain while

utilizing the main chain ledger for secure settlement. Hydra can sound very complicated, but let's demystify some of the jargon.

Let's first clarify what isomorphic state channels are. ISO is a prefix meaning equal, like you may have heard the term isometric,

meaning equal measurements. Morphic is related to shape or form, so isomorphic means having the same structure and properties. State channels extend the idea of payment channels

to also support smart contracts over off-chain channels. Participants in the channel can now, in addition to traditional transactional payments, execute scripts

to handle complex logic off chain before committing the result back to the layer one main chain. Participants lock funds into a smart contract.

They can then transact with others in the state channel off chain in whatever fashion meets their use case. Afterwards, the outcome is settled on chain without

requiring the full transaction history of what occurred off chain. In the meantime, developers can leverage Cardano's proven infrastructure to develop wallets

and dApps that communicate with the layer two system drastically reducing the learning curve for Hydra. While Hydra is being developed in collaboration

with the Ouroboros protocol and the Cardano ledger, it may also be used with other systems that have the same properties as Cardano.

Hydra replicates the main chain's functionality while minimizing friction for users, but still allows the flexibility of having a different fee structure

and timing constraints on the layer two. Hydra gels seamlessly with Cardano as extended UTXO and smart contracts allow developers to build rich isomorphic state channels.

In comparison, the Lightning Network faces some friction as Bitcoin does not support programmability.


Quiz question:
![[Pasted image 20260518041651.png]]
Correct Answer: **Hydra**



topic finished under the text is the separation line

---
## **Cardano's Monetary Policy**
You may often hear the term tokens in regards to cryptocurrencies. This is referring to the economic model of a coin

or token, including its total supply, circulating supply, and initial distribution among other factors. Cardano had a very fair token distribution in comparison

to its counterparts with 80% of ADA owned by the public. The total supply of 45 billion ADA refers to the amount

of ADA that will only ever exist, and approximately 35 billion of that is the current circulating supply. Cardano's monetary policy is a carefully considered approach

to ensure the inflation rate remains low in the long term. This is achieved by setting a parameter to control the maximum percentage of aada

that can be released in a given period. The Cardano monetary policy is the result of academic research on the game theory associated

with inflation, including a rigorous analysis of the effects of Cardano's circulating supply on its overall value. Cardano's monetary policy is designed

to incentivize stake pool operators to participate in the staking model to guarantee the long-term sustainability of the network. ADA holders who delegate

and stake pool operators are rewarded for their support with a proportion of ada each epoch in addition to transaction fees.

Transaction fees are deterministic or predictable for developers interacting with Cardano. Compared to other cryptocurrencies, Cardano handles fees a little differently.

Fees do not go straight to the block producer. Instead, they are pooled and distributed to all stake pools that created blocks

during an epoch. Incentivizing users to participate in staking and governance is not an exact science. There are examples of blockchains

who have suffered low participation numbers and have switched to a model that pays participants. Cardano's monetary expansion depends on a long-term commitment by

stake pool operators to support the chain. It is the SPOs who run the cardano-node, which is the heartbeat of the network.

The incentive system does not significantly change over time, and while staking rewards gradually depreciate, transaction fees should increase as adoption grows.

SPOs can also receive rewards by providing similar support for side chains and partner chains. More about that shortly. Cardano's

monetary policy focuses on two main points: one, staking rewards for those participating in the network as discussed above. Two, funding the treasury.

Staking rewards come from two sources. Fees from every transaction and from all blocks produced during each epoch go into a virtual pot.

A fixed percentage of the remaining ADA reserves is also added to this pot. every epoch. ADA reserves is the difference between total supply

and circulating supply. That percentage, denoted RHO, is known as the monetary expansion. It is a protocol parameter currently set at 0.3%,

but may be updated in future. A set percentage of the pot is then sent to the treasury, and the rest is used as epoch rewards.

The treasury is another important keystone of Cardano's monetary policy. The goal is that there will always be funds available to develop Cardano.

The funds should be accessible through governance mechanisms where proposals are voted on by ADA holders. Funds are regularly sent to the Treasury

to ensure it is always topped up. This main goal of Project Catalyst and ultimately the 'Age of Voltaire' is to enable access

to treasury funds via on chain governance mechanisms. There are many other parameters you can review online, will look at them in greater detail in future courses.

Quiz question:
Which of the following refers to the economic model of a coin or token, including its total supply, circulating supply and initial distribution among other factors?
![[Pasted image 20260518041905.png]]
Correct Answer: **Tokenomics**


topic finished under the text is the separation line

---

## **NFTs on Cardano**
Crypto can be rife with jargon, especially with NFTs, where terms like coins, tokens, currencies, assets, multi-asset, et cetera, are often used interchangeably.

Sometimes use cases overlap and tokens fit into multiple categories. A reminder, we have a supporting glossary for this course,

which you can review as needed. Almost everything in Cardano can be traced back to the research papers. Native assets are no different

with the original concept discussed in the Native Custom Tokens in the extended UTXO model paper. Cardano has the unique ability to create, interact with,

and delete bespoke tokens or assets natively. When we say 'native', we mean that in addition to sending and receiving the official currency, ada, you may interact

with custom assets right out of the box without the need for smart contracts. Fungible and non fungible tokens, NFTs are both native assets treated as first class citizens,

meaning they have the same capabilities as ADA in every sense because the functionality is already built into the protocol.

This reduces complexity, making it easier for developers and opens up new uses. Cardano's native assets function based on a set of rules

that govern the creation, issuance, and management of native tokens on the Cardano blockchain. This design has broad ramifications, for example, all the security features that apply

to ADA automatically apply to your token. Multi-asset support is written into the integration with centralized exchanges, so now it's easy for exchanges

to list your newly minted token. Also, everything that comes with the governance stack, the voting mechanics seamlessly work for your token as well.

No code has to be rewritten. It's a 'batteries included' turnkey solution. The creation and transfer of native tokens cost a fraction

of transaction fees on other chains. You can check how much something will cost in advance and it won't spike later just because the network is busy.

This predictability is referred to as determinism. Native tokens are scalable because they do not require the use of a separate layer

for smart contracts, this makes it possible to transfer a large number of digital assets in one transaction to multiple wallet addresses.

Native assets are flexible and can be customized to meet the specific needs of different dApps. Native tokens are more secure

because they are managed by the Cardano ledger itself, which makes them transparent and auditable. The policy is set by the user who wishes

to mint the new asset. The node checks adherence to minting policies when a transaction is processed by running the code

or checking for the required signatures. Transaction data must satisfy the minting policies of all assets the transaction is attempting to mint.

Native tokens represent value and act as an accounting unit, so they can be used for payments and transactions in the same way as ADA is.

While ADA is used as Cardano's main currency for fees and rewards today, there is a clear path laid out

in a research paper (Babel Fees via Limited Liabilities) on how users can potentially pay transaction fees in native tokens in future. Cardano is designed so the EU TXO model

and native asset design work seamlessly together with efficiency and robust security properties built in. Cardano's design decisions enable unique features such

as a token bundle, which is a mix of token scoped under one or more minting policies. Any tokens can be bundled together, including ada.

You can see how powerful this feature can be by reviewing some of the records on eutxo.org. Unlike Ethereum's ERC20 standard,

native tokens do not require special transfer fees or additional event handling logic to track transactions. With Ethereum, ether is an asset and ERC20 is a smart contract

and both compete for resources while at the same time being treated differently by the blockchain. ERC20 token creation requires manual modification

of the contract standard, which opens the door for human error and likelihood of bugs. There have been billions of dollars lost due

to security issues resulting from such designs. We will explore this in more detail in the Cardano Blockchain Certified Associate CBCA course.

Quiz question:
![[Pasted image 20260518042057.png]]
Correct Answer: **Determinism**


topic finished under the text is the separation line

---

## **Interoperability on Cardano**
Interoperability is defined as the ability of blockchain networks to talk to each other, enabling secure transactions and transfer of digital assets and tokens.

Mass adoption is also dependent on enabling interoperability with the legacy financial system enabling users to onboard to and exit from the fiat currency world.

In addition to inventing the first provably secure proof of stake protocol called Ouroboros, Professor Aggelos Kiayias and his fellow researchers introduced a whole gamut

of interoperability protocols such as non-interactive proofs of proof of work and side chain protocols. If the different blockchains and systems don't have a seamless way to communicate

with each other, everything works in silos and potential user bases are diluted. Sometimes it makes business sense for traditional rivals

to partner for mutual benefit. Take cloud service providers, for example. Oracle is available on Microsoft Azure and Amazon Web Services

although they compete in many areas. Sidechains are a key enabler for interoperability. A sidechain is a blockchain in itself linked

to a main blockchain, the main chain or parent chain through a two-way mechanism called a bridge. Digital assets from one chain can be utilized in another

and the results shared back and forth. Multiple side chains may be joined to a single parent chain, each of which can function in a different fashion.

A side chain can be thought of as just another blockchain. The difference between them is often philosophical, not technical.

The side chain typically aligns with the main chain, but can have its own business logic, cryptocurrency, monetary policy, consensus rules,

programming language, subset of users, smart contract capabilities, stablecoins, use cases like NFTs, loyalty points, et cetera. Side chains are suited to medium to low risk protocols

where new or growing ecosystems need a jumpstart as the side chain can leverage an existing main chain security, liquidity wallets

and user base. Side chains can literally take a load off a layer one main net, all the while enjoying the veracity

provided by its parent chain. Even if there is large transaction traffic on a side chain, these transactions don't need

to be reconciled on the main chain. A side chain won't eat up the resources from its parent main chain. As you might expect at this stage, a lot

of deep thought and academic rigor went into Cardano's architecture. Another example is in how rewards incentivize side chain partnerships.

ADA holders who delegate their stake get rewarded in ada, however, the same SPOs that power the main chain will also provide staking liquidity for side chains.

The result is if the SPO you delegate to is also part of the side chain SPO subset, you will also be rewarded in

that side chain's native asset in addition to your usual ADA rewards. The 'Why Cardano' essay from 2017 describes the vision

for a layered architecture. The strategy and terminology was updated slightly in 2023. The new model would mean there would still

be separation of layers. The Cardano Asset and Settlement Layer (CASL) will act as a proven robust settlement layer for partner chains,

while the Cardano Service Layers (CSL) mirrors the philosophy of microservices or service oriented architecture. You can think of partner chains as an extension

of the side chains concept. Midnight is muted to be the first of its kind. Midnight will be a fourth generation blockchain

as it will enable data protection and follow a multi resource consensus model, leveraging both proof of work and proof of stake simultaneously.

Advancements in zero knowledge proofs will enable data and metadata to be protected. Blockchains can't keep a secret today, Midnight aims to introduce this capability

and with it a new world of use cases. Partner chains will have the flexibility to construct their own computation layers using modular

components while still leveraging the CASL. Each CSL service layer can have its own distinct logic with unique token ons, consensus protocol, et cetera,

but they will all have the same common ancestor in the CASL. This design will mean Cardano could potentially be the

settlement layer for other blockchains. Security will be provided by Cardano's SPOs as before, but now multi resource consensus will allow validators from

other chains to contribute. The introduction of Babel fees (still in research) will allow chains to integrate smoothly as users will be able

to transact in their own native currency while card SPOs can still be rewarded in ada.


Quiz question:
![[Pasted image 20260518042243.png]]
Correct Answer: **Interoperability**



topic finished under the text is the separation line

---


## **Governance on Cardano**
## Transcript of "Governance on Cardano"

"One of the cornerstones of Cardano is decentralization, but true decentralization must be realized across three planes: block production, consensus networking, and governance.

Cardano has traditionally managed update proposals and trialed governance tooling through two mechanisms. The Cardano Improvement Proposals, CIP, helps steer the boat

from a technical standpoint. Engineers and product designers propose reusable technical solutions to common problems. The other mechanism is Project Catalyst,

a community-driven innovation fund. Cardano holders can propose projects, review, comment, and vote on them. Community funds are allocated to the most promising initiatives.

Catalyst takes an experimental approach, and the process has been tweaked and improved over standalone funding rounds. Governance on Cardano is still in its infancy,

and we are now in the phase of implementing on chain mechanisms to realize the vision for the age of Voltaire.

Many of the learnings taken from the catalyst journey are fed into CIP 1694. CIP 1694, named after the year of Voltaire's

birth, is a proposal for bootstrapping on chain governance. Back when Cardano was formed, there was a tripartite structure with Emurgo, Cardano Foundation (CF) and IOG.

It was always intended to transition to a members based organization, MBO, that would manage the bureaucracy of protocol governance. Throughout 2023

and 2024, IOG and the CF ran workshops all around the globe to gather feedback and refine CIP 1694. To summarize, the proposal focuses

on three different categories. One, the idea of representation. Direct representation is where an ADA holder personally votes and delegated authority,

where you hand someone else your vote. In CIP 1694, this role is called a DRep, a delegated representative. A constitution describes the guardrails for the system

to ensure some degree of stability. For Cardano, this constitution can be drafted to be machine understandable, so once a voting mechanism is in place,

the constitution can then be ratified, hashed, and embedded into a transaction. Institutions set standards and facilitate a review process by domain experts acting

as the custodians of knowledge and best practices. One member's based organization or MBO focusing on Cardano governance is called Intersect.

It is an aggregation point for anyone interested to meet and debate issues, manage Cardano's roadmap, facilitate the development of strategies to achieve key milestones,

and attract suitable developers and entities to build tooling, services, critical infrastructure, et cetera. While intersect is the anchor institution for Voltaire,

it is just one. Another MBO is pragma, which attempts to foster an alternative open source ecosystem for Cardano and other blockchains.

In summary, while liquid democracy is not a new concept, and constitutions have been written before, nothing on this scale has been

attempted in the crypto space. The following are some of the key milestones for the age of Voltaire. In the fourth quarter of 2023, Cardano wallets Lace,

Yoroi, and others announced integration into the Governance Tool (GovTool) for Voltaire testing within SanchoNet. The Interim Constitution was drafted providing a framework

for the Constitutional Committee to function during the bootstrapping phase. Throughout 2024, there was ongoing community consultation through another series of workshops to discuss

and debate Cardano's constitution. Feedback from the workshops was fed into the constitutional convention, which took place in Buenos Aires and Nairobi, Kenya

in December, 2024. Delegates representing over 50 countries voted in favor of the Constitution. The DRep Pioneer Program supports prospective candidates on

understanding the DRep role, code of conduct, the delegation process, how to become a DRep, DRep rewards, engaging with the community

among other topics. Intersect provides similar support for the Constitutional Committee, ensuring that members are trained for their roles and are able to execute effectively.

There are several working groups and committees with different remits, such as the Membership and Community Committee, Technical Steering Committee,

Open Source Committee, Parameter Committee, Vision Committee, Budget Committee, product Committee, and Cardano Civics Committee. The Chang upgrade in September, 2024 was another Cardano

milestone as it implemented a minimum viable on chain governance. The Plomin upgrade followed in January, 2025 where all on chain governance actions were turned on.

The Constitution was subsequently ratified in an on chain vote when a governance action was submitted and passed the required threshold.

Quiz Question:
![[Pasted image 20260518042526.png]]
Correct Answer: **Constitution**


The whole Chapter is finished under the text is the separation line for the new module

---
New chapter is down (Benefits & Use Cases)
# Benefits & Use Cases
The 10 topics of **Benefits & Use Cases** are:
1. **Blockchain Business Benefits**
2. **Is Blockchain Right for Your Use Case?**
3. **Different Kinds of Use Cases**
4. **Role in Web3**
5. **DeFi**
6. **Tokenization**
7. **Gaming**
8. **Payment Rails**
9. **Supply Chains & Traceability**
10. **Blockchain for Good**

## **Blockchain Business Benefits**
For the rest of the course, we'll focus on the business side of things, listing the types of use cases blockchain enables and some of the business models which have sprung up. By the end, you should be able to conclude if blockchain is the right fit for your business. Blockchain has the following benefits for business: Transaction times: compared to traditional interbank transfers, Cardano has demonstrated it can transfer thousands of digital assets to multiple recipients globally and settled in minutes for minimal fees. There is no verification required from a central authority or clearing house. Cost savings: A blockchain network reduces expenses in several ways. The network is self policed by network participants through 'inclusive accountability'. 'Killing the middleman' as intermediaries are no longer required participants exchange value directly. Duplication of effort is eliminated because the shared ledger provides a single source of truth. Security: Blockchain inherently protects against interference, fraud, and hacking. Privacy: The Cardano Foundation offers a digital identity wallet that prioritizes security, privacy, and interoperability to drive adoption and support existing ecosystems. Users can securely generate, update, deactivate, and restore decentralized identifiers, DIDs, and KERI (Key Event Receipt Infrastructure) Automatic Identifiers (AIDs). Zero Knowledge proofs, and other cryptographic primitives enable selective disclosure and other advanced privacy capabilities. Blockchains can be permissioned or permissionless. Some companies use permissioned blockchains to achieve privacy. Permissioned blockchain provides each participant with a unique identity enabling the use of policies to restrict participation and access to sensitive details. Permission blockchains are adopted sometimes out of necessity to comply with data protection regulations. For example, to protect medical records in accordance with the Health Insurance Portability and Accountability Act HIPAA. Auditability with a shared public ledger provides a 'single pane of glass' for monitoring and auditing transactions. Operational efficiency, cryptocurrencies, and the blockchains they run on operate 24/7 with no concept of 'business days' or public holidays. Tokenization of assets streamlines near instant transfer of ownership. Smart contracts can contain business terms and conditions that could be written in a way to be self-executing and self-enforcing. This offers more security and efficiency than traditional paper contracts.

Quiz question:
![[Pasted image 20260518043312.png]]
Correct Answer: **The blockchain provides complete anonymity for those who prefer complete privacy**



topic finished under the text is the separation line

---
##  **Is Blockchain Right for Your Use Case?**
Quiz question:
![[Pasted image 20260518043342.png]]
Correct Answer: **Porter’s Five Forces**





topic finished under the text is the separation line

---

## **Different Kinds of Use Cases**
Quiz question:
![[Pasted image 20260518043439.png]]
Correct Answer: **Payment rails**




topic finished under the text is the separation line

---

## **Role in Web3**
Blockchain technology is the foundation stone for Web3, but what is Web3? To understand the future let's recap the past first. Web 1.0 refers

to the Internet's early days in the 1990s characterized by static text-based websites where the primary activity users did was to read.

It was a little like an encyclopedia, users could search and study topics, but there was little stimulation or interactivity.

Web 2.0 arrived in 1999, coined by Darcy DiNucci to distinguish it from Web 1.0. Web 2.0 saw the introduction

of interactive websites like YouTube and Facebook. If Web 1.0 was a read era, web 2.0 allowed users to read and write.

The big tech companies subsidized the huge storage expenses so users could upload content and social media was born. User generated content with garner reactions

and sentiment based algorithms would become ever more sophisticated thereafter. It was Gavin Wood, co-founder of Ethereum who introduced the term Web3 to describe the next iteration

of the internet, which would revolve around blockchain. While it has become somewhat of a buzzword bandied about, you can think of it as a decentralized network

where the users now read, write, and own their content currency and digital assets. Blockchain is often said to kill the middleman,

and in this case, the big tech companies are the middlemen whose stranglehold on user data is removed. Here is an example that might resonate

with you right now depending on what browser you are using. Most people unwittingly disclose a lot of data just by surfing the web.

Brave is a browser based on Google Chromium that protects user privacy. By leveraging blockchain technology, it flips the traditional advertising model by compensating

for ads in its ERC 20 token, BAT or Basic Attention Token. Another Web3 term is the semantic web where computers can comprehend

and use information just as humans do. With the relentless advancement of AI continuing at a dizzying pace, blockchain may be adopted out of necessity

to ensure the integrity of digital content against deep fakes. The biggest use case for blockchain in future may be its ability to verify

and authenticate digital content. For example, a video's unique hash could be recorded on chain before a video is played.

Its authenticity can be verified by cross-checking its hash against the hash on the blockchain. Some of the less glamorous use cases

of blockchain are infrastructure solutions that offer an alternative to the major cloud providers. For example, IPFS (interplanetary file system) is like

a file system for the blockchain world. This provides users with a place to store and retrieve large data sets with all the benefits

of blockchain, decentralization, data integrity, and so on. There are also decentralized compute offerings.


Quiz question:
![[Pasted image 20260518043642.png]]
Correct Answer: **Brave**

topic finished under the text is the separation line

---

## **DeFi**
Defi or decentralized finance is arguably the number one use case for blockchain to date. While TradFi has barriers to entry

and can discriminate against those in the developing world, DeFi is more inclusive dispensing with the requirements for KYC registration and minimum account balances.

DeFi creates an open, transparent, and decentralized alternative by removing the various intermediaries. DeFi allows users to have self custody of their own assets

and transact directly with anyone globally. The term DeFi was coined in 2018 by Ethereum developers who introduced smart contracts to the blockchain space,

building on the 2009 breakthrough of Bitcoin as the first peer-to-peer digital currency. ERC token standards opened the door for the proliferation

of NFTs and financial services like stable coins, decentralized exchanges, lending and borrowing protocols, and yield farming. Yield farming refers

to depositing tokens into a liquidity pool to earn rewards paid out in a native currency or sometimes the protocol's own token. Think of it

as providing liquidity in return for favorable interest rates. The DeFi space has grown steadily since with other blockchains adding

to the total value locked TVL on sites like DeFiLama, which tracks such metrics. As you would expect in an unregulated industry

there are plenty of scams, so DYOR 'do your own research'. Some users, especially newcomers, tend to leave their funds on centralized exchanges, CEXs,

just out of convenience. However, it is generally safer to self custody as you have total control and access to your funds.

DeFi happens mostly on decentralized exchanges, DEXs, where trading takes place via self-executing smart contracts and peer-to-peer transactions. There are no intermediaries.

ADA and digital assets transfer back and forth between users' wallets. DEXs on Cardano make use of determinism (reliability) of afforded by the E-U-T-X-O model.

A stable coin is a fixed price cryptocurrency, which is pegged or backed by another stable asset. Stable coins enable instant payment

and settlement of transactions, but most importantly, they offer a safe haven from volatility. Stable coins represent a stable asset regardless of

how other assets fluctuate or if a country suffers from high inflation or an unstable national currency. It's generally accepted that stable coins are essential

for a blockchains defi ecosystem to flourish. We delve into the different kind of stable coins in future courses.


Quiz question:
![[Pasted image 20260518044151.png]]
Correct Answer: **Stablecoin**

topic finished under the text is the separation line

---

## **Tokenization**
Tokenization is the on chain digital representation of real world assets. Native assets or tokens are the smallest pieces of data on the Cardano blockchain.

They are defined by three things, a name, a minting policy, and an amount. Just one example where tokenization offers a solution is

around the diamond mining industry. Most people have heard of the story of 'blood diamonds' mined and war zones, and sold to finance, all kinds

of nefarious activities. The establishment of the Kimberley Process in 2003 is a multilateral trade regime that outlines safeguards for preventing and eliminating blood diamonds from the

global supply chain. This includes some required criteria to certify diamonds are from legitimate sources. Blockchain is an obvious platform for such requirements.

An immutable audit trail enables compliance, and retailers can verify supplier credentials. NMKR, an NFT and tokenization service, partnered with Tiamonds

to bring tokenized diamonds to Cardano and also provide user-friendly plug and play tools for projects. NFTs can be used for many other different use cases in a

blockchain powered digital economy. Fungible tokens can be used in a wide range of different contexts. Defi DAO tokens, for example,

a utility token can be integral to a decentralized lending and borrowing protocol. Utilizing a non-custodial system, NFT backed loans can be facilitated, enabling users

to leverage their digital assets. Loyalty points to reward and incentivize readers. Wrapped assets. For example, Wrapped BTC is a synthetic version of Bitcoin

represented by a token, built and deployed through a smart contract on other blockchains. Meme coins are tokens usually based on a joke rather than

real world utility. Staking. Native tokens can be staked to participate in a protocols operation. In return, users benefit from yield farming opportunities

where users can stake Liquidity Provider (LP) tokens to earn additional rewards, usually in the form of the platform's native token. NFTs also have a wide variety

of use cases: profile pictures, digital art, collectibles, digital twins - digital copy of something in the real world, POAP NFTs

(Proof of Attendance Protocol) shows you attended or took part in an event. Fractional ownership of physical assets like property,

fine art. Gaming, NFTs can be used in all types of creative ways in gaming, which segues us nicely to our next video.

Quiz question:
![[Pasted image 20260518044259.png]]
Correct Answers:
1- **A minting policy**  
2- **A name**  
3- **An amount**

topic finished under the text is the separation line

---


## **Gaming**
While trillions of US dollars were printed in 2020 alone, many cryptocurrencies such as Bitcoin and ADA have a hard cap on their supply,

which creates scarcity. This scarcity can be extended to tokens and other digital assets in gaming and the Metaverse. The Metaverse is a 3D virtual world

built on augmented and virtual reality, and is popular for online role playing games. McKinsey and Company predict the Metaverse economy

to reach a $5 trillion by 2030. Markets and economies form around the creation and trading of tokens and digital assets.

For example, gamers can be rewarded in-game assets for clearing stages of a game. These in-game assets can be tokens, collectibles,

virtual lands, NFT, art, avatars and so on, with various levels of digital scarcity. New terms of entered the lexicon like 'GameFi' (Game Finance).

Many games have become widely popular, offering 'play to earn' models for players. They can earn various digital assets by reaching milestones,

beating other real world players, or AI generated opponents. Often these in-game assets can also be traded on real world exchanges.

This is a break from traditional 'pay-to-play' games, which often require a subscription. This is the familiar theme throughout the old Web 2.0 gaming

world, where the gamer is just paying for a license that can be taken away by a game studio. There are no incentives around earning, collecting,

or trading various digital assets. Blockchain offers gamers the opportunity for true ownership. Web2 games can currently handle more transactions

and active player online than a Web3 game, but as blockchain scaling solutions mature, the gap is closing.


Quiz question:
![[Pasted image 20260518044532.png]]
Correct Answer: **The Metaverse**

topic finished under the text is the separation line

---


## **Payment Rails**
A payment rail is the digital infrastructure enabling money transfers. TradFi, or Traditional Finance, is made up of centralized institutions who control the flow of funds

between permission parties in exchange for transaction fees. These fees are usually high compared to blockchain alternatives, usually because of the lack of credible remittance alternatives.

On a blockchain, counterparties transfer value on a public ledger that records and validates the details publicly at the same

time for everyone. Blockchain disrupts the current hierarchical financial system by 'killing the middleman'. The middleman in this context can be any

of the following intermediaries: real-time gross settlement, RTGS, networks or equivalent fund transfer systems. Interbank networks such as the Clearing House

Interbank Payments System (CHIPS), automated clearing House (ACH), and Fedwire Payment System, among others. Society for Worldwide Interbank Financial Telecommunications (SWIFT), the communication network

for both a ACH and wire transfers. Credit card networks like Visa, MasterCard, and American Express. Visa is now enabling crypto withdrawals on a large scale.

FinTech applications like Stripe, PayPal, Revolut, et cetera, which connect to the ACH or RTGS networks to settle payments also now enable users

to buy, hold, and sell cryptocurrencies. Blockchain transactions are irreversible, but custom logic can be codified in smart contracts to allow some recourse in the event of a dispute,

failure to deliver service or other form of trust breach. Blockchains are permissionless and inclusive for anyone with an internet connection.


Quiz question:
![[Pasted image 20260518044647.png]]
Correct Answer: **True**

topic finished under the text is the separation line

---


## **Supply Chains & Traceability**
Supply chains often involve many different intermediaries, consolidating many different data sources to track goods from suppliers to consumers. Blockchain technology can simplify interactions

between different stakeholders where every touchpoint can be tracked and logged on a shared public ledger. Many industries and verticals rely

on efficient supply chains. International shippers have adopted blockchain technology to monitor shipments and ensure containers are not tampered with any business.

Relying on perishable goods being delivered in time can review the entire path tracked on a blockchain. Payment can be made once delivery is confirmed.

When a smart contract initiates a transaction transferring funds, the benefits are self-evident for all parties involved. Enhanced transparency makes life easy for auditors.

Any adverse conditions or mistreatment, whether intentional or unintentional can be identified and mitigated. Continuing the theme of financial inclusion,

those in the developing world have less intermediaries to pay. The above solution can be replicated in many contexts where transparency and traceability is required.

For example, the Cardano Foundation in collaboration with Georgia's National Wine Agency and the Bolnisi Winemakers Association and Scant Trust created a solution on the Cardano blockchain

to ensure the quality and authenticity of Georgian wine. Mohammed Alampi, head of Firearms and Toolmark section of the Dubai Police explained at the Card Summit 2023,

how blockchain technology is helping combat organized crime by enabling shared transparent data for tracing firearms across borders. Any process where there are disparate data sources can

benefit from blockchain, healthcare is an obvious candidate for such a solution. As digital health records can be stored and shared with high security assurances,

advancements in zero knowledge and private smart contracts mean healthcare information, data management systems can potentially shield confidential information while still availing

of selective disclosure when necessary. Hospitals today typically contain information siloed across different data systems. With the use of blockchain

and decentralized identifiers, DID patients and healthcare providers can control what they share and with whom.



Quiz question:
![[Pasted image 20260518044845.png]]
Correct Answer: **Midnight**




topic finished under the text is the separation line

---


## **Blockchain for Good**
Many businesses now have an ESG (Environmental, Social, and Governance) mandate. Adopting blockchain for their ESG data allows businesses to demonstrate trust, accuracy, and regulatory compliance.

Blockchain's decentralized nature means their ESG reporting is more reliable and also verifiable. Cardano's. Proof of stake protocol (PoS), Ouroboros, provides

and improves upon the security guarantees of proof of work (PoW), but at a fraction of the energy cost. PoS solves the energy consumption challenge faced

by most blockchains today. By leveraging blockchain technology, businesses can ensure that once ESG data is recorded, it cannot be tampered with

ensuring data integrity. This level of transparency and trust in ESG data is missing from traditional ESG reporting methods. The Cardano Foundation has partnered with Veritree

who are the world's first fully integrated platform for tree restoration through blockchain. There is also a Sustainable ADA project

who compiled the Cardano Impact Report 2023, describing how blockchain is recalibrating the way we view value, identity, positive social, and environmental impact.



Quiz question:
![[Pasted image 20260518044939.png]]
Correct Answer: **Environmental, Social and Governance**


The whole course content is finished under the text is the separation line for the Key Takeaways

---




























# Key Takeaways
- A **cypherpunk** is one who advocates the widespread use of cryptography and privacy-enhancing technologies as a means to social and political change.  
      
    
- For code to run on a computer, it first needs to be translated into **machine code** by a compiler. The computer can digest machine code much easier than a high-level programming language. If a language is very ‘high-level’ it may need to be translated into an intermediate representation before it can be translated further into the lowest level 1s and 0s the computer executes.   
      
    
- **Decentralized identifiers (DIDs)** allow you to identify yourself without using a central authority. DIDs function with three key components:
    - Blockchain provides a secure, shared network for storing your data.
    - Verifiable Credentials are tamper-proof certificates issued by universities, driving test centres, etc.
    - Decentralized Identifiers are unique universally recognised IDs.  
          
        
- A **domain-specific language (DSL)** is a language specific to a particular application domain like finance or law. A general-purpose language can be used across a wide range of domains.   
      
    
- **Fiat money** - a type of currency declared legal tender by a government. It has no intrinsic or fixed value and is not backed by any tangible asset. In theory, the state can print as much fiat money as it sees fit. ‘Fiat’ means ‘by decree’ … From the Latin for "let it be done," the word fiat is a binding edict issued by a person in command. The strength and credibility of the issuing state is the main factor when it comes to fiat money.  
      
    
- **Fungibility** is about the relationship between two assets. Tokens are fungible with each other if they are interchangeable. For a fiat currency to be a satisfactory means of exchange, it has to be fungible, so a $5 bill is interchangeable with other $5 bills. Non-fungible assets are not interchangeable with each other. For example, two distinct paintings, or two on-chain tokens representing the two real-world paintings. If there are no other assets a token is fungible with, the token is deemed to be unique (non-fungible). It is common for artists, musicians and authors to release limited-edition NFT collections.   
    It can be confusing, as technically there isn't much of a distinction between native assets and NFTs. Unlike fungible native assets, which might consist of millions of interchangeable tokens, an NFT is a single native asset that cannot be re-minted or destroyed, and it exists on the blockchain forever. On Ethereum, this functionality requires a separate standard, ERC721.   
      
    
- **Game theory** is a branch of mathematics concerned with the analysis of strategies for dealing with competitive situations where the outcome of a participant's choice of action depends critically on the actions of other participants.  
      
    
- **Immutability** is a blockchain ledger’s ability to remain unchanged and permanent.   
      
    
- A **Layer 2** blockchain solution sits on top of a Layer 1 solution like Bitcoin, Ethererum or Cardano. Layer 2 protocols use the Layer 1 'parent' blockchain for network and security infrastructure. Layer 2s are typically more flexible in their ability to scale transaction processing. There are generally three types of Layer 2 solutions.    
    - **State Channels** (like Hydra, or the Lightning Network on Bitcoin)
    - **ZK Rollups**
    - **Optimistic Rollups  
          
        **Both ZK and optimistic rollups collect off-chain transactions into a batch, then submit them to the Layer 1 blockchain as one transaction.  
          
        

- A **Zero-knowledge (ZK)** rollup is built on top of the existing Layer 1 blockchain to make the transactions faster, cheaper, scalable, secure, and private by not disclosing everything while transacting with the verifier. The problem with many other Layer 2 solutions is that they are not secure enough. There is a trade-off where they focus more on scalability, which can leave them open to exploits. ZK rollups are so powerful as it’s much faster to prove you know the answer, rather than doing the computing to get the answer.   
      
    
- **Optimistic rollups** are less secure than ZK Roll-Ups but offer greater flexibility because they don’t require everything to be encoded in a ZK circuit. In contrast to ZK rollups where you prove everything is correct, you are just proving dishonesty (with Fraud proofs) as required. As the name suggests, you optimistically presume transactions are valid, or use fraud proofs to prove false transactions within 7 days.  
      
    
- **ZK rollups** are more scalable as they consume less blockchain resources compared to Optimistic rollups. ZK rollups are difficult to implement today, mainly because they take time to compile and can slow down your dApp. This is improving every year, however, and it is a hot research space.  
      
    
- **Liquid democracy** is a form of collective decision-making, with elements of direct democracy and representative democracy meshed together through the use of software. Voters either vote on issues directly, or delegate their voting power to a trusted third party.   
      
    
- **Multisig** is where a transaction requires multiple signatures before it can be executed. It is usually used to ensure more security for important transactions, instead of a single-signature transaction.  
      
    
- A **node** on a blockchain is just one of the servers, or computers, that collectively run the blockchain's software. This network allows the blockchain to validate transactions while keeping the network secure in a decentralized fashion.  
      
    
- In a blockchain context, a **P2P (Peer-to-peer)** network that acts as a decentralized ledger. In this decentralized peer-to-peer system, each computer holds a complete copy of the ledger and keeps verifying its authenticity with other nodes to ensure data accuracy.  
      
    
- The term **Opinionated** software relates to the level of guidance and structure a software solution provides. An opinionated solution usually comes with a predefined set of conventions, best practices and design patterns. It shephards developers in a certain direction, which can speed up development but can sometimes limit flexibility.  
      
    
- **Plutocracy** is something governed by the wealthy  
      
    
- **Programmability** is a term used to describe a computer, or blockchain, that is capable of accepting instructions in the form of programming language code. Programming languages have different levels of **expressiveness**. 'Expressiveness' is a measure of how easy it is to write code that's easy to understand, both for the compiler and for a human.  
      
    
- **Proof of X (X can be anything)** consensus mechanisms are simply a means to ensure that all decentralised participants (peers, nodes or miners) willing to secure the network can reach agreement on the correct state of the latest version of a blockchain.  
      
    
- **Security tokens** represent ownership in a company, stocks, real estate or an asset, not unlike traditional securities. They are subject to similar security laws and regulations, and must comply with registration and disclosure requirements. Users typically invest in security tokens hoping for capital gains, dividends, or other forms of income.   
      
    
- A **sidechain** is a separate, standalone blockchain linked to a main blockchain (hence the term ‘mainchain’) usually using a two-way bridge. Tokens and other digital assets can be transferred between sidechains and the mainchain.  
      
    
- A blockchain’s **state** refers to the current status, or snapshot, of all data stored on-chain.  
      
    
- A **state channel** is a blockchain layer 2 solution. It enables a group of users to run unlimited private transactions off-chain. These transactions are not public. The initial and final state of the transactions is all that is recorded on the main blockchain.  
      
    
- **Turing completeness** is a property that describes the ability of a system to compute any possible calculation or program. It is commonly used to describe programming languages.  
      
    
- **TradFi** (short for Traditional finance) is an umbrella term encompassing all aspects of the traditional financial system, ie. banking, the stock market, the bond market, venture capital funds, and hedge funds.  
      
    
- A **utility token** is used to access a particular product or project on the blockchain. Typically, users are incentivized to participate in the network by using the token in return for rewards or discounts. The holder of a utility token does not have any ownership or investment stake in a project.   
      
    
- **Utility tokens** are often confused with security tokens, but they differ in their functions and legal status. Utility tokens are not considered securities as they do not represent ownership or investment in a company or asset. They therefore do not attract regulatory scrutiny.  
      
    
- A **virtual machine (VM)** can be thought of as a digital version of a physical computer.   
      
    
- A **zero-knowledge proof** is where one party can prove to another party that something is true, but crucially avoiding disclosing anything beyond the mere fact that something is true. The classic example is proving to a barman you are over the eligible age to drink beer, but not divulging your address and other personal information.