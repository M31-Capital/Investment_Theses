![Screenshot 2024-09-12 at 1 41 46 PM](https://github.com/user-attachments/assets/ea11e6e6-0170-435c-bc01-f89901a93a1b)

[Marlin Protocol (POND)](https://www.marlin.org/) is a multi-prover coprocessor platform that trustlessly connects smart contracts with Trusted Execution Environments (TEEs) and Zero-Knowledge Proofs (ZKPs) to multiply blockchain processing power and expressivity. We believe Marlin’s current valuation offers an attractive long-term investment upside given the market’s misunderstanding of coprocessors and verifiable cloud services today.

|  | LAUNCH | ENTRY | CURRENT |
| :---- | :---: | :---: | :---: |
| **Date:** | December 2020 | November 2023 | August 2024 |
| **Price:** | $0.28 | $0.010 | $0.014 |
| **Circulating Market Cap:** | $121.2m | $77.8m  | $113.3m  |
| **Fully Diluted Market Cap:**  | $2.8b | $100.0m  | $140.0m |
| **Circulating Supply:**  | 433m POND (4.3%) | 7.78b POND (77.8%) | 8.09b POND (80.9%) |
| **Max Supply:**  | 10b POND | 10b POND | 10b POND |

**INVESTMENT THESIS**  
---

Top 3-5 reasons why we need to own this name: 

1. **Coprocessors will significantly enhance smart contract capabilities.**

2. **Misunderstood coprocessor value proposition.** 

3. **Exciting long-term TAM and investment upside potential.** 

4. **Web3 application stacks need truly decentralized services.** 

5. **teeML is misunderstood by the market and grossly underutilized.** 

**KEY RISKS**  
---

Top 3-5 reasons why this investment will fail: 

1. **Coprocessing Competition**

2. **Lack of Product-Market-Fit**

3. **Lack of brand and coprocessor narrative awareness**
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

Blockchains—and thus smart contracts—are computationally constrained because transactions must be executed and data must be stored across all decentralized nodes. In turn, complex applications like verifiable AI training and inference will always be infeasible on blockchains. 

Marlin uses coprocessing, high-powered offchain computing with concise verifiable onchain attestations, to scale blockchains and enable significantly more smart contract expressivity. Applications can trustlessly use Marlin’s TEE and ZK-verified coprocessing subnetworks to boost throughput and its flexible relay network to transmit data between blockchain networks. Marlin Protocol network components include: 

* **Oyster:** Network of TEE coprocessors offering secure and cost-effective computation services. Users (Web3 applications) can securely rent confidential instances or outsource serverless jobs, enabling a fully decentralized and verifiable cloud infrastructure. 

* **Kalypso:** Permissionless ZK-proof marketplace that outsources proof generation to a network of third-party providers, improving computational integrity and the user experience.  

* **Relay Network:** Enhances blockchain throughput by enabling offchain data access and relay, providing APIs for offchain data, and supporting integration across multiple blockchains.

![image7](https://github.com/user-attachments/assets/1d78f185-fd6b-44f1-bbc0-559d1904597a)

### ***Target Markets and Use-Cases*** 

* **DeAI:** Marlin’s Oyster network allows AI models to auto-scale with demand, maintain data privacy, and ensure model integrity. The processing of inputs and AI models is handled within the TEE, providing privacy and preventing data tampering. After processing, coprocessors create ZK proofs that validate the correctness of the computation without revealing specific inputs or models. These ZK proofs are then uploaded to the blockchain, making them available for decentralized applications to use. This setup is ideal for applications like prediction models, self-governing DAOs, autonomous systems, and credit-scoring models.

  * **Talus Network** uses Marlin’s verifiable compute layer for trustless AI smart agents. 

* **DeFi:** Marlin’s TEE coprocessing enhances decentralized exchanges by reducing transaction latency and increasing throughput. This improvement is crucial for applications such as order book DEXs, automated market makers, and lending protocols, ensuring efficient trade executions and maintaining liquidity. 

  * **Injective** uses Marlin’s low-latency network infrastructure for high-speed trading across their DeFi-focused L1

* **Oracles:** Marlin provides a robust infrastructure for decentralized oracles, ensuring timely and accurate data feeds to smart contracts. This is essential for various blockchain applications that depend on real-time data, including price feeds for assets, event data providers, and weather data services. 

* **Gateways:** Marlin enables fully decentralized gateways that offer secure and seamless access to blockchain networks and cross-chain communication. Applications include cross-chain bridges and decentralized web access through browsers. 

* **Web3 Gaming:** Marlin’s coprocessors create better user experiences for decentralized gaming by lowering latency and boosting throughput. This ensures smooth and responsive gameplay for online multiplayer games, eSports platforms, and blockchain-based gaming applications.

* **Frontends:** Marlin improves dApp frontends by optimizing data transmission between the user interface and the blockchain. This results in faster load times and a more seamless user experience for platforms such as DeFi platforms, NFT marketplaces, and social media dApps.

* **dApp Cache:** Marlin offers a distributed event-driven caching system called Marlin Cache, designed to accelerate and reduce costs for dApps. It caches frequently accessed blockchain data closer to users, significantly improving response times from 230-1500ms down to 5-10ms for cache hits. This system complements existing blockchain API services by allowing deeper geographical distribution of lightweight cache nodes, enhancing performance, and reducing load on origin servers.

# **2. INVESTMENT THESIS** 
<a id="investment-thesis"></a>

1. **Coprocessors will significantly enhance smart contract capabilities**. Marlin uses both TEE and ZK coprocessing to facilitate trustless offchain computation, significantly enhancing smart contract expressivity and enabling chain abstractions. 

2. **Misunderstood coprocessor value proposition.** We believe coprocessors will be the necessary infrastructure for scaling complex Web3 applications, but the market still misunderstands the technology and its implications for all Web3 use cases and end-markets. 

3. **Exciting long-term TAM and investment upside potential.** We believe the coprocessor market can reach over $20 billion by 2030, resulting in nearly 200x upside potential for Marlin long-term*.*

4. **Web3 application stacks need truly decentralized services.** Users can interface smart contracts with coprocessing subnetworks, meaning Web3 services like gateways, relays, and offchain APIs can finally be entirely serverless and self-managed and complete the fully trustless stack. 

5. **teeML is misunderstood by the market and grossly underutilized.** teeML represents the most pragmatic solution to powering onchain smart contracts with offchain LLM processing. It's currently over 1000x faster and considerably cheaper than other coprocessing solutions like zkML and opML.

# **3. TECHNICAL OVERVIEW** 
<a id="technical-overview"></a>

### ***Oyster: TEE Subnetwork***

The Oyster Subnetwork is a collection of hardware-isolated nodes, operating within a TEE and enabling decentralized applications to perform complex computations offchain while ensuring data and process integrity through multiproof verifiability. 

* **TEE**: TEEs are physically isolated enclaves that ensure data and processes remain confidential and tamper-proof, even if the physical machine is compromised. In short, TEEs are completely separate from the operating system and any potential malware which enables secure computation on untrusted TEE systems.  

* **Remote Attestations**: Attestations verify the authenticity and integrity of the code running inside the TEE. It involves generating cryptographic proof that the application has been correctly instantiated in the agreed upon TEE and is executing the expected code, which can be verified by external entities before they interact with the node.

* **Networking**: Oyster nodes facilitate decentralized, secure communication channels through a peer-to-peer network. These channels ensure data integrity and confidentiality during transmission, using secure enclaves to protect against unauthorized access and tampering. Using Marlin protocol's high-performance networking stack, nodes can efficiently handle large volumes of data with low latency and high throughput, ensuring reliable communication between decentralized applications.

### ***Oyster Cloud***

Oyster Cloud provides TEE-based instances that can be rented individually, ensuring high performance and secure end-to-end connections. Users can deploy backends or extend their smart contracts on Oyster with minimal changes. Oyster Cloud also manages auto-scaling and failure recovery, allowing developers to focus on their products without worrying about infrastructure maintenance. 

* **Control Plane:** The control plane monitors events from the overarching JobRegistry smart contract and initiates new TEE-enabled nodes for incoming jobs. This component ensures efficient management and deployment of secure instances, automatically scaling the system based on demand.

* **End-to-end Connections:**  Marlin ensures secure end-to-end connections using specially modified containers within a secure enclave. These containers are isolated from the rest of the system and use virtual sockets for internal communication. To relay TCP traffic securely, Marlin employs custom proxies with specialized IP packet rules (iptables) to control and moderate network traffic. This setup keeps data channels secure and encrypted at all times. 

![Screenshot 2024-09-12 at 1 44 57 PM](https://github.com/user-attachments/assets/a8887654-720f-4454-aef9-ec25a4d3e861)

### ***Oyster Serverless***

Oyster Serverless is an optimized computing platform designed for secure execution of JavaScript and WebAssembly. It uses AWS Nitro Enclaves, Cloudflare workerd runtime, and cgroups (control groups) to match demand for confidential and streamlined code execution. This serverless infrastructure scales automatically based on demand, ensuring applications handle varying workloads without manual intervention. Users can outsource jobs to the serverless pool without the need to rent specific machines, focusing on application logic rather than infrastructure management. This model is cost-effective as users are billed only for the duration of task execution.

* **Security and Isolation within AWS:** Oyster Serverless uses AWS Nitro Enclaves to provide an isolated and secure environment for executing sensitive code. Nitro Enclaves use the Nitro Hypervisor to isolate CPU and memory, ensuring that the parent instance cannot access the enclave's resources.   
    
* **Runtime Environment:** The platform uses Cloudflare's workerd runtime, which is designed to execute JavaScript and WebAssembly securely and efficiently. Workerd provides a production-ready web server environment that can be self-hosted, allowing for flexible deployment options. It supports a wide range of web platform APIs, ensuring compatibility with existing JavaScript codebases and enabling seamless integration with other Cloudflare services.

* **Resource Management:** Oyster Serverless employs cgroups to manage and isolate resource usage among different tasks. Cgroups ensure that each task gets the necessary resources without interfering with others, providing a stable and predictable execution environment. This mechanism also helps in auto-scaling by dynamically adjusting resource allocation based on the current demand, ensuring optimal performance and cost-efficiency.

### ***Kalypso: Decentralized ZK Proof Marketplace***

Kalypso is Marlin's decentralized marketplace for ZK proof generation. It allows applications to outsource ZKPs, enhancing efficiency and cutting costs.

* **Core Smart Contracts:** Kalypso's core smart contracts manage operations within the proof marketplace, oversee the registration of Proof Generators, and handle key registration processes. 

* **Matching Engine:** The Matching Engine ensures efficient pairing of participants within the marketplace. It connects specialized hardware operators with users needing ZKPs, optimizing resource utilization and reducing idle time. The engine's design allows for flexibility, enabling users and operators to prioritize either cost or speed and to join or leave markets as needed, facilitating a dynamic and responsive ecosystem.

* **Markets:** Markets in Kalypso are specialized environments tailored for specific circuits and applications. Market Creators can parameterize each Market to account for unique requirements such as minimum stake amounts, TEE support for private inputs, and recommended proving software. Markets consist of various components, including Proof Generators (for both confidential and non-confidential inputs), Input Verification Enclaves, and Proof Verification Contracts. This modular structure allows for versatility in handling different types of zero-knowledge proof requests and generation processes.

<img style="width: 45%;" alt="image13" src="https://github.com/user-attachments/assets/8d3fd986-da20-4d93-81dc-e2fa6d8b5492">


### ***Relay Network***

The Relay Network is a permissionless and incentivized network built to securely connect blockchains. In effect, Marlin facilitates reliable, low-latency data relays in a completely trustless and privacy-enabled way. 

* **Producers**: Producers introduce data blocks into the network and ensure data is universally available for consumption. They are rewarded based on the speed of their block transmission across the network but can be slashed for invalid block submissions. 

* **Receivers**: Receivers subscribe to and receive data blocks, allowing them to access up-to-date information from the network. Receivers, which can be miners, exchanges and full nodes, pay a subscription fee for data transmission. 

* **Relayers**: Relayers are nodes that transmit the block from the producer to the receiver. These nodes are grouped in clusters, which are rewarded based on the speed of propagation. 

![image1](https://github.com/user-attachments/assets/6e0e9271-9b31-4043-bb9e-583669f135fd)

* **Propagation:** The Relay Network uses erasure coding to split data into chunks, ensuring integrity by allowing reconstruction from a subset of these chunks. Relayers distribute the chunks, and receivers reconstruct complete data blocks from them. A rewards system incentivizes top-performing relayers based on performance metrics and subscription fees, promoting high performance and reliability.

### ***Multicast SDK***

Marlin’s Multicast SDK provides tools for developers to build efficient and scalable applications on Marlin. 

* **Transports:** The SDK includes support for multiple transport protocols, enabling developers to choose the most suitable communication methods for their applications.

* **WASM64 Support:** Marlin supports WebAssembly 64-bit (WASM64), allowing developers to create applications that utilize large memory spaces, which is essential for running complex AI models.

* **Hyper Parallel Processing:** Marlin’s architecture supports parallel processing, enabling large-scale computations without affecting neighboring processes.

* **Endianness:** The SDK supports different endianness formats, ensuring compatibility with various hardware architectures and facilitating seamless data exchange.

<a id="business-model-&-tokenomics"></a>
# **4. BUSINESS MODEL & TOKENOMICS** 

### ***POND Tokenomics***

**Token Supply:** POND has a total supply of 10 billion and an initial total supply of 3.184 billion. As of July 2024, approximately 8.09 billion (80.9%) were in circulation. The tokenomics are designed to ensure network security, governance integrity, and active participation. The token distribution is as follows:

* Ecosystem Development: 31.9%  
* Staking Rewards: 21.8%  
* Private Sale: 17.2%  
* FlowMint: 16%  
* Team and Advisors: 10%  
* Foundation: 3%

<img style="width:45%;" alt="image4" src="https://github.com/user-attachments/assets/5bc805ec-ff19-4c78-b529-db22d3629155">

**MPond:** Marlin also uses a second token MPond for governance. MPond has a total supply of 10,000 tokens, with a conversion rate of 1 MPond to 1 million POND. Users can mint MPond by locking up their POND tokens, granting them governance power to propose and vote on protocol changes. 

This dual-token design features a delayed 6-month bridge from MPOND to POND to ensure economic security and disincentivize malicious parties from quickly acquiring governance rights. However, users can instantly bridge POND to MPOND, creating illiquid and long-term-focused governance. 

MPond and POND Emission schedule post-TGE: 

![image10](https://github.com/user-attachments/assets/1fb8e928-b4bf-4eb4-8438-91060c4fc24b)

**Token Utility & Value Accrual:** 

1. ***Network Fees:*** End users pay for TEE and ZK coprocessing services in POND. This means that POND demand directly correlates with network usage. 

2. ***Staking Rewards for Validators:*** Validators must stake at least 0.5 MPond or 500,000 POND to operate nodes that cache and relay data. Users can delegate POND and MPOND to other workers and share validator revenue paid out in POND. ***Therefore, POND can be valued based on network cash flow.*** 

# **5. COMPETITIVE LANDSCAPE**
<a id="competitive-landscape"></a>

### ***Decentralized Cloud Services***

Marlin's Oyster subnetwork uniquely combines hardware attestations, cross-chain support, and flexible backend capabilities, making it a straightforward pick for decentralized applications. Gelato and Chainlink critically lack hardware attestations and backend longevity while iExec falls short in serverless capabilities. Akash provides cost-effective cloud instances but relies on trusting the infrastructure. Risc0, Axion, and Delphinus use Zero-Knowledge proofs for secure computations but can't scale or run backends indefinitely like Oyster and rely on cryptographic assumptions for verification. 

|  | Marlin | Gelato & Chainlink | iExec | Akash  |
| :---- | ----- | ----- | ----- | ----- |
| **Security** | Hardware Attestations | Consensus between permissioned operator set | Consensus between workers/TEE | Trusting provider (slashing, reputation) |
| **Support to run backends forever** | Yes | No | No | No |
| **Cross-chain support** | Yes | Yes | Yes | Yes |
| **Coprocessor support for on-chain relaying**  | Yes | Yes | Yes | No |
| **Serverless support** | Yes | Yes | Yes | No |
| **HTTPS endpoints** | Yes | No | Yes | Yes |
| **Fault Tolerance**  | Yes | Yes | No  | No  |

### ***Coprocessors***

While coprocessors are a step in the right direction for blockchain scalability, current solutions overemphasize the promise of isolated ZKPs. We believe Marlin's coupled approach for both TEE and ZK coprocessing is a superior option to isolated TEE or ZK providers. Now, developers can use a single platform to mix and match execution speed, cost, and security guarantees of verification. Especially for bespoke applications like verifiable AI training and inference, we believe Marlin’s user-centric design will attract users in the long run. 

This approach directly contrasts with Risc0, Axiom, and Giza which use isolated ZK proofs. This subjected users to high computational costs and various scalability issues. Conversely, Aizel Network uses TEEs for on-chain LLMs, and Phala Network combines ZK, MPC, and TEEs for its integrated coprocessor. 

|  | Marlin | Aizel Network | Phala Network | Risc0 | Axiom  | Giza  |
| :---- | ----- | ----- | ----- | ----- | ----- | ----- |
| **Overhead Costs** | Low | Low | Low | High | High | High |
| **Security** | TEE, ZK  | MPC, TEE, (ZK in future) | TEE, MPC, ZK | ZK  | ZK  | ZK  |
| **Scalability** | High | High | High | Low | Medium | High |
| **Data Confidentiality** | Yes | Yes | Yes | Yes | Yes | Yes |
| **Flexibility** | High | High | High | Low | Medium | Medium |
| **Supported Models**  | All  | All  | All  | All  | All  | Deterministic  |

# **6. VALUATION & RETURNS ANALYSIS**
<a id="valuation-&-returns-analysis"></a>

## ***Relative Valuation***

Marlin’s coprocessing suite is often compared to isolated ZK alternatives, which have gained massive mindshare but are critically still in early development. Based on industry conversations, ZK coprocessors have received much higher valuation premiums compared to Marlin, including PolyHedra (7.3x) and RiscZero (6.6x). Moreover, the ZK private valuations are mostly \~1 year old, so today’s mark-to-market is likely much higher. We believe TEE peers like Marlin and Phala should at least re-rate closer to ZK valuations, if not be worth more given the superior practicality of the architecture. 

![image2](https://github.com/user-attachments/assets/78012891-7436-4223-8186-6295229270d8)

Furthermore, we argue that comparing Marlin’s live product to the research stage, mostly illiquid ZK-coprocessors paints an incomplete picture. Entire compute ecosystems are more appropriate comparisons because they better reflect Marlin’s flexible L0 architecture and complete cloud offerings. While these alternatives have a wide range of ***higher*** valuations, we believe this average upside of 13.0x is more representative for Marlin than just ZK coprocessors. 

![image6](https://github.com/user-attachments/assets/65614f0a-9309-4a71-b9fa-5ab367d6c74c)


## ***Long-Term Upside Potential***  

[Grand View Research](https://www.grandviewresearch.com/industry-analysis/cloud-computing-industry#:~:text=The%20global%20cloud%20computing%20market%20size%20was%20estimated,are%20realizing%20the%20transformative%20power%20of%20cloud%20computing.) estimates the global Web2 cloud computing market will grow 21.2% from 2023 to 2030, but for simplicity, we assume a 20% CAGR over the time period. Our upside scenario assumes Web3 can penetrate 5% of the global cloud by 2030 and that coprocessors will be 20% of that Web3 cloud market. Looking at current market share dynamics in Web2 cloud services, if Marlin can become a leading player in the coprocessing category (top 3), they’ll likely capture at least 10% of the market. We also believe that coprocessors will demand a 15x valuation multiple, 1.5x higher than standard cloud computing companies since verifiability is a premium feature. Under these assumptions, Marlin would be worth $32B in 2030, representing an attractive **237x upside** **return** compared to today’s valuation. 

<div style="display: flex; justify-content: center;">
    <img src="https://github.com/user-attachments/assets/35838acb-20d5-435d-b183-89180a0505f2" alt="image26" style="width: 50%; margin-right: 10px;">
    <img src="https://github.com/user-attachments/assets/14dbb141-4672-43f0-93e4-25af26c7afb3" alt="image25" style="width: 37%;">
</div>

![image14](https://github.com/user-attachments/assets/99b3dfc0-d5d5-4529-80a5-c07cf51a0ac1)


Sensitivity tables across different input assumptions:

![image8](https://github.com/user-attachments/assets/da9b384e-2978-4932-9e14-6332927f66a1)

# **7. STATE OF THE PROTOCOL**
<a id="state-of-the-protocol"></a>

### ***Marlin Team***

#### **Siddhartha Dutta, Co-Founder** | **[LinkedIn](https://www.linkedin.com/in/duttasiddhartha/)**

   * Former Microsoft Cloud and Enterprise, Adobe Research, Zilliqa Developer 

#### **Prateesh Goyal, Co-Founder** | **[LinkedIn](https://www.linkedin.com/in/prateesh-goyal-2a1534253/)**

   * Former Microsoft Senior Researcher, ETH Zurich Research, MIT PhD, IIT Bombay

#### **Roshan Raghupathy, Co-Founder | [LinkedIn](https://www.linkedin.com/in/roshanrags/)**

   * Former Cityflo Lead Backend Engineer, Microsoft Software Engineer, IIT Bombay

### ***Roadmap***

**Phase 1:** Q3 2024

* Implement Oyster TEE-based serverless coprocessors on AWS cloud platforms  
* Integrate support Circom and Halo2 circuits on Kalypso  
* Optimize Marlin Relay to reduce latency for Ethereum and Polygon networks

**Phase 2:** Q4 2024

* Integrate Marlin Relay with more networks for increased cross-chain capabilities  
* Release SDKs for JavaScript and Rust to facilitate dApp integration  
* Promote to DeFi use cases and establish partnerships with prominent projects.

**Phase 3:** Q1 2025

* Review and update MPond-based governance model for increased community participation   
* Expand Marlin Hub with comprehensive documentation for Oyster, Kalypso, and Relay services

**Phase 4:** Q2 2025 and Beyond

* Develop Marlin-native oracles for low-latency data feeds across multiple blockchain networks  
* Implement sharding in Marlin Relay to increase transaction processing capacity  
* Introduce MarlinVM for custom overlay networks and more advanced computation models

# **8. KEY RISKS**
<a id="key-risks-1"></a>

1. **Coprocessing Competition:** New ZK and TEE coprocessor platforms are rapidly emerging, likely creating a more competitive landscape in the future.   
   *Mitigant:*   
    * ZK is still incredibly costly and underdeveloped. Conversely, TEEs are seeing actual adoption – like Aizel’s teeML – and increasing investor mindshare because of the execution speed and cost benefits. Moreover, Marlin’s first-mover advantage gives it an edge in the category.

2. **Lack of Product-Market-Fit:** Marlin’s success is entirely dependent on higher-level applications and ecosystems leveraging its coprocessing layer for novel & valuable functionality.   
   *Mitigants:*

    * From April to June 2024, Marlin collaborated with Chasm, Talus, OpenLayers, Lighthouse Perpetual Storage, Assisterr, Hyle, GoSleep, and ProjectZKM, matching its novel coprocessing solution to market demands. 

    * Marlin's flexible coprocessing approach is primed for diverse blockchain applications, not to mention the rapidly changing Web3 x AI space, which will likely leverage both ZK and TEE solutions. 

    * As a chain-agnostic base layer, Marlin can easily compose with any stack and does not impose architecture restrictions nor additional trust assumptions. 


3. **Lack of brand and coprocessor narrative awareness:** The coprocessing narrative’s nuanced complexity, especially with TEEs, is a headwind for Marlin’s still underdeveloped branding.   
   *Mitigants:*

    * As of July 2024, investors and developers alike are increasingly excited about coprocessing, especially considering incoming Web3 x AI applications. 

    * TEE builder events (hacker houses) and social media form an attention flywheel for TEEs. Positive investor sentiment is forming because infrastructure/tooling is available, and developers are launching TEE-based applications. 

# **9. SOURCES**
<a id="sources-1"></a>

* [Website](https://www.marlin.org)  
* [Github](https://github.com/marlinprotocol)  
* [Discord](https://discord.com/invite/xqJfSGY6gR)  
* [Docs](https://docs.marlin.org)  
* [Twitter](https://x.com/MarlinProtocol/)  
* [Blog](https://blog.marlin.org)
