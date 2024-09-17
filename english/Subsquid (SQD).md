<img width="200" src="https://github.com/user-attachments/assets/92299654-1405-4ff2-822d-e297ea0b6f0b">

[Subsquid Network (SQD)](https://subsquid.io/) is a decentralized indexing and querying solution for blockchain data, enabling developers to efficiently access and analyze on-chain information. It provides a scalable and modular architecture, allowing for customized data pipelines and real-time updates. The project is not well known or understood by the market, creating a highly attractive entry valuation.

|  | LAUNCH | ENTRY | CURRENT |
| :---- | :---: | :---: | :---: |
| **Date:** | January 2024 | June 2024 | August 2024 |
| **Price:** | $0.094 | $0.05 OTC (Market @ $0.10) | $0.041 |
| **Circulating Market Cap:** | $5.0m | $25.0m  | $10.4m  |
| **Fully Diluted Market Cap:**  | $126.0m | $134.0m  | $54.9m |
| **Circulating Supply:**  | 53.4m SQD (4.0%) | 180.5m SQD (13.5%) | 251.4m SQD (18.8%) |
| **Max Supply:**  | 1.34b SQD | 1.34b SQD | 1.34b SQD |

**INVESTMENT THESIS**
---

Top 3-5 reasons why we need to own this name: 

1. **Unique and differentiated asset in a highly valuable part of the Web3 technology stack (data lake)**

2. **Neglected and severely mispriced because of its ineffective social media marketing**  
     
3. **Subsquid has a networking architecture superior to large incumbents**  
     
4. **Uniquely attractive risk/reward investment opportunity; Subsquid’s current FDV offers 18x upside**  
      
5. **Opportunity for M31 to add meaningful value to the investment by working closely with the team**

**KEY RISKS**
---

Top 3-5 reasons why this investment will fail: 

1. **The brand and value prop isn't well known by the market.** Leadership has indicated a potential re-brand in the near-future, but this would introduce additional execution risks.

2. **The Graph is currently the leading blockchain data indexer,** and developers are hesitant to shift their development tools.

3. **Other ZK coprocessor projects have proprietary ZK proving technology** and are closer to the mainnet than Subsquid’s offering, **giving them first-mover advantages.**

4. **Subsquid hasn't yet solved the centralized blockchain data injection problem**, which can impact market adoption due to the risk of a single point of failure.

---
---
### *Table of Contents:*

1. [*PROTOCOL OVERVIEW*](#protocol-overview)

2. [*INVESTMENT THESIS*](#investment-thesis)

3. [*TECHNICAL OVERVIEW*](#technical-overview)

4. [*BUSINESS MODEL & TOKENOMICS*](#business-model-&-tokenomics)

5. [*COMPETITIVE LANDSCAPE*](#competitive-landscape)

6. [*VALUATION ANALYSIS*](#valuation-&-returns-analysis)

7. [*STATE OF THE PROTOCOL*](#state-of-the-protocol)

8. [*KEY RISKS*](#key-risks-1)

9. [*SOURCES*](#sources-1)

---
---

# **1. PROTOCOL OVERVIEW** 
 <a id="protocol-overview"></a> 

**Product:** Subsquid is a decentralized query engine optimized for efficiently extracting large volumes of data. It currently processes historical on-chain data from over 100 EVM and Substrate networks, as well as Solana (in beta) and Starknet. The data includes comprehensive details such as event logs, transaction receipts, traces, and per-transaction state diffs for EVM. It is also developing ZK coprocessor functionality, leveraging its multi-chain indexing capabilities along with existing ZK prover marketplaces like Polyhedra ,=nil, and RiscZero to trustlessly connect smart contracts with its network of off-chain data lake resources.

**Problem:** One of the biggest challenges Wev3 developers face today is accessing data at scale. It's currently highly complex to query and aggregate the exponentially growing amount of data produced by blockchains (transactions and state data), applications (decoded smart contract states), and any relevant off-chain data (prices, data kept in IPFS and Arweave, pruned EIP4844 data). This data is often fragmented across multiple ecosystems, chains, and technologies, leading to non-standardized structures and silos. This fragmentation results in incomplete datasets, making it difficult to extract meaningful insights. 

In Web2, data is stored in centralized data lakes like BigQuery, Snowflake, Apache, and Iceberg to facilitate access. However, storing Web3 data in similar centralized data lakes would defeat the purpose of open, resilient access. If aggregated, filtered, and easily extractable, Web3 app data can unlock the potential of the industry in a multi-chain paradigm.

![image3](https://github.com/user-attachments/assets/40be325f-7ebc-40d2-8a65-df26119ecbba)

**Solution:** Subsquid offers a modular approach where on-chain data is extracted from a decentralized data layer ([Subsquid Network](https://docs.subsquid.io/subsquid-network/)), rather than directly from a blockchain node. This approach enables up to 100x faster indexing, guarantees data consistency, and provides reliable indexing even for small networks. Given its superior architectural design, Subsquid reduces data extraction and indexing costs by up to 90% compared to centralized RPC providers like Alchemy or Infura. Using Subsquid Cloud, developers can avoid the costs and hassle of indexing infrastructure maintenance.

***Product Suite***

**Subsquid Network:** A distributed query engine and data lake around which the Subsquid ecosystem is built. It currently serves historical blockchain data for over 80 networks. Compared to data access using conventional chain node RPC, Subsquid Network allows for near-zero cost data access in a more granular fashion and from multiple blocks simultaneously. There are currently two independent instances of Subsquid Network:

* *Permissionless Public Network:* The decentralized version of Subsquid Network is currently in the testnet phase.  
* *Open Private Network:* Subsquid's private data lake, formerly known as Archives, is a production-ready fork of the early Subsquid Network. It serves as a stand-in for the permissionless version until it matures. Its API is identical to that of the P2P gateways of the public network.

**Squid SDK:** The Squid SDK is a powerful TypeScript toolkit for building indexers on top of Subsquid Network, featuring:

* High-level libraries for extracting and filtering Subsquid Network data in ETL (Extraction, Transformation, Loading) pipelines.  
* Ergonomic tools for decoding and normalizing raw data and efficiently accessing network state.  
* Pluggable data sinks to save data into Postgres, files (local or s3), or BigQuery.  
* An expressive GraphQL server with a schema-based config.  
* Seamless handling of unfinalized blocks and chain reorganizations for real-time data ingestion.  
* Rapid data extraction and decoding for local analytics.

This application is primarily geared towards institutional blockchain data providers to create their APIs leveraging Subsquid Network.

**Subsquid Cloud:** A Platform-as-a-Service for deploying Squid SDK indexers on top of the Subsquid Network. The indexers deployed to the cloud will source data from the Subsquid Network, but the hosted service itself is centralized, featuring:

* Provisioning of Postgres and other compute resources for indexers.  
* Zero downtime migrations between indexer versions.  
* Provisioning of high-performance RPC endpoints for real-time applications.  
* Intuitive deployment management through a web application or CLI.  
* Google Cloud-level SLAs.

This application is more suited for DApp developers and analytics platforms.

**Subsquid Firehose:** Developing and running subgraphs is challenging because it requires running a full archival node, which is not feasible for many networks. Subsquid Firehose is an open-source lightweight adapter that solves this by running as a sidecar to a graph indexer node, ingesting and filtering data directly from Subsquid Network instead of an RPC endpoint.

**ApeWorx Subsquid Plugin:** ApeWorx is a modular Web3 development framework for Python programmers used to develop and test dApps. The plugin provides free access to blocks and event logs data and data retrieval is orders of magnitude (over 10x) faster than RPC-based data sources.

***Target Market***

* **Decentralized Application (dApp) Projects:** Projects that are developing dApps across various blockchains can benefit from Subsquid's ability to provide customized data indexing and querying solutions. This includes projects in sectors like DeFi, NFTs, gaming, social media, and more. By leveraging Subsquid, these projects can enhance their application performance and user experience.  
* **L1 and L2 Blockchain Networks:** By integrating Subsquid, blockchain ecosystems enhance their data infrastructure, providing developers with the tools they need to build powerful, data-driven applications.    
* **Blockchain Analytics and Research Firms:** Companies and organizations that specialize in blockchain analytics, research, and data services may use Subsquid to gather and analyze blockchain data more efficiently. Subsquid's tools can help these firms process large volumes of data for insights, trends, and patterns relevant to their research or analytics products.

***Use Cases***

* **On-Chain Protocols (ZK Coprocessor):** Subsquid Network, in conjunction with existing proof markets, enables applications to move complex logic off-chain securely, allowing them to harness more compute power while verifying results on-chain. This opens doors to a wide range of data-driven applications such as order book DEXs, lending protocols, and perpetuals on the blockchain.  
* **Multichain Applications (NFT, DeFi, Wallets, RWA):** Subsquid allows multi-chain applications to request data in a more granular fashion from multiple chains simultaneously, compared to conventional chain node RPC data access. This capability is crucial for applications as they expand across multiple chains.  
* **Web3 Data & Dev Tooling:** Subsquid provides granular data from multiple blockchains, which is essential for data companies and development tools that need to support multiple chains based on specific developer requirements.  
* **Web3 Games:** The Subsquid SDK allows Web3 games to index required on-chain user actions according to their data requirements and save this information to their local databases like Postgres, BigQuery, S3, and others.  
* **Web3 Social:** Subsquid can also be used to index social protocols like Farcaster and Lens, meeting the requirements of their front-end clients.

# **2. INVESTMENT THESIS** 
<a id="investment-thesis"></a>


1. **Unique and differentiated asset in a highly valuable part of the Web3 technology stack (data lake),** which will become more important as applications become more complex, decentralized AI proliferates, and general industry adoption expands, resulting in exponentially more on-chain data.  
     
2. **Neglected and severely mispriced** because of its ineffective social media marketing, underwhelming token launch event, and esoteric technical differentiation.   
     
3. Despite the lack of attention from the market, **Subsquid has a networking architecture superior to large incumbents,** impressive early customer traction, and an exciting roadmap to offer both full data warehouse capabilities and ZK coprocessing functionality.  
     
4. Uniquely attractive risk/reward investment opportunity; **Subsquid’s current FDV offers 18x upside to achieve valuation parity with The Graph (GRT),** which we believe has objectively inferior technology and highly inefficient network economics.  
      
5.  Opportunity for **M31 to add meaningful value to the investment by working closely with the founders** on their potential reband, storytelling in the media, and business development (we have already made intros to Stateless, Injective, and Super Protocol). 

    

# **3. TECHNICAL OVERVIEW**
<a id="technical-overview"></a>

Subsquid Network is designed to provide infinite horizontal scalability, permissionless data access, trust-minimized queries, and low maintenance costs. Its architecture ensures:

* Raw data is uploaded into permanent storage by data providers.  
* Data is compressed and distributed among network nodes.  
* Node operators bond a security deposit, which can be slashed for byzantine behavior.  
* Each node efficiently queries local data with DuckDB.  
* Queries can be verified by submitting a signed response to an on-chain smart contract.

***Network Architecture***

![image9](https://github.com/user-attachments/assets/9f2873bc-05bb-422d-ae99-bc50ed7f0999)

* **Data Providers:** Data providers ensure the quality and timely provision of data. During the bootstrapping phase, Subsquid Labs GmbH serves as the sole data provider, acting as a proxy for chains from which the data is ingested block-by-block. The ingested data is validated by comparing hashes, then split into small compressed chunks and saved into persistent storage. These chunks are randomly distributed among workers. After the Mainnet launch, the dataset metadata is kept on-chain with attestations, enabling fully trustless verification. Following this, Subsquid will start onboarding new operators.  

![image11](https://github.com/user-attachments/assets/ba9cbfd5-917d-475e-9a02-61586e23f3fd)

* **Workers:** Contribute storage and compute resources to the network. They serve the data in a peer-to-peer manner for consumption and receive SQD tokens as compensation. Each worker must register on-chain by bonding 100,000 SQD tokens, which can be slashed if they violate protocol rules. SQD holders can also delegate tokens to a specific worker, signaling reliability and earning a portion of the rewards.

* **Scheduler:** Distributes data chunks submitted by data providers among workers. It monitors updates to data sets and worker sets, sending requests to workers to download new chunks or redistribute existing ones based on capacity and redundancy targets. Upon receiving an update request, a worker downloads the missing data chunks from persistent storage.

* **Logs Collector:** Collects liveness pings and query execution logs from workers, batches them, and saves them into public persistent storage. The logs are signed by the workers' P2P identities and pinned to IPFS. This data is stored for at least six months and is used by other network participants.

* **Rewards Manager:** Accesses logs, calculates rewards, and submits a claimable commitment on-chain for each epoch. Workers then claim their rewards individually, which may expire after an extended period. 

* **Data Consumers:** Query the network by operating a gateway or using an externally provided service (public or private). Each gateway is bound to an on-chain address. The number of requests a gateway can submit is capped by the amount of locked SQD tokens, effectively yielding virtual "compute units" (CU) based on the lock period. All queries cost 1 CU until complex SQL queries are implemented.

***Rewards*** 

Network rewards are distributed to workers and delegators for each epoch. The Reward Manager submits an on-chain claim commitment, allowing participants to claim their rewards. The initial reward pool, comprising 10% of the total SQD supply allocated at TGE, has a fixed supply and protective mechanism capping the rewards per epoch. For the first three years, the reward cap and total supply remain fixed. After this bootstrapping phase, the reward cap decreases significantly until governance decides on the inflation schedule and new tokens are minted to replenish the reward pool.

**Reward Rate:** The rate depends on how much of the network is being used and the total amount of tokens staked. Network utilization is calculated by comparing the target capacity (desired storage space) and actual capacity (available storage space). The target annual percentage rate (APR) is calculated based on utilization and total staked tokens. It's capped to ensure rewards don't exceed a certain limit. The base APR is around 20% but can increase to 70% to attract more workers until the network reaches its desired capacity.

Subsquid Labs GmbH currently operates the Scheduler, Log collector, and Reward Manager without collecting any operational fees. All the data is published via libp2p pubsub and is fully auditable, Subsquid plans to decentralize this setup after the Mainnet launch.

***Query Validation***

Subsquid Network provides economic guarantees for the validity of queried data, with the possibility of on-chain validation. All query responses are signed by the worker who executed the query, acting as a commitment to the response. If deemed incorrect, the worker's bond is slashed. Validation logic may be dataset-specific, with options including:

* *Proof by Authority:* A whitelist of on-chain identities decides the validity of responses.  
* *Optimistic On-chain:* After a validation request, anyone can submit proof of an incorrect response.  
* *Zero-Knowledge:* A zero-knowledge proof verifies the response exactly matches the request. The proof is generated off-chain by a prover and validated on-chain by the smart contract.

***Multichain Zk Coprocessor*** 

Subsquid is developing a ZK coprocessor solution, leveraging its multi-chain indexing capabilities along with existing ZK prover marketplaces like Polyhedra ,=nil, and RiscZero to trustlessly connect smart contracts with its network of off-chain data lake resources.

![image2](https://github.com/user-attachments/assets/28498f26-f8ce-4228-a054-c805f58eb909)

**Work Process:** When a user sends a query request, the Subsquid Network first computes the results of the query. Then, it uses Proof Market Networks to generate a ZK proof, ensuring the results are derived from the correct data. Finally, the query results and the proof are passed to the user.

This opens doors to high-compute and data-driven applications such as order book DEXs, lending protocols, and perpetuals, even on blockchains with low TPS and strict programming languages.

# **4. BUSINESS MODEL & TOKENOMICS** 
<a id="business-model-&-tokenomics"></a>

***Business Model***

**Data Consumers:** Data consumers, such as developers and businesses, must operate a gateway or use an external service (public or private) to query the Subsquid network. Each gateway is linked to an on-chain wallet address, and the number of queries it can perform is determined by the amount of SQD tokens it has locked. The more tokens locked by the gateway operator, the greater the bandwidth they are allowed to consume. This mechanism operates similarly to virtual "compute units" (CUs), with locked SQD tokens generating CUs over time.

**Pricing Model:** All queries initially cost the same price of 1 CU. The query cap is calculated by:

* Determining the virtual yield in SQD on the locked tokens.  
* Multiplying by the current CU price (in CU/SQD).

Additionally, a booster mechanism incentivizes gateway operators to lock their tokens for longer periods, increasing the number of CUs allocated per SQD annually. At the launch, the parameters are set with a BASE\_VIRTUAL\_APY of 12%, and 1 SQD yields 4,000 CUs.

![image6](https://github.com/user-attachments/assets/15ff8677-c627-4dc7-b182-fa3e97c44697)

For example, if a gateway operator locks 100 SQD for 2 months, the virtual yield is 2 SQD, which means it can perform 8,000 queries (8,000 CU). If 100 SQD are locked for 3 years, the virtual yield is 12% \* 3 APY, so the operator gets CUs worth 108 SQD, that is it can submit up to 432,000 queries to the network within 3 years.

**Payment Flow:**

* *Customers (Data Consumers):* Pay by locking SQD tokens to generate CUs, which are used to submit queries.  
* *Gateway Operators:* Benefit from the CUs generated by their locked tokens, allowing them to serve more queries. They are incentivized to lock tokens for longer periods to increase their CU yield.

**Decentralization Plan:** Subsquid plans to decentralize over time by gradually increasing the role of community governance and reducing central control. Key aspects of the decentralization plan include:

* *Community Governance:* Empowering the community to participate in decision-making processes, such as adjusting the CU pricing model, BASE\_VIRTUAL\_APY rates, and other network parameters.  
* *Incentives for Participation:* Providing incentives for network participants to engage in governance and contribute to network security and stability.  
* *Distributed Infrastructure:* Encouraging a wide distribution of gateway operators across different geographical regions to enhance network resilience and reliability.

By progressively decentralizing the network, Subsquid aims to create a more robust, secure, and community-driven ecosystem that benefits all stakeholders involved.

## ***Tokenomics***

SQD is the ERC-20 (Ethereum, Arbitrum) utility token of the Subsquid Network, used for demand-side payments, supply-side rewards, network participant delegation (enabling network revenue sharing), and governance. Users interacting with the Subsquid chain as workers must stake SQD tokens to participate in roles. 

With a total token supply of 1.337b SQD, half (668m tokens) are allocated to the Subsquid DAO: 54% to the community, 15% to the team and advisors, 23% to early adopters, and 8% to financial backers. The remaining 50% is allocated to Subsquid Network operations: 56% for the treasury, 22% for operations, and 22% earmarked for rewards.

![image12](https://github.com/user-attachments/assets/11d426e3-88b9-4b45-b47f-c74b04392b7b)
  
The token distribution is structured to ensure long-term commitment and ecosystem development. Key allocations include 12% for pre-seed backers and 16.3% for seed backers, both with a 6-month lockup and subsequent 24-month vesting. Strategic backers from early 2022 receive 4.6% with a 12-month linear vesting, while Strategic II backers get 2% with a 6-month lockup and 18-month vesting. The team is allocated 15% with a 6-month lockup and 24-month vesting. A significant 28.1% is reserved for network development and ecosystem activities with a 36-month vesting period. Additional allocations include 5% for market liquidity, 10% for network node operators with an 84-month vesting, and 5% for community sales with a 6-month vesting. Early adopters and node operators from the testnet are rewarded with 1% each, with varying lockup and vesting periods.

![Screenshot 2024-09-12 at 1 00 22 PM](https://github.com/user-attachments/assets/5b4648d7-f2e3-45c8-95d4-85c8166ba6f8)

# **5. COMPETITIVE LANDSCAPE**
<a id="competitive-landscape"></a>

## ***Blockchain Indexing***

The Graph is the closest competitor to Subsquid in the indexer space. By design, The Graph's indexing node is a black box that executes subgraphs compiled into WASM. The data is sourced directly from the archival node and local IPFS, and the processed data is stored in a built-in Postgres database. In contrast, Subsquid Network offers near zero-cost data access, more granular data retrieval from multiple blocks, and superior batching and filtering capabilities. 

![image7](https://github.com/user-attachments/assets/83e16b19-b0d9-40c0-aaa9-e37f5f4a9f9c)

* *Free Access to Historical Data:* Subsquid Network is currently completely free to query, allowing developers to reduce development costs significantly. This is possible because Subsquid charges fixed subscription fees to chains from which the data is provided.  
* *High-Speed Data Processing:* Subsquid Network ensures rapid data retrieval and processing, making projects run smoother. Each worker handles a subset of blocks, has a modular architecture, and uses DuckDB database. This architecture reduces latency, allowing for faster application performance and a better user experience.  
* *User-Friendly Deployment:* The Firehose adapter allows subgraphs to be deployed in as little as five minutes without additional setup. It runs as a side-car to a graph indexer node, ingesting and filtering the data directly from Subsquid Network instead of an RPC endpoint. This streamlined process eliminates the need for extensive configuration, simplifying the transition from development to deployment and reducing time-to-market.  
* *Local Run Capability:* Subsquid Network offers flexibility in deployment. Users can run their subgraph locally with a few simple commands, eliminating the need for Subgraph Studio or an archive node. This setup makes data available almost immediately without the need for extensive syncing.   
* *Code-Free Deployment:* Previously, using Subsquid Network required migrating the subgraph to the Squid SDK, which could be time-consuming for larger subgraphs. Now, the Subsquid network gateway eliminates the need for migration, allowing subgraphs to be deployed without changing a single line of code.   
  


| Feature | Subsquid | The Graph |
| :---- | :---- | :---- |
| Programming Language | Typescript | AssemblyScript (complied to WASM) |
| Indexing Speed | \~1k-50k bps | \~100-150 bps |
| Real-Time Indexing  (Unfinalized Blocks) | Yes | No |
| Off-Chain Data | Yes | No |
| Data Targets | Customizable | Postgres-only |
| Customizable DB Migrations | Yes | No |
| Multi-Contract Indexing | Yes | Limited |
| Analytic Data Targets | BigQuery, Parquet, CSV | No |
| Local Setup | Easy | Requires an archival node |
| Custom Resolvers  and Mutations | Yes | No |
| Secret .env Variables | Yes | No |

**Database ZK Coprocessors:** Unlike some coprocessors that develop verifiability technology in-house, Subsquid views this as a pluggable component that can be developed in conjunction with ZK prover marketplaces like Polyhedra, \=nil, RiscZero, and others. This approach allows Subsquid to innovate and improve much faster by leveraging the development efforts of other teams in the existing ZK coprocessor space.

| Feature | Space and Time | Subsquid |
| :---- | :---- | :---- |
| Multi-Chain  Support | All EVM chains, Sui, Aptos, Sei | Supports all EVM and Substrate-based  chains (Cosmos & Solana soon) |
| Can Incorporate  Off-chain Data | Yes | Yes |
| Query Cost  | Sub-dollar cost per query | Sub-dollar cost per query (without  Zk proof) |
| Proof System | Proof of SQL | Pluggable component leveraging 3rd party ZK prover marketplaces like Polyhedra,  \=nil, RiscZero, and others |
| Latency with  Proof Generation | 0.5 seconds | In development stage |
| Data format | Data Warehouse: Stored in a  structured format, optimized for querying. | Data Lake: Stores raw blockchain data, optimized for holding vast amounts  of data. |
| Data Processing | ETL (Extract, Transform, Load): Data  is transformed before loading. | ELT (Extract, Load, Transform): Data is loaded in raw form and transformed  when needed. |
| Queries  | Utilizes SQL for querying. | Offers a framework to create  custom GraphQL & APIs for data queries. |
| Customizability | Offers extensive flexibility in data  analysis, with support for custom  SQL queries and integration with  traditional data analytics tools. | High level of customization in how data is indexed and queried, allowing  developers to tailor data endpoints to  their needs. |

# **6. VALUATION ANALYSIS**
<a id="valuation-&-returns-analysis"></a>

### ***Relative Valuation***

Subsquid’s best liquid token comp is GRT, which trades at 18x FDV premium to SQD. Space and Time will be another direct comp when the token starts trading later this year, which should also be a catalyst for SQD, drawing market attention to the value of the Web3 big data sector. 

Longer-term, as the Web3 industry matures and adoption reaches the mainstream, it’ll be reasonable to compare Subsquid to similar Web2 companies, which imply 100x+ upside if the project (and Web3 at large) is successful. 

![image8](https://github.com/user-attachments/assets/0f9b334e-250f-43f6-8a79-7b777e83f98e)

***Note**: Subsquid’s last private funding round came in January 2024, with a partial public sale via CoinList that gave the project a $125m FDV. The token sale raised $6.3m in just 19 minutes, making it one of the fastest sales on the platform.* 

# **7. STATE OF THE PROTOCOL**
<a id="state-of-the-protocol"></a>

***Subsquid Team*** 

**Dmitry Zhelezov, Co-Founder** | [Dmitry Zhelezov | LinkedIn](https://www.linkedin.com/in/dmitry-zhelezov-23766217/) 

* Holds a Ph.D. in mathematics and has extensive experience in scaling query nodes and peer-to-peer (P2P) networks. He worked at Hydra (a query node framework for Substrate blockchains) and Helix Cognitive Computing (developing cutting-edge digital ecosystems and peer-to-peer digital exchange networks).

**Marcel Fohrmann, Co-Founder** |  [Marcel Fohrmann | LinkedIn](https://www.linkedin.com/in/marcel-fohrmann/) 

* Previously co-founded Helix Cognitive Computing and graduated from Stanford Business School.

**Evgeny Baburov, Product Lead** | [Evgeny Baburov | LinkedIn](https://www.linkedin.com/in/ebaburov/) 

* Brings over 20 years of industry experience. He worked as Product Lead at VTB (a global provider of financial services), Edna (a digital communication solutions provider), and founded Sane.company (a web studio and advertising agency).

**David Langellotti, Growth Lead** | [David Langellotti | LinkedIn](https://www.linkedin.com/in/david-langellotti-3722a1207/) 

* Has more than 7 years of experience in marketing. He worked at Altercap (crypto-finance platform), QRC Group (marketing and documentation for companies in the web3 space), and Blockpass (provides privacy-focused KYC/AML).

***Subsquid Metrics & Partnerships***

![image4](https://github.com/user-attachments/assets/e8c9ad94-2739-46ce-ad36-67e8b4308b8c)
![image10](https://github.com/user-attachments/assets/36cbd0d9-f6c6-421b-ab78-f4dbd38fee39)

**Google Cloud Partnership (BigQuery Integration):** Google Cloud’s BigQuery is a powerful enterprise data warehouse solution that allows companies and individuals to store and analyze petabytes of data. Designed for large-scale data analytics, BigQuery supports multi-cloud deployments and offers built-in machine learning capabilities, enabling data scientists to create ML models with simple SQL. BigQuery is also fully integrated with Google's own suite of business intelligence and external tools, empowering users to run their own code inside BigQuery using Jupyter Notebooks or Apache Zeppelin.

Multi-chain projects can leverage Subsquid alongside BigQuery to quickly analyze their usage across different chains and gain insights into fees, operating costs, and trends. Saving custom-curated data to BigQuery lets developers leverage Google's analytics tools to gain insights into how their product is used, beyond the context of one chain or platform.

**Partner with RPC Providers:** Subsquid partners with key RPC providers (Nodies, Blastapi, Chainstack) by offering zero-interest loans for operating gateways to the Subsquid Network. With minimal operational costs, these providers can deliver indexed data from the Subsquid Network to their users, thus driving Subsquid adoption.

**One-Click Node Deployment**: Subsquid has partnered with Deutsche Telekom, Google Cloud, and Blockjoy to enable one-click deployments for node operations. This collaboration simplifies node development for node operators. 

**Supporting New Ecosystems:** Subsquid plans to support emerging chains like Solana, Fuel, Sui, and Aptos in its roadmap. With minimal competition in the indexing space for these networks, Subsquid has already observed signs of traction, even while support is still in beta for some of these networks.

***Roadmap***

![image14](https://github.com/user-attachments/assets/3639b8da-811b-4f80-b8f7-1904c3433d35)

* *Mainnet Launch:* Establishes the foundation for network growth, enabling token delegation and permissionless data access.  
* *Cosmos Support:* Expands capabilities to the Cosmos ecosystem, broadening the user base.  
* *Permissionless Dataset Submission:* Subsquid GmbH currently maintains datasets, with plans for decentralized submission and curation.  
* *Decentralized SQL Database Streaming:* Distributes and syncs databases across the data lake, ensuring accuracy and timeliness.  
* *Enterprise Tooling:* Implements Kafka for real-time data handling and Snowflake for big data analysis and storage.

# **8. KEY RISKS**
<a id="key-risks-1"></a>

1. Although Subsquid has differentiated technology and impressive early customer traction, **the brand and value prop isn't well known by the market.** This is evident in its lackluster token launch and conversations with many Web3 investors. Leadership has indicated a potential re-brand in the near-future, but this would introduce additional execution risks.  

   *Mitigant*  

      * This creates an extremely attractive entry point for M31 to build its investment. Our storytelling abilities, broad network reach, media connections, and other resources can help communicate the protocol’s value in a way the market can easily understand.

2. Despite its disadvantages, **The Graph is currently the leading blockchain data indexer,** and developers are hesitant to shift their development tools.

   *Mitigant*

      * Having an effective distribution strategy by partnering with leading Web3 educators can help attract more developers to switch.


3. **Other ZK coprocessor projects have proprietary ZK proving technology** and are closer to the mainnet than Subsquid’s offering, **giving them first-mover advantages.**  

   *Mitigant*  

      * The ZK marketplace approach may end up being a better strategic approach in the long-run; as ZK technologies continue to innovate and evolve, the tech-neutral marketplace approach allows the Subsquid platform to continuously offer the best 3rd party solutions in the market, each optimized specifically for use case and workload. 

4. **Subsquid hasn't yet solved the centralized blockchain data injection problem**, which can impact market adoption due to the risk of a single point of failure.  

   *Mitigant*  

      * Subsquid can leverage existing decentralized RPC networks like Pocket, Lava, or Stateless to decentralize their data entry.

# **9. SOURCES**
<a id="sources-1"></a>

* [Website](https://www.sqd.dev)  
* [Whitepaper](https://docs.sqd.dev/subsquid-network/whitepaper/)  
* [Github](https://github.com/subsquid)  
* [Discord](https://discord.com/invite/hellosqd)  
* [Docs](https://docs.sqd.dev/overview/)  
* [Twitter](https://x.com/helloSQD)  
* [Podcasts](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://podcasts.apple.com/us/podcast/subsquid-network-the-web3-data-lake/id1471243424%3Fi%3D1000643735766&ved=2ahUKEwiYquu6hrqIAxV4F2IAHartEigQFnoECBcQAQ&usg=AOvVaw1LMdyhBLUKEXDggCIsUay6)
