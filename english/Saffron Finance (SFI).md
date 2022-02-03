# Saffron Finance (SFI)

* Token Type: Liquidity Network
* Circ. Token Supply: 91.7k
* Max Token Supply: 100.0k
* Market Capitalization: 
* 24-hr. Volume: $928.3k
* Launch: Nov 2020

## Overview

Saffron is a protocol for tokenizing on-chain assets, including contracts that otherwise impair access to utilized capital. Tokenized ownership of on-chain assets gives liquidity providers greater flexibility and uninterrupted access to their underlying collateral while enabling leveraged staking and bespoke risk management.

## Background

Existing decentralized earning platforms expose liquidity providers to complex code driven outcomes. Network participants must evaluate an array of catastrophic scenarios where the resulting state could wipe out their holdings or lead to significant impermanent loss. It is hard to anticipate the net effect of extreme market volatility or focused economic attacks. Saffron narrows the set of possible outcomes by giving liquidity providers dynamic exposure.

The first application of Saffron gives liquidity providers the option to select customized risk and return profiles via the use of Saffron pool tranches. Saffron separately tokenizes the future earning stream and the net present value of utilized principal in each tranche. Earnings, based on tokenized holdings, are distributed accordingly across all tranches via payback waterfalls.

## Investment Thesis

**Traditional finance institutions will want exposure to DeFi without necessarily taking on the risk inherent to crypto systems.**

* Interested in high yield DeFi exposure, without having to succumb to the risks of IL.
* Guaranteed APY associated with tranches.

**Retail demands dynamic exposure + fast and efficient trading of fixed and variable yields.**

* Saffron gives LP’s the option to select customized risk and return profiles via the use of Saffron pool tranches. 
* Saffron separately tokenizes the future earning stream and the net present value of utilized principal in each tranche. 
* Earnings, based on tokenized holdings, are distributed accordingly across all tranches via payback waterfalls.

## Catalysts:

* Recent influx of projects w/ investment including Element Finance, Barnbridge, Pendle Finance.
* Volatility from bear-bull markets lead to customized risk management strategies. 

## TAM & Valuation: (Work in Progress)

[BarnBridge Token Terminal](https://www.tokenterminal.com/terminal/projects/barnbridge)

[Santiment](https://app.santiment.net/charts?slug=saffron-finance)

## Industry Outlook 

* With over $18 trillion in negative-yielding sovereign debt in traditional markets, Saffron is creating a bridge to enable the migration of billions in investable assets from the traditional debt and fixed income markets to crypto native capital markets

## Competitors

**Traditional competitors**

* Financial Insurance Companies. 
 
**Crypto Competitors (Tokenized Risk Protocols):** 
* Skyrim
* Barnbridge has more products (smart yield, smart bond, smart exposure, smart alpha)
    * BarnBridge is a risk tokenizing protocol. It aims to reduce the risks associated with DeFi, such as inflation risk, market price risk, and cash-flow volatility risk. By letting users select a risk profile, BarnBridge can redistribute risk via tokenized, liquid tranches
    * BarnBridge competes specifically with SFI’s  5+ planned V2 pools (the Fixed Interest pool) and potentially the multi-asset pool as well (not sure what their plans are for their launch)
    * Barnbridge contracts expire after X amount of time. Also, they are fixed interest, and SFI is insurance with 10X interest multiplier. Their contracts also have a negative interest rate for junior tranche when there is a low compound interest rate.
    * There isn't actually any similarity between the two systems other than the concept of separating high and low risk. The mechanics are entirely different
    * [BarnBridge Dune](https://dune.xyz/0xBoxer/barnbridge)
![](https://user-images.githubusercontent.com/96431097/152413426-ffbd2689-1950-4b23-a367-0ca47e6f64d9.png)
* Element Finance
    * Element Finance is a protocol that enables users to seek high fixed yield income in the DeFi market. Users can access, via the ecosystem and existing AMMs at a discount without being locked into a term, allowing the exchange of the discounted asset and the base asset at any time
* Pendle Finance
    * Pendle is the first protocol that enables the trading of tokenized future yield on an AMM system. We aim to give holders of yield-generating assets the opportunity to generate additional yield and to lock in future yield upfront, while offering traders direct exposure to future yield streams, without the need for an underlying collateral.

## Technology
![](https://user-images.githubusercontent.com/96431097/152413770-20c99515-37a9-4756-8270-5b1edee3c68c.png)
![](https://user-images.githubusercontent.com/96431097/152413790-539afb68-6641-4f4b-86e9-407e124d1c59.png)
[Saffron Finance](https://beta.saffron.finance/portfolio)

**AA Tranche:** LPs adding liquidity to the AA tranche earn less interest but are covered in the case of loss from platform risk. That covered capital comes from the principal and interest earnings of A tranche LPs. AA tranche LPs are are awarded with 95% of the SFI token generation. (Currently merged with S tranche). 

**A Tranche:** LPs adding liquidity to the A tranche earn more interest but lose their principal and interest earnings in case of loss from platform risk. A tranche LPs earn 5% of the SFI tokens generated per epoch. SFI earnings are not included in covering first loss for AA tranche LPs. 

**S Tranche:** The S tranche (currently merged with AA) earns 95% of SFI generated per epoch. The system uses the S tranche to balance the A and AA tranches such that they are always in a perfect equilibrium with each other such that the tranche interest multiplier is maintained at its exact value. For example, with a tranche interest multiplier of 10, the AA:A ratio in a pool is always 10:1.

## Business Model & Revenue Sources:
* Currently Saffron has no fees, in V2 they will have a dashboard available with stats on fees.
* The Saffron protocol in this scenario acts as an escrow service for transfer of risk between A tranche participants and AA tranche participants.
    * Added liquidity, when removed, is used to pay back the initial principal of AA holders before paying the principal and interest of the yield enhanced A tranche.
    * In exchange for this enhanced return, participants of the A tranche must stake Saffron’s native tokens (SFI) to mitigate against failures on the underlying platform (such as Compound, Aave, or Curve).
![](https://user-images.githubusercontent.com/96431097/152414110-560e5c11-26fb-47a2-a0c1-19b2ae1df178.png)

## Token (SFI)
* ERC-20 capped at 100,000 SFI. 
* Tokens are a subsidy for liquidity providers and are awarded via liquidity mining. 
* The first epoch will generate 40,000 tokens. 
* SFI token subsidy is halved every epoch, up to and including epoch 7. 
* Beginning on epoch 8, halving discontinues and SFI are steadily released at a rate of 200 tokens per epoch, until reaching the 100,000 cap or a governance vote to change the emission schedule.
* SFI tokens must be staked before an LP can join the yield-enhancing A tranche. 
* There are no fees in version 1, however, upon introduction of fees SFI staking will entitle stakers to a proportional share of fee revenue. 
* Fees continue to provide incentives when SFI token generation ends. Fees continue to provide incentives when SFI token generation ends.
![](https://user-images.githubusercontent.com/96431097/152414297-773590c0-4d0a-41c2-a7a9-943d302f9680.png)
![](https://user-images.githubusercontent.com/96431097/152414314-4c81dc21-01a8-4797-b3a5-c8ec72e4c22d.png)

## SWOT Analysis

Strengths: 
1.	Partners (Coinbase, Dragonfly, Multicoin).
2.	Strong traction: The Saffron protocol has garnered over $50M in Total Value Locked (TVL) across nearly two dozen asset pools.

Weaknesses:
1.	Unable to see previous Epochs, or any relevant stats on the project.

Opportunities: 
1.	The buying and selling of risk is a critical component of any mature financial stack, with risk tranching being relatively new in defi.

Threats:
1.	Competition, Barnbridge


## Key Issues & Risks
* Saffron smart contracts have not yet been audited and users should exercise caution. Code audits and economic attack vector evaluation are included in the team’s ongoing development timeline.
* Several of my contract interactions kept failing.

## Product Roadmap
* In the first version of the Saffron, capital is only deployed on yield farming platforms, but in later versions Saffron will be able to create dynamic risk selection for LPs by adapting to different types of DeFi protocols
* V3 will enhance Saffron protocol by making tranches modular and further customized via a factory contract

## Token Metrics

![](https://user-images.githubusercontent.com/96431097/152414737-8dc4c8b8-43be-42ec-bf7c-72297296b444.png)

## Management & Team

* Psykeeper

## Crypto-Native Diligence

**Open-Source Risk (Forking Risk)**
* Smart Contracts Not Audited

## Resources
* [Docs](https://beta.saffron.finance/docs)








