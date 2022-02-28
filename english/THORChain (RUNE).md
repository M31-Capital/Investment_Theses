# THORChain (RUNE)

* Token Type: Liquidity Network, Cross-chain DEX
* Circ. Token Supply: 300.75m
* Max Token Supply: 500m
* Market Capitalization: $1.057b 
* 24-hr. Volume: $48.94m
* Launch: Apr 2021
* Whitepaper: [THORChain Whitepaper](https://github.com/thorchain/Resources/tree/master/Whitepapers)




## Overview

THORChain is a decentralised liquidity network aimed to allow permissionless trading/swapping between different blockchains i.e. BTC <-> ETH <-> BNB <-> DOGE <-> SOL and more. Users can trade freely without a 3rd party exchange like Coinbase or Binance, reducing custody, censorship, and counterparty risks. 

## Background

Currently, majority of trading activity on cryptocurrencies are done on centralised exchanges, with $8.6 trillion in total spot volume from January to June 2021 alone. Though blockchains like Bitcoin and Ethereum tout permissionless, trustless and censorship resistant properties, the underlying infrastructure (trading) cannot say the same for itself. This remains as a large attack vector for the digital asset space i.e. China and exchange hacks/insolvency. We have seen how important decentralised exchanges (DEX) are with the rise of Uniswap, allowing self-custodial and trustless swapping of assets on Ethereum. Thorchain seeks to create a cross-chain DEX and liquidity network, bringing trustless swaps between Bitcoin, Ethereum, USDT/USDC, and more.     

Thorchain’s development team remain pseudonymous. 

## Investment Thesis

**Cross-chain Swaps**

We have seen Ethereum concede DeFi market share to alternative, cheaper Layer 1 platforms like Avalanche, Terra, Fantom, Solana – mainly owing to restrictive gas prices. What this does is creates severe fragmentation, and the users are forced to silo their liquidity, which also gives them limited options to move their liquidity. Currently, for users to move their liquidity across various chains, and take advantage of the Dapps that reside on them – they are forced to use 2 options- CEX's and Cross-Chain bridges - and the problem with both of them is centralisation. Using CEX's means trusting the third party to custody your assets, and trust them to have enough liquidity to withdraw it to another chain. Using Cross chain bridges also entails centralisation risks, as all bridges are controlled by multi-sigs and are succesptible to hacks. ($300m Ethereum-Solana Wormhole Bridge Hack).


**Multichain Future**

There are numerous chains that are achieving market demand aside from Bitcoin and Ethereum. We’ve mainly seen activity initially transfer over to Polygon and Solana in the initial parts of 2021 and in 2022 – we’ve seen Fantom and Avalanche emerge as strong alternative DeFi ecosystems. Users who wish to trade or shift funds from different blockchains will go through centralized exchanges or Thorchain. Even L2s such as Arbitrum and Optimism will likely use Thorchain for faster swaps between Ethereum.
 

**Deterministic Price of RUNE**
In any financial market, liquidity begets liquidity. If Thorchain becomes the default layer where users, exchanges, institutions, OTC desks, etc., source their Layer 1 assets such as BTC, liquidity will be sucked out from other CEXes and DEXes into Thorchain. The more trading activity on Thorchain, the more liquidity providers are incentivized to pool onto Thorchain. Since RUNE’s value is tied to at least 3x the value of liquidity provided on Thorchain, RUNE has the strongest value capture in the crypto space. 

 
**DEXes are The Future**

* 24/7, permissionless, censorship-resistant, global trading without an intermediary is the future. 
* Users can trade on DEXes at any time.
* Projects and companies can list their tokens on a secondary market without seeking for permission. 
* Anyone can be a liquidity provider on a DEX and capture yield.

## Catalysts 

* Multichain relaunch
* Thorchain Synths
* Thorwallet mobile application

  
## TAM & Valuation 

* Counterintuitively, RUNE’s addressable market is the $2 trillion worth of digital assets, not the amount of trading volume in the digital asset market. RUNE’s value accrual mechanism makes it such that the marketcap of RUNE will be 3x of liquidity provided on Thorchain. We will explain further in the technology section. 

**Scenario Analyses** 
* Let us simulate the amount of liquidity Thorchain can capture by looking at TVLs of other DEXes or potential percentage of assets locked i.e. 1% of all BTC locked into Thorchain.
    * Calculation of market cap of RUNE will be done by taking TVL/2*3 
    * This is because liquidity providers must sell half their assets for RUNE, hence dividing by 2 first. 
    * For the asset-based calculation, we assume that liquidity providers buy RUNE without selling their ETH or BTC.
![](https://user-images.githubusercontent.com/96431097/152429057-499f6271-f294-4008-a1a5-ac4cead0c7f8.png)
    * These calculations do not take into consideration potential price appreciation of the underlying assets such as ETH or BTC. 
    * If we think ETH will 5x and BTC will 2x, and 1% of each gets locked into Thorchain, its price at its fully diluted supply will be $220.8.
![](https://user-images.githubusercontent.com/96431097/152429131-6311ceca-6d00-4640-9d05-5b7412cd1b84.png)

## Industry Outlook 
* Crypto volumes
    * Cryptocurrency volumes have recently hit all-time highs again with $8.6 trillion in total from January to June 2021, and growth should continue for the foreseeable future. 
![](https://user-images.githubusercontent.com/96431097/152429407-7d4d3089-bee0-46ab-9ec4-3a458b968923.png)
    * DEX volume rose from 0.11% of total crypto volume in 2019, to 8.11% today. 
    Note that total crypto volume have also increase by 10-20x since then. 
    DEXes look poised to grow even further.   

* Crypto marketcap
    * The global marketcap of crypto has also increased by ~20x since 2019, growing from a little over $100b in marketcap to $2 trillion today. 
    * With Bitcoin and Ethereum gaining adoption as days pass, we foresee long-term growth for the asset class. 

## Competitors

**Traditional competitors**

* Robinhood?

**Crypto Competitors** 

* CEX
    * Binance
    * FTX
    * Coinbase
* DEX
    * Uniswap
    * Sushiswap
    * Bancor
    * Chainflip
    * Coin98

## Recent Trends & Changes

* Multichain launch, showing cross-chain swaps are indeed possible with Thorchain. 
* Multichain shutdown due to exploits. 
* Stopped to audit the protocol, hired a white-hat team to protect the protocol, released a bug bountry program, implemented security features like insolvency alerts and in discussions for TVL insurance. 

## Technology

There is currently no efficient way of executing cross-chain swaps trustlessly. Thorchain seeks to solve this by creating a model where node/vault operators are economically incentivised to honestly facilitate cross-chain swaps, similar to how Bitcoin miners are economically incentivised not to 51% attack their network. 

1.	Node operators bond RUNE to earn trading fees on Thorchain. 
2.	These node operators hold the assets that liquidity providers provide i.e. ETH or BTC, and sends out i.e. BTC to a user that swapped his ETH for BTC. 
3.	Since RUNE’s value is tied to the health of the network, malicious behavour from node operators that harms Thorchain will harm the value of their bonded RUNE. 
a.	Why Thorchain cannot use other assets, i.e. ETH, for node operators to bond, is because ETH will still have value if Thorchain is compromised, and there will be little to no negative effect on node operators’ bond.

Why would liquidity providers use Thorchain? 
1.	Liquidity providers on DEXes i.e. Uniswap and Sushiswap, receive trading fees, earning yield on their capital. 
2.	The highest trading volume pairs are BTC/USDT, ETH/USDT, DOGE/USDT, XRP/USDT, SOL/USDT, a majority of which are not supported by Ethereum-based DEXes. These high volume pairs will generate high amounts of trading fees for their liquidity providers.

Trustlessness/Security/Decentralisation ranking
1.	Ethereum/Bitcoin
2.	Ethereum—based DEXes i.e. Uniswap
3.	Thorchain
4.	DeFi applications controlled by multi-sigs 
5.	Centralised exchanges

## Thorfi
* Borrowing
    * LPs can borrowing from their position in order to receive yield from trading fees while unlocking capital. If yields are higher than the interest rate, the loan will be self-repaying.
* Synths 
    * In order to facilitate faster trading and settlement times, Thorchain will implement synths, which are redeemable for RUNE + the underlying asset i.e. 1 BTC synth redeemed for 0.5 BTC and the equivalent RUNE value. 
* Single-sided staking
    * Users are able to stake asset single-sidedly to earn yield i.e. BTC. This will likely draw users which are currently staked at providers such as BlockFi and Celsius. 


## Token (RUNE)

* 3x value of RUNE is required for node/vault operators and liquidity providers to earn yield on their assets, hence the marketcap of RUNE will be at least 3x the value of non-RUNE total valued locked.
* Total supply capped at 500m RUNE and was distributed as follows:
    * Protocol Emissions: 220,447,472 (43.87%)
    * Operational Reserves: 65 million (12.94%)
    * Community Reserve (RUNEVault): 65 million (11.94%)
    * Team and Advisors: 50 million (9.95%)
    * Seed investors: 30 million (5.97%)
    * Private Sale: 70 million (13.93%)
    * IDO: 7 million (1.39%)
    * The sum of these would be 502,447,472. It is assumed that the Thorchain team had burnt the additional 2,447,472 tokens.

**Emission schedule:** 

1.	According to the Thorchain team’s unupdated token release schedule, RUNE’s 10-year emission schedule is as follows:
![](https://user-images.githubusercontent.com/96431097/152430566-cc514b76-4730-4171-86fa-5028ae58c94d.png)

2.	The release schedule incorporates a team and seed token unlock schedule starting from Jul 2021. However, these tokens will only start to unlock when Thorchain achieves mainnet, which seems to be pushed back to early 2022.

## SWOT Analysis

Strengths: 
1.	Tackling a large market gap in crypto.
2.	Best token value accrual mechanism 
3.	Relatively complete protocol, left with bug squashing and battle-testing. 

Weaknesses:
1.	Providing a code-based bridge for ERC20 tokens has multiple attack vectors. Since ERC20 tokens can be created by anyone with limitless programmability, ERC20s may prove to be unworkable for Thorchain due to potential exploits. 
2.	Unknown if liquidity providers will shift to Thorchain. 

Opportunities: 
1.	Regulatory and centralised exchange crackdowns could lead to more users on Thorchain.
2.	Since Thorchain will initially restart only on Binance Chain which has been proven to be stable with Bepswap, the fund could LP on it to farm emission rewards. 

Threats: 
1.	Other competitors creating a more adopted version of cross-chain swaps i.e. Chainflip or Coin98


## Roadmap

There are no dates on Thorchain’s roadmap/milestones, but priority are as follows
1.	Mainnet launch
2.	THORFi 
a.	Synths, savings account, lending and composite assets.
3.	Support an additional 15 chains 
4.	Handover of protocol development and treasury 
5.	Planned obsolescence for the team to decentralised the protocol.

## Key Issues & Risks
* Current volume does not justify current marketcap.
* Unknown timeline to completion of mainnet; other cross-chain services such as Chainflip may steal market share. 

## Token Metrics
![](https://user-images.githubusercontent.com/96431097/152431077-52712118-05fb-4eac-836b-eef9e0634984.png)

## Management & Team
* The Thorchain team is pseudonymous and majority of contributors remain unknown, but certain team members are doxxed such as: 
    * Chad Barraford – Technical Lead
    * Kai Ansaari – Project Lead
    * Leena M. – Project Assistant
    * Jatin Kalra – Project Assistant

## CRYPTO-NATIVE DILIGENCE

**Open-Source Risk (Forking Risk)**
    * There is some element of forking risk, see Swipechain. However, the technical difficulty and liquidity and decentralisation is hard to replicate. 
    
 ## Resources
 * [Docs](https://docs.thorchain.org/)
 * [Gitlab](https://gitlab.com/thorchain)
