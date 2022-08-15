Audius – Investment Thesis (GitHub) 

## Overview 

Audius is a decentralized music streaming platform, that leverages blockchain technology to power distribution of music without the need for an intermediary third party (like a Universal Music, Spotify or Apple Music), directly allowing fans and their artists to interact with each other. 

## Background

Before diving into Audius and how they are looking to disrupt the music distribution space, we take a look at what the current industry looks like, and why we need these kinds of protocols to exist in order to democratize an increasingly gatekept legacy system. 

### Music Distribution is Highly Centralized, and Providers Abuse Power

There are two major aspects to music at a distribution level,

1.	[Music Rights and Ownership](https://blog.reverbnation.com/2018/05/09/music-law-101-owns-copyright-song/#:~:text=In%20general%2C%20the%20individual%20who,person%20owns%20the%20resulting%20copyrights.) – *who really owns a piece of music created?*

2.	[Music Distribution](https://soundcharts.com/blog/music-distribution) - *how is that piece of music distributed to consumers, and how it is monetized?*

When looking deeper into the two aspects above, the result may rather surprise you. It is not the artist (the creator of the music) that has a major share in ownership of the music created, nor the artist that gets to decide how and where their music is distributed and monetized. 

All these decisions are taken by centralized authorities and intermediaries like record labels, agents, and music streaming services. 

Pre-internet, the act of creating a piece of music and eventually monetizing it required lots of capital investment and administrative work (like dealing with [royalties](https://www.indiemusicacademy.com/blog/music-royalties-explained) and rights tracking) , which artists couldn’t afford and didn’t want to allocate their time towards. They outsourced this to record labels in exchange for a share of any expected future profit. While this may have seemed like a rational decision for musicians at the time, in hindsight, the upside for providing these services was so high (the record labels essentially went long artists success, VC style), that the record labels came out the biggest winners. They have managed to consolidate their position since, and today, a large amount of the artists successes, depends on the music label they sign with. 

 <img width="800" alt="image" src="https://user-images.githubusercontent.com/96482943/184709790-02e935a2-f044-45b0-aa74-128496648e60.png">


Music studios like Universal, Warner and Sony Music control a large amount of the music rights and ultimately decide who gets to do what with them, irrespective of who created the music, i.e., the artist. Owning the rights to music also means record labels can decide how that music is monetized, marketed, and distributed. The end result? They earn a lion’s share of any revenue generated, while the artist, literally, feeds on scraps.  

The two charts above are the perfect visualizations of the problems in the music distribution space today. 

* In 2021, the global music industry recorded $25.6bn in total generated revenue. The big three record labels (Universal, Sony, Warner) combined earned 68.6% of all of that revenue. The reason for this is simple – they own most of the music rights. 
* Diving a little deeper, and we see the second major problem in the space – of all the revenues generated in 2021, Intermediaries accounted for ~76%, while artists only earned 7%. The reason for this – again, artists end up giving up a large share of ownership in their music in exchange for distribution value. 

### Music is Streaming 

 <img width="700" alt="image" src="https://user-images.githubusercontent.com/96482943/184711340-57da0b4c-0fd4-4abc-b18a-9e43dbaab0a7.png">

 
COVID-19 accelerated the adoption and move towards a more digital centric world. The same can be said for the music distribution space. Today, there is one clear winner when it comes to how music is distributed (i.e., how the music ends up in the ears of the end user), and that is streaming platforms. Platforms like Spotify, Apple Music are the norm when it comes to music consumption. They provide immense value to listeners by providing them with large libraries of music available at any point in time. 

*The number of paid streaming subscriptions over the last 12 years have grown at 42% CAGR, which is incredible*

<img width="700" alt="image" src="https://user-images.githubusercontent.com/96482943/184711373-d74c1380-ee57-41b0-8277-015939dc0bfd.png">
 
Streaming platforms have translated their high demand into the driving source for revenue in the music industry today, accounting for 65% of the total amount of revenue earned by various sources. The big downside to this is that streaming protocols become price makers (since artists, and even music labels need them for music discovery), and we have seen them do so. Streaming platforms earn 20% of the total revenue generated from music. 

These arguments pretty much sum up the major problems with the current web2 music distribution architecture – artists are underpaid and undervalued relative to the value they create (unequal value distribution), and centralized entities (record labels and streaming platforms) control both content discovery as well as monetization potential. While there are other issues like royalty payments, opaque old systems etc. – we believe these are the biggest two problems within the space right now – both of which Audius looks to tackle. 

## Investment Thesis 

The Biggest Value Drivers of Music are Rewarded

Poor Rights Management and Opaque Royalty Calculations

## Industry Outlook & TAM

## Technology - How it Works 

### Network Participants

1.	**Artists** – They produce the content, and upload it onto Audius for discovery, distribution, and monetization. 
2.	**Fans** – They consume the content produced by artists, and engage with the artists and the protocol. 
3.	**Content Ledger** – This is the main ledger for the protocol, which contains the node registry, and other important information. 
4.	**Content Nodes** – These are servers that host content and permission access to it. 
5.	**Discovery Nodes** – These are the servers that are responsible for indexing the main ledger and allowing users and developers to query it.

<img width="700" alt="image" src="https://user-images.githubusercontent.com/96482943/184722834-98bb648d-e3ac-4048-a9e0-aa582da7b97e.png">

*Source: [Audius Whitepaper](https://whitepaper.audius.co/AudiusWhitepaper.pdf)*

### Content Nodes 

Content Nodes host and store all the content that the artists upload onto the protocol. Audius has an extension to IPFS called AudSP (Audius Storage Protocol), which is a decentralized storage protocol that stores all the content and metadata. Users are incentivized to run content nodes (by staking AUDIO tokens) and provide storage space to the network, by earning a share in AUDIO token emissions and a share in protocol fees. 

<img width="400" alt="image" src="https://user-images.githubusercontent.com/96482943/184724791-72d217b2-3efd-48ca-971b-60610743e690.png">

*Source: [Audius Whitepaper](https://whitepaper.audius.co/AudiusWhitepaper.pdf)*

Here’s what content nodes do: 

1.	When an artist uploads a piece of music onto Audius – it is broken up into smaller segments, and distributed across content nodes that encrypt and store the segments. 
2.	When users want to stream the music, they request access to the specific segments of music/songs they want to listen to from the content nodes that store the data. (This all happens on the back end, to users, they are just clicking “[play](https://audius.co/)”)
3.	Content Nodes allow for content permissioning functions, which can restrict who can access the content based on a set of pre-defined conditions. This is extremely useful when artists want to run their own content nodes. They could use on-chain data (like holding a specific amount of the artists token, proof of past history) to restrict access to specific pieces of music to only super fans etc. 

### Content Ledger 

The Audius Content Ledger, is a group of smart contracts deployed on the various blockchains that house various components of the protocol (Ethereum, Filecoin Solana etc.), and is the ultimate source of truth for anything that happens on the protocol. 
The Content ledger includes: 

* Audio content and metadata [format specifications](https://static1.squarespace.com/static/56d5e44060b5e9e20a94b16c/t/5b493e3f03ce642cc82b5890/1531526720147/OMI-MVI1.0-Requirements+(20170726)+(2).pdf)
* Processes for artists to track content and control ownership structure & revenue splits
* Registry of all nodes reachable on the protocol
* Social Graph for all users interacting with the protocol
* Implementations of the governance token model 

### Discovery Nodes 

Discovery nodes, similar to content nodes, are servers that Index the content ledger (where artists register new music, and the history of the network state rests), allowing artists, users and developers to query the ledger and extract valuable, important information. These nodes essentially allow for new music to be discovered on the Audius Network, as well as allow other applications to be built on top of it, using the API.  This is a massive component in providing high user experience to fans and artists alike. 

<img width="400" alt="image" src="https://user-images.githubusercontent.com/96482943/184731259-9815d59f-bee5-4cb4-893e-1cf92a5bec2f.png">

*Source: [Audius Whitepaper](https://whitepaper.audius.co/AudiusWhitepaper.pdf)*

Nodes are incentivized to provide the service by earning AUDIO token emissions and a potential share in protocol revenue. 

## Tokenomics and Protocol Mechanics

The Audius protocol is powered by the Audius platform token ($AUDIO), and 3rd-party stablecoins as well as artist-specific tokens will be supported in the future. 

### Utility

The AUDIO token has three main use cases within the network: 

* Security 
* Feature access 
* Governance 

Audius tokens are staked as collateral for a value added services. In exchange, stakers earn ongoing issuance, governance weight and access to exclusive features. Audius tokens are staked by node operators to run the Audius protocol, and by artists and curators to unlock exclusive features and services. Any $AUDIO staked within the protocol is assigned governance weight, used to shape future iterations of the protocol. Audius tokens will serve as collateral for artist-based tooling as well. 

Early examples incubated by the community include artists tokens, badges and earnings multipliers. In the future, fans may delegate tokens to specific artists and curators to share in their growth on the platform and the issuance of future tokens. Node operators must stake Audius tokens to operate a discovery node or content node, with a larger stake correlating to a higher probability of being chosen by fan clients. 

### Token Distribution 

**Genesis Supply:** 1,000,000,000 AUDIO

**Annual Issuance Rate:** 7% (70,000,000 AUDIO)

<img width="600" alt="image" src="https://user-images.githubusercontent.com/96482943/184735787-1d52f7a2-19e6-4d1e-beae-d0b0da534368.png">

## SWOT

### Strengths

## Catalysts 
## User Metrics
## Crypto Native Diligence 
## Team 
## Resources 



