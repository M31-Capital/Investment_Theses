![File:Chainlink Logo Blue.svg - Wikimedia Commons](https://github.com/user-attachments/assets/752849ca-85a6-4532-9491-22c01ccad4f0)

[Chainlink (LINK)](https://chain.link/) is a Web3 linchpin that bridges blockchains to the outside world of external APIs, data sources and other offchain resources. As the industry’s first data oracle, Chainlink was the key enabler of “DeFi Summer'' in 2020, but has evolved tremendously in the years since, becoming a one-stop-shop for all Web3 middleware services. Most investors are still unaware of the platform’s full product suite and broader long-term vision, creating an attractive investment opportunity today.*

|  | LAUNCH | ENTRY | CURRENT |
| :---- | :---: | :---: | :---: |
| **Date:** | September 2017 | July 2021 | August 2024 |
| **Price:** | $0.109 | $16.30 | $11.19 |
| **Circulating Market Cap:** | $38.1m  | $7.4b  | $6.8b  |
| **Fully Diluted Market Cap:**  | $109.6m | $16.2b  | $11.1b  |
| **Circulating Supply:**  | 350m LINK (35.0%) | 456m LINK (45.6%) | 608m LINK (60.8%) |
| **Max Supply:**  | 1b LINK | 1b LINK | 1b LINK |

**INVESTMENT THESIS**  
---

Top 3-5 reasons why we need to own this name:  

1. **Web3 is increasingly data-centric and needs a robust, full-service middleware backbone.** 

2. **Market undervalues Chainlink’s multi-layer value proposition.** 

3. **Unmatched partnerships & customers across Web2 and Web3.** 

4. **One-stop-shop middleware platform.** 

**KEY RISKS**  
---

Top 3-5 reasons why this investment will fail: 

1. **Fierce Middleware Competition**

2. **Advancement of ZK and TEE Coprocessors**

3. **Centralization Misconceptions.** 

---
---
### *Table of Contents:*

1. [*PROTOCOL OVERVIEW*](#protocol-overview)

2. [*INVESTMENT THESIS*](#investment-thesis)

3. [*TECHNICAL OVERVIEW*](#technical-overview)

4. [*BUSINESS MODEL & TOKENOMICS*](#business-model-&-tokenomics)

5. [*COMPETITIVE LANDSCAPE*](#competitive-landscape)

6. [*VALUATION & RETURNS ANALYSIS*](#valuation-&-returns-analysis)

7. [*STATE OF THE PROTOCOL*](#state-of-the-protocol)

8. [*KEY RISKS*](#key-risks-1)

9. [*SOURCES*](#sources-1)
---
---
# **1. PROTOCOL OVERVIEW** 
 <a id="protocol-overview"></a> 
 
Smart contracts cannot pull or push data offchain because blockchains are completely isolated, deterministic networks. Chainlink invented decentralized oracle networks to solve this issue and universally bring offchain data onchain. Using Chainlink, Web3 apps can trustlessly access high frequency **data streams and feeds**, enabling novel use cases like automated smart contracts and low-latency DeFi Markets [https://chain.link/data-streams].

Beyond one-way data feeds, Chainlink also pioneered a two-way **Cross-Chain Interoperability Protocol (CCIP)**. CCIP is the foundation for cross-chain ecosystems because it provides secure and efficient data transfer across blockchain networks.  

Finally, Chainlink offers trust-minimized compute like **Verifiable Randomness Function (VRF), Automation, and Functions** enabling reliable, secure, and highly expressive decentralized applications.

![](https://github.com/user-attachments/assets/2432b398-adc6-4ebf-9295-2be696db0dd3)

# **2. INVESTMENT THESIS** 
<a id="investment-thesis"></a>

1. **Web3 is increasingly data-centric and needs a robust, full-service middleware backbone.** Chainlink was the key enabler of DeFi Summer and has pioneered the coprocessing narrative. As of August 2024, Chainlink’s middleware stack is irreplaceable because accurate and reliable connection to offchain data is paramount to Web3’s most used applications. Equally important to historical markets, emerging \- and massive \- sectors like AI will require similar data-enabled infrastructure for onchain agents, RAGs, and LLMs.

2. **Market undervalues Chainlink’s multi-layer value proposition**. Most investors still minimize Chainlink to one-directional data feeds. However, Chainlink’s product suite encompasses L0, L1, and L2 services like cross-chain communication, data-triggered smart contract automation, and confidentiality services for bringing sensitive data onchain. Chainlink addresses many of the critical Web3 infrastructure pain points and accrues value across all of Web3, but the market continues to underestimate the breadth of its product suite. 

![image25](https://github.com/user-attachments/assets/e4460cb1-08a7-474d-86e4-01bc5af1d9c6)

3. **Unmatched partnerships & customers across Web2 and Web3.** As of August 2024, Chainlink partners with over 2150 projects, including giants like AWS, Google Cloud, T-Mobile Systems, Linea, and Rocket Pool, and supports over 330 blockchain protocols. Chainlink has long-standing relationships in traditional finance as well, working with industry giants like SWIFT, Fidelity, and DTCC since 2017\. 

4. **One-stop-shop middleware platform:** Once integrated with one Chainlink service, such as data feeds or automation, protocols can seamlessly add services like CCIP without new trust frameworks. This simplifies integration for developers and institutions, making Chainlink a versatile and scalable solution for various blockchain applications, and allows the platform to benefit from strong network effects. 

# **3. TECHNICAL OVERVIEW** 
<a id="technical-overview"></a>

## ***Data Feeds***

Chainlink Data Feeds uses a Decentralized Oracle Network (DON) to connect smart contracts with high-quality, tamper-proof data. The network architecture involves multiple independent nodes pushing data from various offchain sources and coming to a consensus on the most accurate data point before delivering it to a smart contract. Contrary to popular belief, ***Chainlink is more of an integrated SDK than a single network. Users can interoperate across its middleware products without having to worry about single points of failure or incremental trust assumptions.*** 

Data feeds are protected against Sybil attacks through reputation-based node selection and staking mechanisms. Nodes are financially incentivized to provide accurate data, as malicious behavior can result in the loss of staked assets. Additionally, data transmission is secured using cryptographic proofs, ensuring that data remains tamper-proof during transit.

**Proof of Reserve (PoR):** Chainlink uses DONs for PoR, which verifies that offchain reserves have sufficient collateral. PoR attests to cross-chain and offchain asset availability, ensuring that assets claimed to be held in reserve by various financial institutions or stablecoins are indeed available. This is particularly important for centralized exchanges (CEXs) and centralized DeFi (CeDeFi) who have an unfortunate history of fraudulent activities and financial mismanagement. 

By offering real-time data aggregation of offchain reserve assets, PoR supports trusted reserve reporting, prevents fraudulent practices such as fractional reserve banking, and provides cryptographic proof that customer deposits are fully backed.  Additionally, PoR aids in regulatory compliance by helping these companies meet transparency and solvency requirements, protecting them from legal issues and enhancing their reputation. Its real-time monitoring capabilities also help prevent liquidity crises during events like "bank runs," where many users attempt to withdraw funds simultaneously.

Chainlink nodes in the DON are responsible for conducting regular audits of reserve assets, checking the balances held by institutions and reporting the findings onchain. Transparency is a key feature, as the results of these audits are publicly accessible onchain, allowing users to independently verify the reserve status. This transparency fosters trust in the financial institutions and assets backed by these reserves onchain. Taking this a step further, automated verification allows smart contracts to automatically trigger actions based on the PoR feeds. For example, if the reserves fall below a certain threshold, the smart contract can halt operations or notify stakeholders, ensuring real-time risk management.

![image12](https://github.com/user-attachments/assets/df37c477-3d00-44f8-9667-fe708a27da11)

### ***Data Streams***

Chainlink Data Streams provide low-latency delivery of offchain market data that can be verified onchain. With Chainlink Data Streams, dApps have on-demand access to high-frequency market data backed by a decentralized, fault-tolerant, and transparent oracle network. 

**Pull-Based Oracles:** Unlike push-based oracles (Chainlink’s Data Feeds), Data Streams allow applications to *pull* data by checking if certain thresholds are met. Push-based oracles deliver data onchain even when it may not be immediately required, while pull-based oracles provide data more efficiently by retrieving and verifying it only when needed. For example, a decentralized exchange can retrieve a Data Stream and validate the data onchain during trade execution.

![image21](https://github.com/user-attachments/assets/983ba208-1995-4bc1-8c42-2eb66fcb388d)

The Data Streams API services use an active-active multi-site deployment setup, ensuring high availability and robust fault tolerance. This architecture is deployed across multiple distributed and fully isolated origins, ensuring fault tolerance. 

Recently, social media has spread false reports of decentralized oracle competitors outpacing Chainlink in Data Streaming speeds. However, in an August 2024 speed analysis conducted by Chaos Labs (independent third-party Oracle testers), Chainlink’s Data Streams performed considerably better than Binance, Pyth, and Redstone. 

**Streams Direct:** Developers can connect to offchain APIs or WebSocket connections for dynamic updates from the Data Streams Aggregation Network. On-chain smart contracts can then verify these reports, allowing for use cases such as displaying indicative pricing offchain on front ends or settling trades onchain.

## ***Cross-Chain Interoperability Protocol (CCIP)***

CCIP is an independent node network that acts as a secondary validation service for data and token transfers across blockchain networks. CCIP’s functionality can be categorized into three main capabilities: 

1. **Arbitrary Messaging**: Developers can send arbitrary data (encoded as bytes) to smart contracts on different blockchains. This capability enables complex, multi-step tasks, such as rebalancing indexes or minting NFTs, by facilitating detailed and specific instructions sent along with the data.

2. **Token Transfers:** CCIP enables secure and effortless EVM token transfers via lock-and-mint or burn-and-mint mechanisms. CCIP has built-in security features like rate limits and audited token pool contracts that abstract development complexity and boost composability. CCIP enables L2s like Mode to support cross-EVM capabilities, eliminating liquidity silos and unlocking secure cross-chain transactions. 

3. **Programmable Token Transfer**: Programmable token transfers combine token transfers and arbitrary data messaging into a single transaction. For instance, tokens can be sent to a lending protocol with specific instructions on their use, such as utilizing them as collateral for a loan. This enhances the flexibility and utility of token transfers in cross-chain interactions.

 **Lane Architecture:** CCIP uses one-directional pathways called lanes to coordinate data transfers between source and destination blockchains. For clarification, Ethereum Mainnet to Polygon Mainnet and Polygon Mainnet to Ethereum Mainnet are two separate lanes. Each lane is composed of two OCR (Off-Chain Reporting) and DON committees:

1. **Committing DON**: Monitors and commits transactions on the source chain.

2. **Executing DON**: Executes the corresponding transactions on the destination chain.

 **DON Orchestration:** In CCIP, the DON committees provide reliable method for monitoring, verifying, and transmitting data between source and destination blockchains. During each round of consensus, participants in the DON agree on an observed data value, resulting in a report attested by a quorum of participants. One of the nodes transmits this report onchain in a round-robin fashion, ensuring no single participant is solely responsible for every transmission.

**Risk Management Network:** The Risk Management Network provides is the secondary validation layer parallel to the primary CCIP system that uses the DON to verify both offchain and onchain components.

* **Offchain Risk Management Nodes**: These nodes continuously monitor supported chains for abnormal activities and independently verify the Merkle roots of committed messages. If the reconstructed Merkle root matches the committed root, the node blesses it; if discrepancies are found, the node curses the system.

* **Onchain Risk Management Contracts:** These contracts exist for each destination chain, tracking votes for blessing or cursing based on set thresholds. They maintain details of authorized nodes and their respective blessing and cursing weights.

* **Blessing Procedure**: When a Risk Management node blesses a Merkle root, the contract aggregates the blessing weights. Once the combined weights exceed the threshold, the Merkle root is considered blessed.

* **Cursing Procedure**: Nodes vote to curse by assigning a random 32-byte ID to each vote. If the total cursing weight exceeds the threshold, the system is considered cursed, pausing CCIP operations on the affected chain until the issue is resolved.

![image3](https://github.com/user-attachments/assets/c1150e7f-9a79-4155-95ea-72d562c84ec5)


## ***Automation***

Chainlink Automation allows developers to automate smart contract executions based on predefined conditions like time-based triggers and custom logic instead of manual intervention. Automation boosts the efficiency, customization, and reliability of smart contracts, which can now trigger transactions, rebalance portfolios, and execute complex trading strategies, all based on offchain data. 

Chainlink uses a decentralized Automation network to monitor blockchain and external conditions that will trigger smart contract executions. The individual nodes in the Automation network determine which triggers have been met, come to consensus, and then cryptographically sign a report to start the triggered task.

![image26](https://github.com/user-attachments/assets/493cd625-8e86-4a2a-aeb0-89e9d8eb841f)

**Streams Trade:** By combining Data Streams with Chainlink Automation, decentralized applications can automate trade execution, mitigate frontrunning, and limit bias or adverse incentives in executing non-user-triggered orders. This setup allows for seamless integration and robust performance in DeFi trading applications.

An example of Streams Trade is  Beefy Finance, a decentralized yield optimizer platform that integrates Chainlink Automation to automate yield harvesting functions across over 700 yield pools on BNB Chain and Polygon. Streams Trade eliminates the need for manual intervention or centralized bots, ensuring that yield is harvested promptly which maximizes compounding efficiency Streams Trade also enables  automated trade execution and reduces frontrunning on Beefy Finance. 

## ***Functions***

Chainlink Functions is a trust-minimized compute infrastructure allowing smart contracts to fetch API or external data and then run verifiable, custom computations. The process begins when a smart contract, known as the consumer contract, sends a request to the FunctionsRouter contract. The FunctionsRouter manages subscriptions and serves as the entry point for these requests.

Once the request is received, the FunctionsCoordinator contract emits an OracleRequest event that is picked up by the DON. The oracle nodes in the DON execute the provided source code in a secure, serverless environment, with each node running the computation independently and returning its results. The Chainlink OCR protocol then aggregates these results, ensuring that the final response is trust-minimized and resistant to manipulation. This aggregated response is sent back to the FunctionsCoordinator, which then relays it to the consumer contract via a callback function.

![image20](https://github.com/user-attachments/assets/635b3c8f-8349-41c6-a8db-55defdea4a44)

To further enhance security, Chainlink Functions supports the inclusion of encrypted secret values in requests. Using threshold encryption, these secrets can only be decrypted by a multi-party process involving several DON nodes, ensuring that sensitive information such as API keys remains protected throughout the computation process. Additionally, developers fund a subscription account with LINK tokens to pay for requests, streamlining the payment process and ensuring that consumer contracts do not need to hold LINK directly. 

A typical example of Chainlink Functions is compliance for onchain financial protocols. For instance, a smart contract can act as a vault for depositing and withdrawing funds. Before executing these transactions, the contract can use Chainlink Functions to call the Chainalysis API to check if a user's wallet meets compliance requirements, such as being free from illicit activity. This ensures that only compliant transactions are processed, enhancing the security and legality of onchain financial operations.

## ***Verifiable Random Function***

Chainlink VRF (Verifiable Random Function) is a tamper-proof and cryptographically verifiable random number generator for smart contracts on Arbitrum, Avalanche, BNB Chain, Ethereum, and Polygon mainnets. When a consumer contract requests randomness, it sends a request to the VRF Coordinator contract, which then forwards it to Chainlink's VRF oracle nodes. These nodes generate a random value and a cryptographic proof using a seed value from the request. The VRF Coordinator aggregates and verifies these proofs onchain to ensure integrity and fairness, then returns the final random value to the consumer contract via a callback function.

![image8](https://github.com/user-attachments/assets/a0d5c7a7-8ce4-491c-a420-be31ada09ee1)

Many decentralized games and esports platforms rely on Chainlink VRF for in-game random number generation, such as loot drops, enemy encounters, or procedurally generated game elements. VRF adds much-needed depth and excitement to the decentralized gaming experience, making it more engaging for players.

Chainlink released VRF v2.5 in April 2024 which updates wrapper and interface contracts. This makes it an essential tool for applications relying on unpredictable outcomes, such as blockchain games, NFTs, and consensus mechanisms, providing both security and flexibility for developers.

Chainlink VRF v2.5 introduces two methods for requesting randomness: subscription and direct funding. The subscription method allows developers to create a subscription account funded with LINK or native tokens, supporting multiple consumer contracts and calculating costs post-fulfillment to reduce gas overhead. This method is ideal for regular requests. 

The second method is the direct funding method, which requires consumer contracts to pay directly for each random request. This is suitable for infrequent, one-off requests, with costs estimated and charged at the request time.

![image1](https://github.com/user-attachments/assets/a9ee2d0b-32b9-40f0-ba49-524494c4cda0)

## ***DECO***  

### 

DECO is a privacy-preserving oracle protocol that allows users to prove information about their web sessions using zero-knowledge proofs (ZKPs). DECO verifies data provenance by verifying information and sessions from TLS-compatible web servers while maintaining user data confidentiality. For example, a  user can demonstrate that he accessed his private account report from the bank's website and that his balance exceeds a specific amount. However, he does not disclose any other details from the report, such as his account number or exact balance.

### 

DECO's architecture consists of three main components: the DECO Prover, the DECO Verifier, and TLS-compatible web servers. The DECO Prover runs on the user's device or in a secure environment and generates ZKPs to prove facts about web sessions without revealing sensitive data. A decentralized oracle network operates the DECO Verifier and verifies the authenticity of data using ZKPs provided by the DECO Prover. TLS-compatible web servers serve as data sources, while DECO's backward compatibility with TLS ensures that no modifications are required.

The DECO Prover interacts with TLS-compatible web servers to retrieve data, generates ZKPs to prove facts about the data and sends these proofs to the DECO Verifier for verification. The DECO Verifier validates the ZKPs and attests to the authenticity of the data without ever seeing the actual data itself. This architecture allows DECO to provide privacy-preserving data verification while maintaining compatibility with existing web infrastructure, which makes it easier to integrate various data sources and applications.

As of August 2024, DECO is in the developmental and testing phases. At the IC3 Hackathon, Chainlink introduced the DECO Playground, which allows partners to test and provide feedback to help refine the product before mainnet. 

![image10](https://github.com/user-attachments/assets/568418ca-65db-4e20-a491-4dc3bcfe15ff)

## ***BBCA (Byzantine Broadcast with Commit-Adopt)*** 

Chainlink's BBCA is another product in development set to speed up and simplify DAG (Directed Acyclic Graph) consensus mechanisms. Thanks to its unique Commit-Adopt and Byzantine Reliable Broadcast (BRB) architecture, BBCA reduces the time it takes to reach consensus by reducing the number of network trips needed.

BBCA-Chain, the protocol built on BBCA, allows non-leader blocks to be transmitted independently and in parallel, similar to Ethereum's "uncle blocks." It uses a causally-ordered BRB with an active Commit-Adopt feature, letting nodes verify if they've locked onto a value without extra communication. This keeps the process efficient while ensuring strong consensus.

The BBCA-Chain forms a backbone of leader blocks that can commit independently without needing extra votes or layers, speeding up consensus decisions and making the process more reliable. As Chainlink continues to refine BBCA, it could significantly enhance the efficiency of blockchain consensus, making it a powerful tool for high-performance decentralized applications.

In DeFi, where rapid and secure transaction processing is critical, BBCA-Chain can reduce latency and improve the efficiency of smart contract executions. BBCA will become integral to the Chainlink middleware stack, enabling smoother user experiences and better scalability across Web3. 

<a id="business-model-&-tokenomics"></a>
# **4. BUSINESS MODEL & TOKENOMICS** 


***LINK Tokenomics***

LINK has a max supply of 1 billion tokens, and as of August 2024, approximately 608 million LINK tokens are in circulation. Each year, roughly 7% of the total supply of LINK tokens are released. In the initial distribution, 35% of LINK tokens were sold to the public. 30% is held by Chainlink for further development, and the remaining 35% is gradually emitted to Node Operators. 

<img width="794" alt="image6" src="https://github.com/user-attachments/assets/853711c7-9d05-48ba-b773-1ab4e1422990">

<img width="665" alt="image15" src="https://github.com/user-attachments/assets/019f6ab6-2d40-447c-a7ab-0d6a0d360b3f">

**Token Utility**

* **Payment for Services:** LINK is used to pay for Chainlink’s middleware services, including data feeds and streams, VRF, and cross-chain services. 

* **Staking:** Node operators stake LINK tokens as collateral to ensure the honesty and reliability of data, with slashing penalties for malicious behavior. 

* **Revenue share:** Holders can delegate their tokens to supply-side contributors in order to enhance security and participate in network revenue share. 

![image24](https://github.com/user-attachments/assets/ddc2577a-38c6-4709-8a50-07bab2e7df4f)


# **5. COMPETITIVE LANDSCAPE**
<a id="competitive-landscape"></a>

## ***Decentralized Oracle Providers***

Chainlink stands as the leading decentralized oracle network, offering secure, reliable, and customizable Web3 data solutions. Unlike competitors like Band Protocol, API3, DIA, and Pyth Network, Chainlink provides a comprehensive suite of services, including CCIP, verifiable random functions, off-chain compute & data retrieval, and reserve asset monitoring. Users are not forced to adopt additional trust assumptions when adding incremental Chainlink services. So, while competitors may offer specific features, none match Chainlink's full-suite data solution, extensive ecosystem, and proven track record, making it the industry standard for decentralized oracles services. 

|  | Chainlink | Band Protocol | API3 | DIA | Pyth Network |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **Security** | High | Medium | Medium | Medium | High |
| **Scalability** | High | High | Medium | High | High |
| **Incremental Trust Assumptions** | No  | Yes | Yes | Yes | Yes |
| **Customization** | High | Medium | High | High | Medium |
| **Cross-chain Support** | High | High | Medium | High | High |
| **Off-chain Computation**  | Yes | Yes | Yes | Yes | Limited |
| **Event-based Triggers** | Yes | Yes | Yes | Yes | Yes |
| **API Connections** | High (any API) | Limited | Limited | Limited | Moderate |
| **Verifiable Random Functions** | Yes | No | No | No | No |
| **Autonomous Reserve Asset Monitoring** | Yes | No | No | No | No |
| **First-Party Oracle**  | Yes | Yes | Yes | No | Yes |

# **6. VALUATION & RETURNS ANALYSIS**
<a id="valuation-&-returns-analysis"></a>

## ***Relative Valuation***

Considering Chainlink’s expansive middleware product suite, we believe that the most comparable protocols are L0, L1, and L2 ecosystems that support rich application layers, not isolated oracle providers. This is because Chainlink similarly secures value across the entirety of Web3 and provides services for DeFi, gaming, financial services, climate, insurance, asset tokenization, NFTs and more. The peer group’s average FDV of $71.6B implies **a 6.6x near-term re-rate potential for LINK.** 

Given Web3’s nascency, we can look to Web2 for similar assets in a more mature market as a proxy for LINK’s long-term upside. Given Chainlink’s valuable product suite for all end-markets, we believe the best Web2 comps are broad cloud and enterprise platforms that are end-market agnostic and provide many types of services. The peer group’s average FDV of $1.1T implies **a 100x+ long-term upside potential for LINK.** 

![image19](https://github.com/user-attachments/assets/5f1fa761-0d50-48d1-a51a-cdda8cba0d6e)

## ***Total Addressable Market (TAM)***  

To contextualize our estimate for Chainlink’s total addressable market, we will first consider alternative industry benchmarks for digital assets. In 2021, Mckinsey and Co. estimated that the transaction volume to be disrupted by Web3 is roughly $867 trillion.  

<img width="880" alt="image14" src="https://github.com/user-attachments/assets/e52690c4-caa6-4a6f-af3a-e4b2cf971586">

Similarly, Chainlink estimated that onchain assets **represent over a quadrillion dollar opportunity.** 

![image7](https://github.com/user-attachments/assets/cffd7e03-ed29-411a-8130-22f9e42b65e0)

For our estimation of Chainlink’s TAM, we sum the total Web2 global market valuations across asset classes and then forecast out to 2030\. For annual growth, we will use inflation as a conservative rate  assumption. Global inflation over  the last five years has been looming in the mid-to-high single digits, so we believe 4% is a reasonable annual growth rate forecasted until 2030\. 

<img width="595" alt="image29" src="https://github.com/user-attachments/assets/357d8af7-92a3-454b-a27d-b80a49486e53">

*(Source: International Monetary Fund as of 7/30/2024)*

![image5](https://github.com/user-attachments/assets/be562cae-f797-4912-9abe-087a665fdb20)

Using the estimates from the Web2 market valuations, we forecast **DeFi’s TAM to be $1,186T by 2030\.** To estimate Web3's penetration, we will assume that Web3 holds a 0.1% market share across all assets in 2024 that will continuously increase by 3.5% increments each year. By 2030, this puts Web3 penetration of global financial markets at \~20% penetration by, which seems reasonable for an upside scenario. 

![image13](https://github.com/user-attachments/assets/b9e8a4b8-4b07-4b23-8a40-9ad88cf85fe4)

We can then calculate the money earned by these Web3 applications. McKinsey & Co. estimates that Web3 applications will earn 1%-2% on the value exchange they facilitate. For estimation sake, we will use the midpoint of 1.5%. Because we’re modeling asset value, not transaction volume (which is typically much higher), we believe this assumption is sufficiently conservative.

![image28](https://github.com/user-attachments/assets/d0274409-2d7f-4870-a408-a7ded3ba5acf)

## ***Long-Term Upside Potential***

We can extrapolate one step further to estimate the 2030 upside potential for LINK. From 2020 to 2024, Chainlink has maintained an average market share over 75%. While the competition in the decentralized oracle network space is increasing, Chainlink’s product suite is growing rapidly, boosting user stickiness and network effects. In contrast to increasing competition, we estimate Chainlink will maintain a market share of 70% until 2030\. 

<img width="710" alt="image2" src="https://github.com/user-attachments/assets/877eacc9-c9f7-4bf3-8522-462eac408d4b">

*(Source: Defi Llama as of 7/30/2024)*

![image17](https://github.com/user-attachments/assets/6a00ed2b-275b-4112-8a99-bb8f78f000ec)

To estimate Chainlink’s future revenue, we will assume similar take rates to B2B Web2 services like Stripe (2.90%), Visa (2.29%), Paypal (3.49%) or Mastercard (2.24%). This gives us a range of potential take rates for Chainlink of 2.5% to 3.5%, so we will use the midpoint of 3%. Looking at integrated product suites like AWS in Web2, our static take rate is conservative. Simply put, as users onboard with more Chainlink products, their total take rate will increase. 

We can also assert the following statement about Chainlink’s contribution margin:  

Staker profit (contribution margin) \= Chainlink revenue \- supply-side costs (depends on specific product/service)

Typical software companies have 40% EBITDA (cash flow) margins, but 80-90% gross margins (similar to contribution margin), so we assume 70% for LINK stakers. Margin has been a contentious issue in the past for Chainlink, with critics pointing to its history of customer subsidies and low profitability. However, we don't believe that early-stage profitability (especially in an emerging industry) should be used to predict the next 5-10 years. As blockchains become cheaper and more efficient, new Chainlink products are adopted, and the industry matures, we believe 80%-90% contribution margins are achievable.

![image22](https://github.com/user-attachments/assets/57e341b5-67a3-4303-b43c-4583e0c2bfd3)

Applying a 20x multiple to 2030 staker cash flow, the model yields an upside target of **$920 (\~85x from today’s price).**


![image30](https://github.com/user-attachments/assets/0d145c6a-edb2-4bfb-adec-993d5ca543d7)

![image16](https://github.com/user-attachments/assets/0691736e-8cc3-4ca4-9a47-b0ae11c9d10b)


# **7. STATE OF THE PROTOCOL**
<a id="state-of-the-protocol"></a>


 ***Chainlink Traction***

As of August 2024, there are more than 2,150 projects and 2,570 integrations in the Chainlink ecosystem. Total Value Enabled (TVE), or amount of money transacted using price feeds, is the main metric Chainlink monitors and has steadily increased over the last four years. 

![image11](https://github.com/user-attachments/assets/f1c983e8-1393-4dbc-a97f-d0382c2f98cd)

## ***Chainlink Enabled Protocols & Adoption***

### *Decentralized Finance (DeFi):*

* **Aave:** A decentralized, open-source, and non-custodial money market protocol. Chainlink provides secure price feeds to ensure the accuracy of collateral valuations and loan liquidations.

* **Compound:** An Ethereum-based money market protocol for lending and borrowing assets. Utilizes Chainlink oracles to fetch real-time price data for secure lending and borrowing.

* **Venus:** An algorithmic money market system on Binance Smart Chain. Relies on Chainlink for reliable price data to manage loans and collateral.

* **Synthetix:** A platform for trading synthetic assets. Employs Chainlink's price feeds to support the trading of synthetic assets with zero slippage.

* **Alchemix:** A future-yield backed synthetic asset platform. Integrates Chainlink oracles to ensure the stability and accuracy of future-yield backed synthetic assets.

* **Lyra:** An options trading platform on the Optimism network. Uses Chainlink price feeds for options pricing and settlement.

* **Opyn:** An open, decentralized options platform. Utilizes Chainlink for capital-efficient options protocols with automated settlement.

### *Enterprise and Institutions:*

* **Fidelity International and Sygynum:** Fidelity now offers Net Asset Value (NAV) onchain through Chainlink’s oracle data feeds and Sygnum’s onchain representation of Fidelity’s Institutional Liquidity Fund. 

* **ANZ:** A major banking institution exploring Chainlink's CCIP for secure and interoperable tokenized asset management. Uses Chainlink's CCIP for tokenized asset management in banking.

* **Telefónica:** A global telecommunications company partnering with Chainlink to enhance SIM card security using Web3 technology. Partners with Chainlink to enhance SIM card security using Web3 technology.

* **SWIFT:** A global provider of secure financial messaging services collaborating with Chainlink to test blockchain interoperability for tokenized assets. Collaborates with Chainlink to integrate services for blockchain interoperability and tokenized assets. 

* **DTCC:** Uses Chainlink to enhance blockchain-based solutions for financial institutions via secure and reliable financial data transmission.

### *Stablecoins and Pegged Assets:*

* **Fei Protocol:** A decentralized, scalable, reserve-backed stablecoin. Uses Chainlink oracles to maintain the stability of its reserve-backed stablecoin.

* **Liquidity:** An interest-free lending platform that enables the minting of the LUSD stablecoin. Employs Chainlink's ETH price feeds to support interest-free loans and the LUSD stablecoin.

* **Paxos:** A brokerage and custody platform providing tokenized real-world assets. Leverages Chainlink to tokenize real-world assets, providing secure and transparent price data.

* **TrustToken:** A blockchain-agnostic stablecoin backed by USD held in reserves. Utilizes Chainlink oracles for accurate price feeds of USD-backed stablecoins.

* **Wrapped BTC:** A tokenized version of Bitcoin on the Ethereum blockchain. Relies on Chainlink to provide reliable price data for tokenized Bitcoin on Ethereum.

### *Exchanges and Trading Platforms:*

* **dYdX:** A layer 2 decentralized exchange for spot trading and perpetual contracts. Integrates Chainlink for secure and low-cost price feeds on its decentralized exchange.

* **Loopring:** A layer-2 decentralized exchange providing high throughput, low-fee trading. Uses Chainlink oracles to provide high throughput and low-fee trading on its L2.

* **DODO:** A proactive automated market maker that mimics human market-making behaviors. Employs Chainlink's proactive market-making price feeds to mimic human market behaviors.

### *Insurance and Risk Management:*

* **Arbol:** Provides parametric crop insurance for farmers based on weather conditions. Utilizes Chainlink for weather data to support parametric crop insurance.

* **Etherisc:** Offers parametric insurance for real-world events such as flight delays. Relies on Chainlink oracles for real-world event data, such as flight delays.

* **Nexus Mutual:** A decentralized discretionary mutual that provides an alternative to traditional insurance. Uses Chainlink price feeds for decentralized discretionary mutual insurance.

### *Real-World Assets (RWA):*

* **RealT:** A platform for tokenized real estate, allowing users to buy fractions of a property’s cash flows. Employs Chainlink oracles to tokenize real estate and provide fractional property cash flows.

* **CrescoFin:** A tokenized invoice protocol providing interest-yielding insured deposited products. Uses Chainlink for tokenized invoice protocols, ensuring interest-yielding insured deposits.

### *Payment Solutions:*

* **Flexa:** A cryptocurrency payment platform for merchants to accept instant, guaranteed crypto payments. Integrates Chainlink to facilitate instant and secure cryptocurrency payments for merchants.

* **Crypto.com:** A crypto mobile app where users can pay merchants using tokens via a Visa debit card. Utilizes Chainlink for accurate price feeds in its crypto payment and Visa debit card services.

### *Gaming and NFTs:*

* **Bored Ape Yacht Club:** A collection of 10,000 unique Bored Ape NFTs on the Ethereum blockchain. Uses Chainlink VRF for generating random and unique NFTs on Ethereum.

* **Aavegotchi:** A DeFi-powered crypto-collectible game featuring interest-generating NFTs. Leverages Chainlink for interest-generating token-backed crypto-collectibles.

* **Axie Infinity:** A Pokémon-inspired universe where users breed and battle Axies. Employs Chainlink for secure and accurate price data in its Pokémon-inspired universe.

### *Asset Management and Portfolio Optimization:*

* **Set Protocol:** A non-custodial asset management protocol for social trading and indices. Integrates Chainlink for non-custodial asset management and social trading protocols.

* **PoolTogether:** A no-loss savings game where users can win prizes without risking their deposits. Uses Chainlink to provide accurate and transparent prize data for no-loss savings games.

## ***Partnerships***

*Technology Companies:*

* **AWS:** Collaborates with Chainlink for secure cloud data services, simplified oracle node operations, and increased data-availability for dApps. 

* **Google Cloud and BigQuery:** Works with Chainlink to offer diverse data feeds including weather, news, and asset pricing. 

* **Space and Time:** Partners with Chainlink for decentralized data warehousing and secure oracle services for trustless, real time data-queries. 

* **Swisscom:** Provides digital asset pricing feeds through a Chainlink oracle node. 

*Blockchain and Crypto Projects:*

* **AP Oracle:** Chainlink and Oracle partner to help startups monetize blockchain APIs using Chainlink’s oracles. 

* **Binance:** Provides cryptocurrency price data to Binance exchange. 

* **Everpedia:** Uses Chainlink to post verified election result data from the Associated Press. 


<img width="628" alt="image4" src="https://github.com/user-attachments/assets/457d35e5-e0c0-4219-867a-0e5de14686c3">


### ***Leadership & Developer Community*** 

**Sergey Nazarov, CEO:** Sergey graduated from New York University with a B.A. in Philosophy and Management. Before Chainlink, Sergey co-founded SmartContract.com, promoting smart contracts' mainstream adoption, and Secure Asset Exchange, offering secure access to decentralized exchanges. Sergey now serves as a prominent thought leader in decentralized oracle services and through Chainlink, has spearheaded the push towards a data-driven Web3 landscape. 

**Steve Ellis, CTO:** Steve holds a B.S. in Computer Science from New York University. Before Chainlink, Steve co-founded SmartContract.com with Sergey and Secure Asset Exchange. During these ventures, Steve developed smart contracts and pioneered the core architecture behind today’s decentralized exchanges. 

**Chainlink BUILD Program:** BUILD is Chainlink’s incubator program accelerating early-stage startups building with Chainlink. To help developers focus on application functionality rather than infrastructure headaches, Chainlink provides subsidized Oracle services, comprehensive technical support, and community resources. Notable projects from the BUILD program include Space and Time, Krypton, and bitsCrunch, and as of August 2024, the BUILD program has hosted over 100 projects. 

**Chainlink Economics 2.0 and SCALE Program:** Chainlink’s SCALE (Sustainable Chainlink Access for Layer 1 and 2 Enablement) program covers oracle operating costs, such as transaction gas fees for L1s and L2s. As these ecosystems mature, operating costs transition to being covered by dApp user fees, promoting a sustainable economic model. SCALE is part of Chainlink Economics 2.0, which aims to boost data security, reduce oracle service costs, and increase participation from Chainlink stakers. The Chainlink Economics 2.0 scales the next generation of high-performance and data-centric dApps.  As of August 2024, the SCALE Program supports zkSync, CELO, Starknet Avalanche, Metis, Moonbeam, and Moonriver, not to mention price feed support for Base Testnet. 

<img width="771" alt="image23" src="https://github.com/user-attachments/assets/f1f6ee87-9a42-492d-95fe-f77e0458eff0">

***Roadmap***

**Phase 1:** Q3 2024 \- Q1 2025

* Launch CCIP v1.5 on mainnet  
* Deploy Data Streams on Avalanche mainnet  
* Expand DECO Playground to more testers and harden codebase  
* Host global CCIP and Tokenization Bootcamps  
* Collaborate with SWIFT on tokenized asset interoperability

**Phase 2**: Q2 2025 \- Q4 2025

* Implement CCIP Widget UI and SDK  
* Extend Data Streams to more Ethereum L2s  
* Optimize Automation billing and gas controls  
* Enhance Functions with external libraries support


**Phase 3:** Q1 2026 \- Q4 2026

* General Availability for Data Streams  
* Launch onchain billing for Data Streams  
* Expand Data Streams to new chains  
* Integrate Automation with more developer frameworks

# **8. KEY RISKS**
<a id="key-risks-1"></a>


1. #### **Fierce Middleware Competition:** As of August 2024, investors are focusing on integrated infrastructure like Chainlink, drawing in more new entrants and increasing competition. Additionally, many Web3 applications are also ditching the modular thesis and instead are developing their own bespoke middleware solutions. 

   *Mitigants:*

      * Massive competitive moat compared to competitors because of its full product suite with no incremental trust assumptions when adding Chainlink products. 

      * The modular thesis is a long-term battle \- and Chainlink at the helm. Chainlink already supports prominent blockchain projects like Aave and dYdX, not to mention partnerships with AWS and GCS. 

      * The integrated service offerings, BUILD and SCALE programs, and rich developer toolkit makes building with Chainlink the easy choice for developers looking for data functionality. 

2. **Advancement of ZK and TEE Coprocessors:** These technologies pose a real threat to Chainlink by offering alternative solutions for efficient, privacy-preserving data handling. 

   *Mitigants:*

      * Chainlink's architecture allows for easy integration of coprocessors, as evidenced by its seamless incorporation of ZKPs for verifiable computations, privacy-preserving data retrieval, and DECO.

      * Coprocessors have specialized, often isolated use cases as compared to Chainlink’s comprehensive, one-stop middleware solution. 

3. **Centralization Misconceptions**: After Chainlink reduced its multisig signature requirement from 5 to 4 out of 8 signatures, select members of the crypto community voiced concerns about Chainlink’s potential centralization risk. 

   *Mitigants:*

      * The multisig signature reduction \- and other prominent centralization misconceptions  \- were directly addressed and debunked by the Chainlink teams as transient technical changes. 

      * Chainlink consistently increases the number of independent node operators and diversifies the DON through an incentive system. 

      * Chainlink's reputation system tracks node performance, encouraging reliability and deterring malicious actions by making it harder for bad actors to gain significant influence.

# **9. SOURCES**
<a id="sources-1"></a>

* [Website](https://chain.link)  
* [Whitepaper](https://research.chain.link/whitepaper-v1.pdf)  
* [Github](https://github.com/smartcontractkit/)  
* [Discord](https://discord.com/invite/chainlink)  
* [Docs](https://docs.chain.link)  
* [Twitter](https://x.com/chainlink)  
* [Podcasts](https://blog.chain.link/sergey-nazarov-media-library/)
