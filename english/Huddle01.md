# Huddle01 – Decentralising the Web2 Live Video Streaming stack

## Investment Thesis

* A Decentralized Internet Needs Decentralized Methods of Communication (ironically, most of crypto communicates and builds communities around centralized communication tools – Discord, Telegram, Twitter, Zoom)
* Current Web2 P2P Live Engagement Architecture cannot scale beyond a certain amount (currently use webRTC)
* Heavy Centralization required for scalable live video applications (AWS/SFU)
* Massive market potential for live streaming (currently creator monetization via streaming sucks) 
* Huddle will form the infrastructure layer to build streaming applications (Fat Protocol’s Thesis) – Huddle’s scaling infrastructure can see a Zoom integration. Zoom will be able to decentralize, scale and integrate web3 features to its services, directly through Huddle. 
* Strong web3 feature set – ENS integrations (ability to expand to more across different chains), token gated meetings (allows for DAOs and organizations to leverage Huddle and gate meeting entry – improving the user experience), NFT avatar integrations etc.  

## Overview

The current audio/video streaming tech stack is highly centralized – not by design, but by need. WebRTC is the backbone of any communication application we use across the internet today – and it alone cannot scale beyond 2-3 users – meaning that centralized infrastructure needs to be used in order to make ‘many to many’ streaming applications possible. Huddle has figured out how to decentralize this critical component of the tech stack, using blockchain and custom tools in order to scale webRTC, without exposing it to centralization of any sorts. Huddle aims to decentralize and scale real time engagement platforms (audio/video live streaming, audio/video conferencing etc.) through the Huddle01 protocol. 

## Background

### WebRTC

In order to establish user to user communication for live engagement applications (live streaming (twitch), audio/video conferencing (zoom), live audio streaming (clubhouse), the technology that is leveraged is called webRTC (Web Real Time Communication Protocol) – an open-source protocol that supports video, voice, and generic data to be sent between peers, allowing developers to build powerful voice- and video-communication solutions.

*webRTC is the infrastructure backbone for any sort of communication application we use today. 

The Problem with webRTC: It cannot scale because it uses a P2P mesh network. P2P, or mesh, is the easiest to set up and most cost-effective architecture you can use in a WebRTC application; it’s also the least scalable. In a mesh topology, two or more peers (clients) talk to each other directly or, when on opposite sides of a firewall, via a TURN server which relays audio, video, and data streaming to them.

Since webRTC by itself cannot scale, it uses other centralized infrastructure to scale past 3 users, and achieve high quality streams. 

### UDP (User Datagram Protocol)

it helps establish low latency and loss tolerating connections between applications on the internet by speeding up transmissions of data, by enabling the transfer of data before an agreement is provided by a receiving party (so it’s sort of like an ‘optimistic’ broadcast and does not guarantee that the data packets will go to the final destination). 

### SFU and MCU (Selective Forwarding Unit and Multipoint Conferencing Unit)

In order to scale, webRTC applications use SFU and MCU – protocols that offload the processing power (similar to how a sidechain would), allowing for faster speeds and better output quality. To put it simply, without an SFU and MCU, webRTC cannot scale beyond 2-3 users. 
 

SFU is perhaps the most popular architecture in modern WebRTC applications. Put simply, an SFU is a pass-through routing system designed to offload some of the stream processing from the client to the server (exactly like a rollup, or more accurately, a sidechain would offload transactions on from a layer 1 blockchain). Each participant sends their encrypted media streams once to a centralized server, which then forwards those streams—without further processing—to the other participants. 

Although an SFU is more upload efficient than a mesh topology—for example, on a call with n participants you have only one upstream per client rather than n–1 upstreams—clients still have to decode and render multiple (n-1) downstreams which, as the number of participants grows, will drain client resources, reduce video quality, and thus limit scalability.

In an MCU topology, each client is connected to a centralized MCU server, which decodes, rescales, and mixes all incoming streams into a single new stream and then encodes and sends it to all clients. Although bandwidth friendly and less CPU intensive on the client side—instead of processing multiple streams, clients have to decode and render only one stream—an MCU solution is rather expensive on the server side. Transcoding multiple audio and video streams into a single stream and then encoding it at multiple resolutions in real time is very CPU intensive, and the more clients connect to the server the higher its CPU requirements.

TLDR: SFU and MCU are the only options to scale webRTC, and both suck. 

Security: a DTLS session is initiated and is utilized to exchange security context and data. Audio and Video data are transferred via SRTP protocol using UDP.



## Huddle Protocol Design

![image](https://user-images.githubusercontent.com/96482943/173389908-5f04ac20-e720-4ae2-b831-fd7a8b086977.png)


Anyone can connect to Huddle to generate instant, real time communication. (If you think about it, with a link and an internet connection, Huddle enables instant communication between two individuals. Can definitely see a ‘decentralized FaceTime’ like application being built on Huddle.)

* Anyone can host a meeting
* Anyone can be a node providing bandwidth and resources. 
* Anyone can join a Huddle meeting initiated by the host. 

### Huddle Network Participants

* Node Providers: They provide verifiable services (computation) and earn network rewards in return. 
* Hosts: They are the users that start meetings and negotiate with the node providers for computational resources to host a huddle meeting. 
* Peers: They are participants in a host’s meeting. 
* Validators: They validate the proof for crypto rewards.


## Huddle Protocol Tech Stack

Huddle01 aims to provide seamless real-time communication for the Next-Gen. It will also lay a solid foundation for builders to innovate on top of it and build various client-facing applications. Huddle Provides a ready to use platform for video conferencing with a single click. They also have custom SDKs, on both mobile and web platforms for custom platform integrations. The protocol aims (and has so far proven) to scale WebRTC through a decentralized network of nodes, being able to provide live audio/video streaming infrastructure that is fast (low latency) and inexpensive (not CPU intensive) to use.

<img width="600" alt="image" src="https://user-images.githubusercontent.com/96482943/173389714-e52945b1-9e62-4a24-8b3f-418fd93dbf07.png">


## Backend Infrastructure: 

### WebRTC  

WebRTC establishes a secure SRTP ( and SCTP channels over UDP protocol to exchange Audio/Video/Data secured by DTLS protocol

Custom Media Server wrapped/signaling server (TypeScript): WebRTC is a p2p protocol and discovering peers on the internet can be problematic as they can be behind NAT, Offline, Unreachable, or engaged in other connections. Signaling is a process where the peer is able to discover another peer. 


* This is used to expose the SFU written in C++ through our NodeJS wrapper in the form of APIs
* Uses STUN and TURN to bypass NAT
* This uses WebSockets to signal peers and helps establish WebRTC connections
* These APIs and the WebSocket connection together helps ensure efficient and reliable communication between the clients and the media server

SFU is written in C++ bridged with NodeJS: Huddle has deployed the following tech to handle real-time scalability
Tested with a capacity of ~300 users in a single room (4 publishers with 300+ subscribers) on a single 4-vCPU system.
Configurable codecs ( Vp8, Vp9, AV1, Opus): Huddle has enabled users to choose and switch between whatever codecs are available and want to use. (codecs are hardware or software based processes that compress and decompress large amounts of data)

### Simulcast 
Since all the users in the room will have varied set of internet bandwidths, we enabled simulcast that essentially upgrades/downgrades video resolution in real-time for all users depending on the internet bandwidths
Simulcast is a technique by which a WebRTC client encodes the same video stream twice in different resolutions and bitrates and sends these to a router who then decides who receives which of the streams.

### Multithreading (Vertical Scaling) 

Since JavaScript is single-threaded, the capabilities of the system remained limited to a single worker’s capability, physically. We solved this by having all workers in a system share that work-load. This approach of distributing work-load amongst workers in a server is called multi-threading
Cascaded SFU (Horizontal Scaling). The capabilities of the system/room remained limited because of the limitation to only one computer. The solution to this problem is by having multiple servers share the workload, the same way multiple workers helped solve the workload. This approach of connecting multiple servers so as to share the server-load amongst themselves is called cascading SFUs.

### LastN 

The capabilities of being able to host (server-side) or consume (client-side) an A/V call for an individual are limited by two factors: 
* The hardware on the computer
* The internet bandwidth on the computer

Since these factors cannot be scaled after a point, Huddle implements a selective-video forwarding algorithm: Last N. This algorithm only forwards N number of video streams, irrespective of total users in the room, based on their priority/need in the room. You don’t really want to see everybody in the room.

### Recorder

A microservice is responsible for recording the meetings. We have a browser instance spawned server-side through a Puppeteer script that records the meeting-room, transcodes the video through FFmpeg, and then sends it to the Uploading Service that takes care of uploading it to IPFS and S3 (wherever necessary)

### Live Streaming

Fork of Huddle's Recorder Service that essentially transcodes the video input from the Puppeteer script and sends it to their live-streaming partners for live broadcasts

### TURN servers

A lot of people in the world are behind NAT which disables them from visiting certain domains etc - TURN allows users to proxy their A/V packets through secure channels on ports which ultimately allows them a secure seamless communication experience

### Filecoin storage

Processes the files to content addressable form ie CAR files and automatically sends deals to Filecoin miners with good reputations. This service also maintains auto deal structuring and offline file transfers for Filecoin miners. On testing the service was doing 4+ TB of storage per day with a replication factor of 10. For caching, processing, buffering, backup, and temporary storage the service uses IPFS and S3.

### Web3 APIs

Huddle can integrate the below APIs to create web3 native features, like token gated meetings, NFT avatars, ENS integrations, Decentralised Storage, and Decentralised video transcoding 

<img width="800" alt="image" src="https://user-images.githubusercontent.com/96482943/173389561-72453b58-0266-4202-897d-b458b212f826.png">

 
## Business Model 

Pay for access to web3 native API and SDK. 

### Pricing: 
* Audio/Video - $0.003/user/min
* Recording - $0.001/min
* RTMP out - $0.01/min

## Team 

<img width="800" alt="image" src="https://user-images.githubusercontent.com/96482943/173389271-e1c7913c-9191-49f7-9b31-f417237ba5a9.png">

Questions: 

* Huddle uses validators (dPoS) for governance and essentially creates an L2 for data availability? 
* What do the consensus algorithms look like? 
* What is libp2p?
* How will users pay for mins? Will there be a subscription-based model that offers users specific number of mins? Or will payment be routed through the protocol token?
* Open-source risk: can applications leverage the HRTP and HRTCP protocol directly (as in, without an SDK) and build out their own versions without routing through the Huddle protocol?
* How does HRTP and HRTCP work specifically? 



