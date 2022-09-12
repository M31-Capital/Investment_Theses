# Huddle01 

## Overview

Huddle uses blockchain node to node architecture and custom tools in order to scale webRTC, without exposing it to centralization of any sort which will scale real time engagement platforms (audio/video live streaming, audio/video conferencing etc.) through the Huddle01 protocol.


## Investment Thesis


**A Decentralized Internet Needs Decentralized Methods of Communication**

If the internet has to be truly open, a communication needs to be truly decentralized as well. Current web communication architecture has had to be centralized, which has led to no guarantees of data privacy while using these platforms. In Web3, even today, while most of the internet tech stack is getting progressively decentralized, communication seems to be lagging the rest. The lack of market ready alternatives has been a main reason that web3 communities still use centralized video conferencing applications like zoom, or google meet. Given that data sensitivity in communication is very high, privacy and security are of utmost importance.  

**Web2 P2P Live Engagement Architecture Cannot Scale Beyond A Certain Amount** 

Given the nature of WebRTC, which cannot scale (by itself) at all beyond 2 participants, centralized intermediaries form a middleware layer that allows WebRTC to scale at the cost of security, data loss, quality guarantees etc. Huddle looks at scaling the real time communication protocol by using node to node architecture (blockchains) as opposed to the peer-to-peer architecture it follows today, unlocking lower costs, high throughput, and ultimately, higher quality streaming. 

**Massive Market Potential for Live Streaming (Creator Monetization via Streaming is Poor)** 

There is a massive market for live video streaming. Driven primarily by the parabolic increase in demand and popularity in gaming, live streaming applications like Twitch and Patreon have established strong product market fit, by appealing to more niche creator audiences (than a YouTube would) and enabling some sort layer of creator monetization. It goes without saying that these monetization levers come with their set of drawbacks (take rates, IP ownership issues, privacy concerns etc.) that harm creators in the long run. 

Huddle’s livestreaming SDK infrastructure will allow smaller, individual creators to spin up a livestreaming set up for their own niche audiences, without any need for a middle entity, while having total ownership of content IP, and monetization control.


**Huddle Will Form the Infrastructure Layer for Streaming Across the Internet**

The Bull case for Web3 is that it provides cheaper, more scalable products than its web2 counterparts. As long as the user experience is great, frictionless and the overall product is more cost efficient, demand will accrue. Owning to the current macroeconomic environment, We see the next 2 years play out in a manner where organizations of all sizes that feel the pressure to shrink their bottom lines resort to multiple cost cutting measures, making Huddle an attractive destination for organizational communication. Huddle’s infrastructure could see potential Zoom integrations, or a Twitch Integration. 

**Strong Web3 Feature Set**
 
ENS and Unstoppable Domains integrations (ability to expand to more across different chains), token gated meetings (allows for DAOs and organizations to leverage Huddle and gate meeting entry – improving the user experience), NFT avatar integrations etc. provide a very unique set that unlocks interesting feature capabilities to the protocol that can differentiate it from any other Web2 streaming platform.

## Industry Outlook 

The current audio/video streaming tech stack is highly centralized – not by design, but by need. WebRTC is the backbone of any communication application we use across the internet today, and the problem is that it alone cannot scale beyond 2-3 users, meaning that centralized infrastructure needs to be used in order to make ‘many to many’ streaming applications possible. 

Huddle01 doesn’t have much competition within the Web3 space directly, as nobody in building towards scaling the infrastructure itself. Given that the core infrastructure itself is open source, we can look at video conferencing, and streaming applications built on top of the infrastructure to quantify the TAM of the market, and what value Huddle could potentially capture. 

<img width="600" alt="image" src="https://user-images.githubusercontent.com/96482943/189664005-f8469369-ab69-4666-8c8e-e0b7a3d430e9.png">

Rapidly catalyzed by second order effects of Covid-19 (mainly, remote work), video conferencing applications went from being a once in a while used application, to the daily driver for anyone in any sort of working environment. A quick look at Zoom’s statistics during 2020 and 2021 will put into perspective just how much this space has grown, and will continue to grow, going forward. 

Currently, valued at roughly $8bn, the global video conferencing market is expected to grow to $50bn by 2025. Zoom dominates the space with ~50% market share, as it established itself as the de facto application for video conferencing. Google, Microsoft and Cisco make up a majority of the rest of the market, while much smaller players only have ~4% share. 

## What the Current Technical Architecture for Real Time Communication Looks Like

### WebRTC

In order to establish user to user communication for live engagement applications (live streaming (twitch), audio/video conferencing (zoom), live audio streaming (clubhouse), the technology that is leveraged is called webRTC (Web Real Time Communication Protocol) – an open-source protocol that supports video, voice, and generic data to be sent between peers, allowing developers to build powerful voice- and video-communication solutions.

WebRTC is the infrastructure backbone for any sort of communication application we use today. Here is a list of applications that leverage WebRTC infrastructure. You will notice there are over 

The Problem with WebRTC is that it cannot scale because it uses a P2P mesh network. 

P2P, or mesh, is the easiest to set up and most cost-effective architecture you can use in a WebRTC application; it’s also the least scalable. In a mesh topology, two or more peers (clients) talk to each other directly or, when on opposite sides of a firewall, via a TURN server which relays audio, video, and data streaming to them.

<img width="700" alt="image" src="https://user-images.githubusercontent.com/96482943/189664267-6bb4fd64-c63b-498b-ab72-c9d35d144c56.png">

*WebRTC Mesh Network*

## Scaling WebRTC

<img width="700" alt="image" src="https://user-images.githubusercontent.com/96482943/189666904-2c634a4a-6e66-40de-ada2-b5bec4144b72.png">

Since WebRTC by itself cannot scale, it uses other centralized infrastructure to scale past 3 users, and achieve high quality streams. 

### UDP (User Datagram Protocol)

it helps establish low latency and loss tolerating connections between applications on the internet by speeding up transmissions of data, by enabling the transfer of data before an agreement is provided by a receiving party (so it’s sort of like an ‘optimistic’ broadcast and does not guarantee that the data packets will go to the final destination). 

### SFU and MCU (Selective Forwarding Unit and Multipoint Conferencing Unit)

In order to scale, webRTC applications use SFU and MCU – protocols that offload the processing power (similar to how a sidechain would), allowing for faster speeds and better output quality. To put it simply, without an SFU and MCU, webRTC cannot scale beyond 2-3 users. 
 
### SFU (Selective Forwarding Unit) 

<img width="550" alt="image" src="https://user-images.githubusercontent.com/96482943/173418905-208d99f9-c809-4b0d-b69e-f50bfbeab296.png">

SFU is perhaps the most popular architecture in modern WebRTC applications. Put simply, an SFU is a pass-through routing system designed to offload some of the stream processing from the client to the server (exactly like a rollup, or more accurately, a sidechain would offload transactions on from a layer 1 blockchain). Each participant sends their encrypted media streams once to a centralized server, which then forwards those streams—without further processing—to the other participants. 

Although an SFU is more upload efficient than a mesh topology—for example, on a call with n participants you have only one upstream per client rather than n–1 upstreams—clients still have to decode and render multiple (n-1) downstreams which, as the number of participants grows, will drain client resources, reduce video quality, and thus limit scalability.

### MCU (Multipoint Conferencing Unit)

<img width="550" alt="image" src="https://user-images.githubusercontent.com/96482943/173419307-9f3fd35b-1581-4df8-ae73-7f7935df7068.png">

In an MCU, each client is connected to a centralized MCU server, which decodes, rescales, and mixes all incoming streams into a single new stream and then encodes and sends it to all clients. Although bandwidth friendly and less CPU intensive on the client side—instead of processing multiple streams, clients have to decode and render only one stream—an MCU solution is rather expensive on the server side. Transcoding multiple audio and video streams into a single stream and then encoding it at multiple resolutions in real time is very CPU intensive, and the more clients connect to the server the higher its CPU requirements.

TLDR: SFU and MCU are the only options to scale webRTC, and both are value extractive.

<img width="600" alt="image" src="https://user-images.githubusercontent.com/96482943/173419515-bb10b74f-b2f4-41a5-9c35-3750bbb85ae9.png">

## Technology 

### Huddle01 Protcol Tech Stack

Huddle01 aims to provide seamless real-time communication for the Next-Gen. It will also lay a solid foundation for builders to innovate on top of it and build various client-facing applications. Huddle Provides a ready to use platform for video conferencing with a single click. They also have custom SDKs, on both mobile and web platforms for custom platform integrations. The protocol aims (and has so far proven) to scale WebRTC through a decentralized network of nodes, being able to provide live audio/video streaming infrastructure that is fast (low latency) and inexpensive (not CPU intensive) to use.

<img width="600" alt="image" src="https://user-images.githubusercontent.com/96482943/173389714-e52945b1-9e62-4a24-8b3f-418fd93dbf07.png">

**WebRTC**  

WebRTC establishes a secure SRTP ( and SCTP channels over UDP protocol to exchange Audio/Video/Data secured by DTLS protocol

Custom Media Server wrapped/signaling server (TypeScript): WebRTC is a p2p protocol and discovering peers on the internet can be problematic as they can be behind NAT, Offline, Unreachable, or engaged in other connections. Signaling is a process where the peer is able to discover another peer. 


* This is used to expose the SFU written in C++ through our NodeJS wrapper in the form of APIs
* Uses STUN and TURN to bypass NAT
* This uses WebSockets to signal peers and helps establish WebRTC connections
* These APIs and the WebSocket connection together helps ensure efficient and reliable communication between the clients and the media server

* SFU is written in C++, bridged with NodeJS: Huddle has deployed the following tech to handle real-time scalability, tested with a capacity of ~300 users in a single room (4 publishers with 300+ subscribers) on a single 4-vCPU system.

* Configurable codecs ( Vp8, Vp9, AV1, Opus): Huddle has enabled users to choose and switch between whatever codecs are available and want to use. (codecs are hardware or software based processes that compress and decompress large amounts of data)

**Simulcast**

Since all the users in the room will have varied set of internet bandwidths, Huddle enables *Simulcast*, that essentially upgrades/downgrades video resolution in real-time for all users depending on the internet bandwidths. Simulcast is a technique by which a WebRTC client encodes the same video stream twice in different resolutions and bitrates and sends these to a router who then decides who receives which of the streams. 

**Multithreading (Vertical Scaling)** 

Since JavaScript is single-threaded, the capabilities of the system remained limited to a single participant's capability to physically ship code. Huddle has solved this by having all participants in a system share that work-load. This approach of distributing work-load amongst participants in a server is called multi-threading

**Cascaded SFU (Horizontal Scaling)**

The capabilities of the system/room remained limited because of the limitation to only one computer. The solution to this problem is by having multiple servers share the workload, the same way multiple workers helped solve the workload. This approach of connecting multiple servers so as to share the server-load amongst themselves is called cascading SFUs.

**LastN** 

The capabilities of being able to host (server-side) or consume (client-side) an A/V call for an individual are limited by two factors: 
* The hardware on the computer
* The internet bandwidth on the computer

Since these factors cannot be scaled after a point, Huddle implements a selective-video forwarding algorithm: Last N. This algorithm only forwards N number of video streams, irrespective of total users in the room, based on their priority/need in the room. You don’t really want to see everybody in the room.

**Recorder**

A microservice is responsible for recording the meetings. We have a browser instance spawned server-side through a Puppeteer script that records the meeting-room, transcodes the video through FFmpeg, and then sends it to the Uploading Service that takes care of uploading it to IPFS and S3 (wherever necessary)

**Live Streaming**

Fork of Huddle's Recorder Service that essentially transcodes the video input from the Puppeteer script and sends it to their live-streaming partners for live broadcasts

**TURN servers**

A lot of people in the world are behind NAT which disables them from visiting certain domains etc - TURN allows users to proxy their A/V packets through secure channels on ports which ultimately allows them a secure seamless communication experience

**Filecoin storage**

Processes the files to content addressable form ie CAR files and automatically sends deals to Filecoin miners with good reputations. This service also maintains auto deal structuring and offline file transfers for Filecoin miners. On testing the service was doing 4+ TB of storage per day with a replication factor of 10. For caching, processing, buffering, backup, and temporary storage the service uses IPFS and S3.

### Web3 APIs

Huddle can integrate the below APIs to create web3 native features, like token gated meetings, NFT avatars, ENS integrations, Decentralised Storage, and Decentralised video transcoding 

<img width="800" alt="image" src="https://user-images.githubusercontent.com/96482943/173389561-72453b58-0266-4202-897d-b458b212f826.png">

## Huddle Protocol Mechanics 

 ![image](https://user-images.githubusercontent.com/96482943/189667944-3b1776ed-276d-474e-96c5-bed218bdde64.png)

Anyone can connect to Huddle to generate instant, real time communication. (If you think about it, with a link and an internet connection, Huddle enables instant communication between two individuals. Can definitely see a ‘decentralized FaceTime’ like application being built on Huddle.)

* Anyone can host a meeting
* Anyone can be a node providing bandwidth and resources. 
* Anyone can join a Huddle meeting initiated by the host. 

Huddle Network Participants

* Node Providers: They provide verifiable services (computation) and earn network rewards in return. 
* Hosts: They are the users that start meetings and negotiate with the node providers for computational resources to host a huddle meeting. 
* Peers: They are participants in a host’s meeting. 
* Validators: They validate the proof for crypto rewards.

## Protocol Performance Metrics 

## Business Model 

**Huddle01’s Application Layer** 

A subscription model for access to the product, with a freemium version always available.

•	Personal Pro – Upto 50 Participants 
•	Business – For large meetings upto 100 participants 

<img width="400" alt="image" src="https://user-images.githubusercontent.com/96482943/189668227-5f9ea4c5-02f4-48c3-ada2-0030077a03eb.png">

Add ons: 

* Additional Storage: (1 TB - 20$, 3 TB - 50$, )10 TB - 100$
* Large Meetings ($10 per event, $50 monthly or $500 yearly)
* Call Analytics ($500/year)
* AR Filters (TBD)
* Custom Livestreaming (on YT, FB) 

**Huddle01’s Infrastructure Layer (SDKs/APIs)**

Pricing for SDKs will be based on utilization (the total number of participant minutes consumed), and the fee varies based on quality of video demanded. Each plan comes with 10,000 free minutes/month and priority support 

<img width="310" alt="image" src="https://user-images.githubusercontent.com/96482943/189668440-c314c24a-38cd-4874-b5c5-21fbe7f7433d.png">

*Participant Minutes = Total Number of Participants x Call Duration*

Add ons: 

•	Call Analytics ($500/year)
•	AR Filter Support
•	Custom Livestreaming (on YT, FB)

## Competitive Landscape

<img width="700" alt="image" src="https://user-images.githubusercontent.com/96482943/189668595-d850b3c3-9194-48fe-8750-fdd5dab84ed4.png">

## Team 

Co-Founder & CEO: [Ayush Ranjan](https://twitter.com/ranjan3118) 

Co-Founder & CTO: [Susmit Lavania](https://twitter.com/Susmit_Lavania) 

Team Size: 20+ 

<img width="800" alt="image" src="https://user-images.githubusercontent.com/96482943/173389271-e1c7913c-9191-49f7-9b31-f417237ba5a9.png">

## Resources 

* [Website](https://huddle01.com/)
* [Github](https://github.com/Huddle-01)
* [Twitter](https://twitter.com/huddle01com)
* [Discord](https://t.co/p4v456GDHG)



