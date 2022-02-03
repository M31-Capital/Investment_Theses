# Serum (SRM)

* Token Type: Decentralized Exchange
* Circ. Token Supply: 50.0m
* Max Token Supply: 175.0m
* Market Capitalization: $120m
* 24-hr. Volume: $44.0m
* Launch: Aug 2020
* Whitepaper: [Serum Whitepaper](https://docs.projectserum.com/)

## Overview
Serum is a decentralized exchange (DEX) that will be built on the Solana blockchain; integrating a cross-chain gateway between Serum and the Ethereum network that will provide an entry point for current DeFi users to start trading on Serum.

## Background
Serum was created in July of 2020 by a consortium of partners led by the team at FTX. Decentralized Finance (DeFi) has provided massive growth for the crypto industry in 2020 with the introduction of hundreds of new projects providing services such as lending, derivatives, payments, assets, stablecoins, DEXs and more.

Serum aims to provide a derivatives exchange that is more decentralized than its competitors. It looks to solve many of the weaknesses of the current product offerings including speed, usability, centralization, cross-chain functionality, and more.

## Investment Thesis
**Serum takes market share of Decentralized Exchange volume as well as total crypto volume from CEXs.**
* Current growth rates for DEX volume are approximately 150% CMGR. This rate is certainly not sustainable in the long run but there is a higher focus on DeFi and decentralization as a whole for 2020 going forward.  The expectation is that DEXs should continue to slowly gain market share and start positioning themselves as legitimate competitors to centralized exchanges.
**Usability & Cross-chain functionality**
* One of the main issues with DEXs currently is their limitations whether it is their lack of speed in executing transactions, the cost, the technological floor for users, or the limitations in what assets that can be traded on certain DEXs. The Solana-based Serum DEX will have the speed, cost and UX that users expect from a centralized exchange–all while being trustless and noncustodial. It will also support cross-chain swaps allowing a trustless exchange of assets between chains meaning that Serum can utilize Solana’s fast and efficient network while being interoperable with Etehreum’s ecosystem and ERC20 tokens. Additionally, physically settled cross-chain contracts will be implemented meaning synthetic assets like options and derivatives as well as ERC20 or Solana tokenization of BTC or USD will provide even further interoperability with nearly every asset within the crypto ecosystem.
**True Decentralization**
* Most DeFi protocols are not fully decentralized, having a centralized oracle at one or more points - whether it is the team behind the protocol or a liquidation price oracle pointing to centralized exchange APIs. Serum is a fully functional decentralized exchange that has no oracles to centralized price feeds. Serum has a decentralized automated full limit orderbook giving traders full control over their orders unlike Automated Market Making (AMM) seen in the likes of Uniswap and Curve. 

## Industry Outlook
* Thanks to the popularity of yield farming and the DeFi space as a whole, trading volume on decentralized exchanges set record highs in the months of June, July, and August with September projecting to set record highs as well. In August, DEXs accounted for nearly $12B in trading volume, approximately a 266% increase from July ($4.5B). Uniswap and Curve control the largest amount of traded volume. 

![image](https://user-images.githubusercontent.com/96431097/152416058-ddac85a8-f062-4aea-abf3-ec7dbff2f3e3.png)

* Trading volume on DEXs account for only a fraction of total crypto exchange volume however. Today there is approximately $150B of crypto assets traded daily according to CoinMarketCap meaning the monthly DEX volume represents only 8% of the total crypto DAILY trading volume. 

## Competitors
**Traditional Competitors:** 

There are no serious traditional competitors with Serum at the moment. There could be something down the road where traditional market participants like Robinhood, Square, Fidelity, etc could continue to further dive into the crypto market by expanding their offerings. It is something to keep an eye on in the future, but no real current threat.

**Crypto Competitors:**
* Decentralized Exchange Protocols
    * 0x - 0x is a permissionless protocol to facilitate trading of Ethereum based tokens including ERC-20, ERC-721, and other Ethereum standards. 0x is not itself a decentralized exchange, but instead a system of smart contracts that connects liquidity providers and market makers in order to provide exchange functionality in a range of applications. 
* Decentralized Exchanges
    * Balancer - Balancer is a non-custodial portfolio manager and automated market maker that creates customized pools of various assets allowing users to invest these automatically rebalancing pools as well as trade in and out of them. 
    * Uniswap - Uniswap is a decentralized exchange built on Ethereum that utilizes an automated market making system rather than a traditional order-book. Instead of matching individual buy and sell orders, users can pool together two assets that are then traded against, with the price determined based on the ratio between the two. 
    * IDEX - Aurora’s mission is to build a collection of decentralized applications, including IDEX—the first real-time non-custodial trading platform—that together form a distributed financial and banking platform.
    * DYdX - dYdX is a protocol for decentralized margin trading and lending of ERC-20 tokens. It uses off-chain order books with on-chain settlement and enables traders to short-sell tokens, increase exposure by adding leverage or earn interest on deposited tokens.
    * Curve - Curve is a decentralized exchange optimized for low slippage swaps between assets pegged to the same value.
* Centralized Exchanges 
    * Binance - Binance is a digital asset exchange ecosystem offering a variety of centralized and decentralized products and services for efficiently buying and selling blockchain-based coins and tokens.
    * Coinbase - Coinbase is a secure online platform for buying, selling, transferring, and storing digital currency.

![](https://user-images.githubusercontent.com/96431097/152416483-d0a24665-b24b-482f-8d62-6c5e3dacf299.png)

## Recent Trends & Changes
* proposal passed for initiative to fund projects building on Serum through EcoSerum. 2% of all Serum fees will be used to fund new projects through EcoSerum
* Ledger hardware wallet support of Solana
* First grants have been paid to projects building on Serum
* More announcements coming this week
* Jump, one of the largest liquidity providers, announced partnership with Serum
* A lot of new projects and ideas that are being discussed in the community such as borrowing/lending, AMM bots, SUSHIswap support, yield farming tokens, instant messaging protocols, cross-chain lending, synthetic assets, volatility products, etc. A list of ideas here: https://serum-academy.com/en/serum-project-ideas/project-ideas/


## Technology
Serum is natively on the Solana blockchain (as an SPL token) and available on Ethereum (as an ERC20 token). 
Solana is a high-performance, permissionless blockchain that features support for smart contracts and decentralized applications. Solana claims to have created a cryptographically secure and trustless time source called Proof of History. The PoH is a high frequency Verifiable Delay Function (VDF), which requires a specific number of sequential steps to evaluate, yet produces a unique output that can be efficiently and publicly verified. This VDF takes a bunch of data (the input) and spits out a small, fixed-size output. By using this function in a loop, taking a previous output as an input, these pieces of information together represent the data structure that tells how much time has passed. Thus, because of the cryptographically reliable ordering of events encoded in the blockchain, all the nodes are able to receive and trust the order of the structure without having to re-verify them or witnessing them directly. This can potentially reduce the messaging overhead and aims at providing high optimization capabilities.  
At any given time, a system node is designated as a Leader to generate a Proof of History sequence. The Leader is an elected Proof of History generator. It executes the transactions on the current state and publishes the transactions and a signature of the final state to the replication nodes called Verifiers. Verifiers execute the same transactions on their copies of the state and publish their computed signatures of the state as confirmations. The published confirmations serve as votes for the consensus algorithm. Each Verifier node can be elected as a Leader, this is done through PoS based elections.

PoS is designed for quick confirmation of the current sequence produced by the PoH generator, for voting and selecting the next Proof of History generator, and for punishing any misbehaving validators. Bonding and slashing mechanisms are in place to incentivize honest behavior. A proof of malicious vote will remove the bonded coins from circulation and add them to the mining pool. The network could be configured with a minimum Proof of Stake bond size, and a requirement for a single replicator identity per bond.

The system also offers horizontal scaling by mixing inputs from different generators. In theory, this can bring larger scaling opportunities that can reach up to 710,000 tps. Solana competes with existing smart contract platforms, such as Ethereum, providing higher transaction throughput that could enable large scale applications to be built on top of it.

## Token (SRM)
$SRM is Serum’s governance token based on the Solana blockchain but alternatively also has an Ethereum or ERC-20 version.
10 billion SRM was minted as the maximum supply at inception; of which approximately 175m tokens will be circulating initially. This amount is then set to grow by around 15% annually. The Serum community agreed, in an effort to provide long-term health to Serum and the SRM token, to remove the majority of tokens from initial circulation; to be released only if necessary, to provide liquidity to extraordinary demand. This provides us with the initial circulating supply of 50 million tokens (6 million allocated to IEO participants at $0.11/token and 44 million allocated to project contributors and liquidity providers). Greater than 90% of all tokens are locked up long-term. Lockups last for 7 years with none unlocking within the first year.
It gives holders governance power over the Serum ecosystem. While most components in Serum are deemed immutable, some parameters, like future fees, can be modified via SRM governance votes. 100% of the net prices are used to buy and burn the SRM tokens. SRM can be staked and can also be utilized to pay for fees. This gives SRM holders as much as 50% discount on all trading costs. 
Additionally, there is a token, MSRM which essentially is 1 million SRM stacked together. There is a supply cap of 1,000 MSRM. Each MSRM receives slightly more rewards than 1 million SRM would. Holding MSRM provides an additional 10% discount on fees. 
To participate as a node, each node requires at least 10 million SRM (or a combination of SRM and MSRM) and must have at least 1 MSRM.

The SRM distribution is projected as follows:
* 20%: Team and Advisors
* 22%: Project Contributors
* 4%: Locked Seed and Auction Purchasers
* 27%: Partner and Collaborator Fund
* 27%: Ecosystem Incentive Fund

## Governance
SRM is anticipated to have specialized on-chain governance. It will be responsible for setting some important parameters (e.g. fees) but will not have the ability to take actions that would cripple Serum.

The community has already started putting its stamp on the project with nodes voting in favor of a proposal to create an initiative to fund projects building on Serum through EcoSerum. 2% of all Serum fees will be used to fund new projects through EcoSerum

## SWOT Analysis

Strengths 
1. Solana provides a fast, efficient, and scalable blockchain. Something DeFi doesn’t currently have
2. A large group of teams, partners, and nodes already working on the project 
3. Nodes on Serum receive airdrops of all SPL tokens created.
4. Jump, one of the largest liquidity providers partnering with Serum

Weaknesses
1. A lot of competition
2. a lot of their vision is proof of concept at the moment

Opportunities 
1. An extremely large market opportunity
2. Heightened demand for full decentralization
	
Threats
1. Ethereum solving scalability issues
2. More competitors entering the space

## Key Issues & Risks

* Difficult to bootstrap liquidity because it requires sophisticated market makers, requires a well-capitalized insurance fund, and usually requires an external oracle to determine the funding rate
* Building on an unproven and under-utilized network in Solana
* If Ethereum solves its scalability issues, will a blockchain like Solana even be necessary?

## Management & Team
* Serum is a project led by the teams of FTX, Solano, and Alameda Research
* Partners include: 3Commas, AKG Centures, BitMax, Genesis Block, Genesis Global Capital, Kyber Network, Lemniscap, Multicoin Capital, and more.

**Advisors:** 
* Robert Leshner - Founder at Compound
* Calvin Liu - Strategy lead at Compound
* Sam Bankman-Fried - CEO at FTX and Alameda Research
* Sebastian Conybeare - Engineer at Alameda Research
* Gary Wang - CTO at FTX 
* Long Vuong - Founder at TomoChain
* Dan Friedberg - Fenwick & West
* Clement Ip - Partner at Genesis Block
* Dan Matuszewski - Cofounder at CMS
* Shane Molidor - BusDev at BitMax
* Santiago Roel Santos - Partner at ParaFi 

## Nodes
Below is a list of nodes that are currently preparing to provide onchain staking services. Currently, the only place to stake SRM is on FTX. 
3Commas
Age Network
AKG Ventures
AlexDCrypto
Blocto
BitMax
Capsule Mining
Certus
Chainode Tech
DecaMegaDAO
Dokia Capital
EcoSerum
FTX
Kyros Ventures
Genesis Block
QCP Soteria
Sebytza05
Serum Capital
Serum Pool
Serum Stakers
Staking Facilities
Ubik Capital
W3M
Cross Chain Solutions 

## Resources
* [Website](https://www.projectserum.com/)
* [Github](https://github.com/project-serum)
* [Twitter](https://twitter.com/projectserum) 






