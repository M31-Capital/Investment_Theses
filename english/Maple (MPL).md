# Maple Finance (MPL) 
* Current Price: 			$26.48
* Token Type:			Utility token for governance and fee sharing.
* Circ. Token Supply: 		2.793m
* Max. Token Supply: 		10m
* Market Capitalization: 	$73.9m
* 24-Hour Volume: 		$2.1m
* Launch: 			May 2021
* Whitepaper: 			https://maplefinance.gitbook.io/maple/
* Target Price: 			$48

## Historical Chart
![image](https://user-images.githubusercontent.com/96431097/168857213-4aae876d-83f0-4d33-856a-7734b9663a7c.png)

 

## Overview
Maple Finance is a decentralized lending protocol targeted towards institutional and accredited borrowers, by leveraging capital from lenders from DeFi – by providing them with fixed income opportunities on their stablecoins (currently). They adopt a hybrid off-chain, on chain model to select borrowers, and manage loan pools.

Maple finance seems like a solid narrative play going forward, as it differs from other lending protocols in how it operates and gives out loans – with all of the loans on the protocol undercollateralized. They have a solid (but currently modest) fee generation model – all of which accrues to MPL holders and Pool Delegates (who are also MPL holders by default). More on Pool Delegates further in the memo. 
In the last week – Maple Finance has generated around $240k in revenues from loans. 





## Investment Thesis


Higher Interest Rates for Stablecoin Deposits. 

●	Currently, most non leveraged stablecoin deposits earn an average of around 3-5% on most lending protocols across DeFi – which also depends on the loan utilization of those assets. 
●	Passive depositors can earn between 8-10% depositing their stables into maple finance – and are also protected from default risk by MPL holders. 

Undercollateralized Loans will be in High Demand. 
●	Maple Finance’s offering of undercollateralized loans (some even at no collateral) will attract institutional borrowers – within and possibly even outside of the crypto space going forward.


## Catalysts: 

•	Addition of new loan pools that support different assets. (UST for example – can see high potential of Popsicle finance borrowing UST on Maple Finance – and utilizing its degenbox strategy to earn high yields on stables)
•	MPL treasury growth, fitting the DeFi 2.0 narrative of “Protocol Controlled Assets” 




## TAM & Valuation: 

•	Maple Finance’s primary goal is to provide undercollateralized loans to institutional investors, and ultimately allow traditional institutions to also take part in DeFi without the barriers that they currently face. From a passive lenders’ point of view – maple provides higher interest rates (and will most likely continue to do so) when compared to other lending protocols like AAVE, Compound, MakerDao. 
•	From a borrower’s point of view – undercollateralized loans offer a higher value proposition to other algorithmic lending protocols. 
Quantifying the TAM taking into consideration total deposits from other lending protocols: 
AAVE – $30.2b
COMP –$19b
MAKER- $15.7n
ANC - $1.8b
BenQi - $1.18b
            (other lending protocols not taken into consideration) 

Total – approx. $68bn. Assume DeFi grows by 10x – TVL also grows by 10x – TAM becomes around $680bn.
Assume Maple Finance pulls in 
5% - $34bn
10%- $68bn
20% - $136b


●	We can try valuing the MPL Token using a DDM as the MPL token accrues fees from the treasury and from loans funded. Currently MPL holders generate fees through loans funded. 1% of all loans funded are taken by the protocol as establishment fees – half of which are distributed to MPL holders i.e., 0.5% of all loans funded. This parameter can be changed through governance. Currently the protocol has funded around $218m in loans. 

Conservative: loans 5x in the first year and grow 10% YoY after that. Token is 5x overvalued.

![image](https://user-images.githubusercontent.com/96431097/168857386-03516543-6084-48cb-89f5-dad0dda8d891.png)



Moderate: loans 10x in the first year and grow 20% YoY after that. Token is 2.5x overvalued.

![image](https://user-images.githubusercontent.com/96431097/168857413-78bf9184-6a3f-4752-884a-f889242ce3e6.png)



Bullish: loans 20x in the first year and grow 30% YoY after that. Token is relatively fairly valued according to this model. 

![image](https://user-images.githubusercontent.com/96431097/168857460-ee618a7e-a7cc-4769-817f-21e2c7a5e5d0.png)

 


Uber-Bullish (Fee Change): loans 20x in the first year and grow 30% YoY after that. Establishment fees are changed to 2% of all loans funded through governance. 
Considering this model, the token is undervalued by almost 100%. 

![image](https://user-images.githubusercontent.com/96431097/168857509-72759ee8-095c-4d0d-a201-8ce2951d7e4a.png)

 

This valuation doesn’t consider additional revenues that can accrue to MPL holders who stake MPL-USDC in a balancer pool to provide insurance cover for the lenders in case of a default from the borrowers. MPL stakers receive 10% of all the interest earned by the protocol on loans funded. 
Assuming an average interest rate of 12% charged on all loans – and assuming 50% of the total MPL supply is staked – MPL stakers would earn around $0.82/token in ongoing fees in Y1 – growing to $35.96/token in Y5.

![image](https://user-images.githubusercontent.com/96431097/168857569-09258a67-e7b8-4758-bf18-b33e080e02a9.png)

 


## Industry Outlook 

●	Traditional lending protocols are not providing high enough interest rates on stablecoin deposits, and are currently sustaining liquidity through liquidity mining incentives. As deposits grow – those fees are likely to go lower. 
●	Anchor provides much higher interest rates on UST deposits (at 20%) – however it is limited to UST only – and is paid out in ANC – not the native deposit asset.



## Competitors

●	Traditional competitors – Any traditional banking/brokerage firm. 
●	Crypto Competitors – Undercollateralized lending protocols like Teller Finance. 

## Recent Trends & Changes

●	Can potentially synergize with Tokemak to direct liquidity into the protocol and fund more loans. 





## Technology:

The protocol functions on three main actors. 

Pool Delegates (PDs): They open pool contracts, and perform DD on borrowers + agree loan terms with borrowers for that pool. They then approve loans to borrowers and allocate funds from the loan pool. Selected by the DAO.

Liquidity Providers (LPs): LP’s deposit single assets into pool contracts to fund loans approved by PDs. They receive LP tokens that accrue interest earned by the pool on loans provided to borrowers. 

Borrowers: These are institutions, that are approved by LDs – that take loans at fixed terms from a loan pool. They pay interest to the pool at a fixed rate.

LPs deposit assets into pool contracts managed by a PD. The LPs earn a yield of 8-10% on the assets they stake. The protocol governance selects PDs, who manage a loan pool. They perform DD on borrowers, agree specific loan terms, and also provide default cover to the Loan pool by staking BPT tokens that reflect an MPL-USDC deposit on balancer. 

Additionally, MPL token holders can also earn a higher yield from a pool, by depositing BPT tokens into a staking contract on Maple finance that represents a MPL-USDC deposit on balancer, to cover the loan amount in case of a borrower default.

Protocol Revenue: 
The protocol accrues revenue to the treasury through: 
a) Establishment Fees – 0.5% of the total drawdown amount of loans in a pool. 50% of this value accrues to the protocol treasury. 
MPL Holders:
Revenue accrues to MPL holders through:
a) Establishment Fees from the protocol treasury accrue to MPL holders, as they are distributed periodically.
b) Ongoing Fees – 20% of the total interest earned by the loan pools. 
MPL holders that stake their tokens will receive 50% of this value. 




## MPL Tokenomics:

The value of MPL is derived from: 

1. The value of loans that Maple finance can provide to lenders – fees earned from loans funded. 
2. The number of tokens that Maple will add to its treasury through fees from loan pools of varying assets.  
3. Yields generated on treasury assets. 

![image](https://user-images.githubusercontent.com/96431097/168857634-26070fba-c5b0-42ee-8f5a-317690ca1758.png)


 
## Total supply capped at 10,000,000 MPL. 

30% - Team (24 month vest)
26% - Investors (18 month vest)
25% - Liquidity mining incentives 
14% - Maple Treasury
5% - Initial Token Launch on Balancer.
 
Token Utility : Governance and share of establishment fee revenue.
MPL staking on balancer earns additional rev share in ongoing fees.







## SWOT Analysis

Strengths: 
1.	Offering undercollateralized loans in DeFi.
2.	Higher interest rates on stablecoins provided than most other lending protocols. 

Weaknesses: 
1.	Loan agreements, terms to borrowers, and due diligence for borrowers is done off-chain with lenders getting no access to the DD. 

Opportunities: 
1.	Integrating with ETH L2’s, and alternate L1 projects would bring larger amounts of capital.
2.	Offering pools for non-stable (or non USDC) deposits – which would diversify the Maple treasury. 
3.	Potential collaboration with Olympus Pro to boost owned liquidity to provide loans with

Threats

1.	A large number of the borrowers are in the crypto industry and actively trade. In the case of a crypto market crash, borrowers would suffer significant damage and the risk for default increases.
2.	Stablecoin regulation risk. 
3.	Stablecoin depegging risk



# Token Metrics
#![MPL Token Metrics](https://user-images.githubusercontent.com/96431097/168857051-11713594-1730-4581-82c8-e396f5b72ea6.jpg)






# Management & Team

●	Sidney Powell, Co-Founder 
●	Joe Flanagan – Co-Founder
Team of 18+ with 2 core devs.

Team is actively hiring new developers.


# CRYPTO-NATIVE DILIGENCE

Code Audits
As of now, Tokemak has been audited by Peckshield and Dedaub. This covers all the smart contracts in the protocol, and the security. Most high risk and medium risk issues resolved.
Link to all Audits - https://github.com/maple-labs/maple-core


Open Source Risk (Forking Risk)

●	Forking Risk – Protocol smart contracts can be forked – however, what Maple has as a moat is a solid VC backing, as well as a unique system of pool delegates that guarantee accredited and trusted borrowers.

 
# Resources
Github: https://github.com/maple-labs
Docs: https://maplefinance.gitbook.io/maple/
Code audits: https://github.com/maple-labs/maple-core
