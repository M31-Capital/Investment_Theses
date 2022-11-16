# Ethereum Name Service (ENS)

* Current Price: $12.9 
* Token Type:	Governance Token
* Circ. Token Supply: 25.78m (25.78%)
* Max. Token Supply: 100.0m
* Market Capitalisation: $334m
* Launch: Nov 2018
* Whitepaper: [ENS Whitepaper](https://docs.ens.domains/)

## Overview

When we think of the early internet, it became usable to a larger scale of the global population, only because DNS (Domain Name Systems) made machine readable language human readable. We are able to navigate the internet today largely through domain names. We identify popular applications that we use through the website we’re used to using and domain names bridge internet protocol (IP) addresses, that look like “192.168.1.1” to a more human readable name, like www.m31.capital. ENS is a decentralized, web3 naming service that does the same thing, but instead of an IP address being mapped to a website, an Ethereum address (wallets, smart contracts, hashes) can be mapped to a human readable name like “M31Capital.eth”. 

## Investment Thesis 

**Major Improvement in Ethereum’s UX**

With Ethereum’s focus on being the next infrastructure layer for a decentralized global internet, Ethereum Name Service (ENS) will play a critical role in improving the user experience by 100x. To put it simply, ENS just makes interacting with Ethereum a much more simple, less intimidating experience. 

Take a simple payment transaction on Ethereum for example. 

If Alice wanted to send 10 USDC to Bob, she would need to constantly input the 42-hexadecimal string for Bob’s Ethereum wallet (that looks something like this: 0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48), and constantly double and triple check if the inputted address is exactly correct. This is obviously time consuming, and creates a ton of friction with payments. ENS simplifies this. It maps Bob’s complicated, long wallet address to a simple name: Bob.eth. Now all Alice has to do to send 10 USDC to Bob is Input “Bob.eth” and sign her transaction. 

**The Base Social Layer for Ethereum and Beyond**

On Ethereum, (and on applications outside of Ethereum), users need to sign into and access applications with their wallet addresses. ENS provides something like a unified email address: an ENS name. It is likely that a median user’s entire activity on Ethereum (and potentially other chains) will start and end with a single wallet address. Since everything on Ethereum will need a wallet address to connect to it, ENS becomes the base layer for basic identification. Decentralized social media applications will leverage ENS, video conferencing applications will leverage ENS, a user’s in game experience in will leverage ENS, Ethereum messaging applications will leverage ENS, the possibilities are endless. ENS becomes the base social layer for Ethereum. 

<img width="600" alt="image" src="https://user-images.githubusercontent.com/96482943/202221591-e327b033-53ed-40f2-94b1-e5e203d72d38.png">


**Data Privacy** 

Today, we’re used to ‘sign in with google’, or ‘sign in with Facebook’ which we know has improved the UX of web2 by a major factor by abstracting away the need to create multiple user IDs and passwords for every single new website we use. The cost of this however, has been the fact that our user activity across all the websites we use is constantly monitored, mined, and sold to advertisers without any optionality. ENS provides users with the same “single sign-on” experience, without the need for a middleman like Google or Facebook. 

 

**High Growth Product** 

We have seen a large number of users (relatively) pour into the web3 space over the last couple of years, and paired with the NFT boom and a growing application ecosystem, there has been raging demand for ENS domains. As of today, there have been a total of 2.7m ENS domains created, with close to 50,000-100,000 new addresses being added every month. September 2022 saw the largest number of ENS registrations in a single month, with ~437k new names registered. ENS is a product that will scale as usage of Ethereum and the EVM scales. 

## Industry Outlook 

ENS runs a smart contract on the Ethereum blockchain that acts as a registry (a database) of every single ENS name registered and maps it to its rightful owner, who has complete control over the name. ENS can also integrate DNS names (website domains) such that whoever registers the domain name, actually owns it. In the current domain name industry, centralized registries are used (like ICAAN, GoDaddy, Google, AWS) that keep track of what domain names resolve to what IP addresses, ensuring no conflict. 

Centralized Intermediaries come with their own share of problems: censorship and lack of true ownership being the major concerns, while users still have to shell out large amounts of money simply to rent a domain. 

 <img width="500" alt="image" src="https://user-images.githubusercontent.com/96482943/202221694-e6e91649-89dc-4dbc-94d3-bd2f9506108a.png">


The Domain Name Registrar market is worth an estimated ~$50bn and is expected to grow by 15.5% CARG to ~$170bn by 2027. As of Q2 2022, there were ~351 million total domain names registered, up roughly 3% over the last year. 


## Technology 

ENS has two primary components – the ENS registry, and the ENS revolver. 

**ENS Registry** 

This is the core database of the protocol, and is a smart contract that keeps track (maintains a list) of all domains and subdomains that have been registered on the protocol. It keeps track of data like: owner of domains (which wallet address owns the domain), resolver for the domain, and the caching time-to-live for all records under the domain. 

Simply put, the ENS registry is a database that stores all the ENS addresses currently owned, and what wallet address paid for them. 


<img width="277" alt="image" src="https://user-images.githubusercontent.com/96482943/202221825-73eac9f2-0024-4ba3-9221-f5477e1a4393.png">


**ENS Resolver** 

The ENS resolver is a set of smart contracts that are actually responsible for translating the 42-hexadecimal string of characters into their linked human readable names. As long as smart contracts implement relevant standards, they can act as resolvers. 

 <img width="453" alt="image" src="https://user-images.githubusercontent.com/96482943/202221904-9a710dbb-3e95-4aad-94ea-71b39dd531e6.png">


When looking to find a wallet address that corresponds with its linked ENS name, the registry contract is queried for the resolver for that ENS name, and then that specific resolver is queried to get the linked address. 

**Getting an ENS Domain**

Setting up an ENS domain is something everyone beginning their crypto journey should do, truly establishing their on-chain identity. Here’s how: 

1.	Search for the domain or subdomain name of your choice (ex: alice.eth) on the ENS website
2.	If it is available, you can choose the period for which you want to register the ENS for (no limit), and pay a small fee in ETH based on the registration period. (Fee for a 10-year registration is 0.027 ETH, roughly around ~$50)
3.	The protocol will then assign the domain to the address you connected to the dApp with. 
4.	Alternatively, ENS domains are NFTs, and you can buy domain names that weren’t available, on NFT marketplaces like OpenSea, if the minter is willing to sell it to you. 

## ENS Tokenomics 

The ENS token was launched via an airdrop to the community in November 2021. 
Max supply: 100,000,000 ENS
Team and Contributors: 25% - 25,000,000 ENS
Airdrop: 25% - 25,000,000 ENS
Treasury: 50% - 50,000,000 ENS

 <img width="453" alt="image" src="https://user-images.githubusercontent.com/96482943/202222442-48427afb-f17a-4915-ba1d-1302351436da.png">


Token Unlocks: The last major unlock was completed on 07/05/22 with a linear daily unlock vesting schedule for treasury and team tokens set to last until 04/11/25. 

 <img width="453" alt="image" src="https://user-images.githubusercontent.com/96482943/202222510-26e06bff-a8bf-4fb5-b1ee-d473f6ce3884.png">


* Monthly Unlocked Treasury Tokens: 954,826 ENS
* Monthly Unlocked Team Tokens: 414,437 ENS

As of today, only ~0.8% of team and treasury tokens have been sold so far (or have entered circulating supply)

-	We estimate that the team will sell 10% of their monthly unlocked tokens to fund salaries
-	All the ENS that was distributed to the treasury doesn’t enter circulation and will be used to fund DAO activities. We estimate (aggressively) that 10% of unlocked tokens every month enter circulation
-	By 2025, ENS circulating supply will only increase by ~300bps to 28.172m 

### Token Utility 

Governance over the ENS DAO. Token holders can vote progress the DAO looks to make, while voting on protocol parameter changes. 

### Value Accrual 

There is no quantifiable value accrual mechanism yet for the ENS token, however, there is scope that a ‘fee switch’ could be voted on whereby a share of the protocol revenue may be distributed to ENS holders directly or indirectly. 

## Protocol Metrics

### Usage (Registrations and Renewals)

<img width="452" alt="image" src="https://user-images.githubusercontent.com/96482943/202223075-67a55609-69c6-4f1b-a7c0-52c98518af4c.png">

Total Registrations Since Launch: 2.76m
Registration Growth: +487% YoY 
Renewal Growth: +37% YoY

-	As of Nov 2022, ENS has seen a total of 2.76m registrations, up +487% from 2021 
-	ENS has seen rapid growth over the last year, with monthly new registrations of ENS names increasing 272% each month, on average across the last 12 months. 


### Revenue 

<img width="452" alt="image" src="https://user-images.githubusercontent.com/96482943/202223161-900dc054-6e42-4670-881f-82547156bdac.png">


Total Revenue Since Launch: $81.6m*

Revenue Growth: +203% YoY  

-	The protocol has earned significant revenues for the registration of ENS names, earning 34,941 ETH from registrations and 7,853 ETH from renewals since launch. 
-	The Protocol has built up a significant treasury, which is worth ~$1.27bn. 

*Revenue figure of $81m is the value of $ that a user was willing to pay on the day of ENS registration, accounting for ETH price at that period of time. Since all revenues are paid in ETH – the current $ value of total revenues is ~$55m

## Competitive Analysis 

ENS had the first mover advantage when it came to offering blockchain name services on Ethereum but it isn’t the only protocol that offers this service. Other decentralized naming services like Unstoppable Domains, Handshake Naming Service (HNS) compete with ENS by distributing other blockchain domains like .crypto to users.  

•	HNS – HNS are not exactly domains but are rather, domain extensions and there isn’t 100% ownership guaranteed. HNS runs its own blockchain that uses PoW consensus – meaning its security is far less compared to ENS – which is secured by ETH. 

•	Unstoppable Domains: charge a one-time fee for lifetime registrations, (charges slightly higher upfront fees) but cannot offer the .eth domain name extension – which anyone can get on ENS. While unstoppable offers more or less the same features as ENS, they are controlled by a gatekept corporate entity and are not really an open protocol. Adoption and revenues are far behind.  

<img width="452" alt="image" src="https://user-images.githubusercontent.com/96482943/202224163-d620c9b6-e609-4a76-a59b-d3ff93f21547.png">

## SWOT Analysis 

Strengths:

•	Ethereum continues to remain the chain that on-boards the greatest number of users to DeFi, and as a result that puts ENS in pole position to service as a UX layer for all consumer applications building on Ethereum. 

•	Significantly improves multiple complex aspects of using a layer 1 blockchain today, especially for making payments simpler and user friendly. 

•	Simple, strong business model that generates revenues similar to a SaaS organization.

Weaknesses: 

•	At this point, ENS is not chain agnostic, and it services only Ethereum based users. This could be a hurdle to mass adoption of ENS if the multi-chain thesis plays out as we expect it to, with applications building out across chains and even as stand-alone chains. 

•	ENS adoption is a function of Ethereum adoption as well as consumer applications being built on Ethereum. During tough market conditions, ENS registrations may suffer as not too many new users are onboarding onto these networks. 

•	No clear token value accrual model yet. 

Opportunities:

•	Decentralized social applications like Lens Protocol, Huddle01 and Farcaster can provide the tailwinds required to propel ENS adoption through tough market conditions. 

•	Integrations with centralized exchanges like Coinbase can also pave the path for a large number of users to register ENS names without any of technical complexity involved

•	ENS has a large treasury that can be effectively utilized to develop the protocol to meet the requirements of a large and changing landscape. 


Threats:

•	ENS isn’t the only decentralized wallet name service out there, and faces a tough test of competition from protocols like Unstoppable Domains. 

•	Consumer facing applications are the biggest tailwinds to adoption for ENS, however, if the final state of the consumer application layer happens to be built on Solana or another high-performance chain like Aptos, ENS could rapidly begin to lose market share to native naming services on those chains. 


## Code Audits 

ENS permanent registry smart contract was Audited by Consensys, with all minor and major issues with the code resolved. The entire Audit report can be found [here](https://github.com/ConsenSys/ens-audit-report-2019-02#1-summary)

ENS’ smart contracts can be found [here](https://github.com/ensdomains/ens-contracts)

## Team and Management 

The ENS protocol was initially birthed out of the Ethereum foundation, and spun off into a Singapore based non-profit entity called ENS Labs in 2018.  

The details of the team working on the protocol can be found [here](https://ens.domains/about/)

## Resources

[Website](https://ens.domains/)
[Github](https://github.com/ensdomains) 
[Twitter](https://twitter.com/ensdomains) 
[Docs](https://docs.ens.domains/)



