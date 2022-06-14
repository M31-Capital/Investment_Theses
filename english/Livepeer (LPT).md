# Livepeer: Decentralized Live Video Streaming

## Overview

Video streaming today, is highly centralized. A lot of this has to do with the fact that the core infrastructure (WebRTC) cannot scale beyond 2-3 users, and that the operating costs of providing various video related services, especially streaming are really high owing to how CPU intensive the process is. This has led to a small pool of providers that control the infrastructure that is required to build live streaming applications. 

## Investment Thesis 

* Censorship Resistance 

Censorship is the main problem that has been born out of the extreme centralization of video streaming services. Platforms like YouTube dominate the industry and can dictate prices, advertising schedules, and particular narratives at will. These networks have repeatedly encroached on users’ freedoms and will continue to do so until they are knocked out of the top spots. The growing censorship taking place on these networks is a litmus test demonstrating why it’s vital to have alternatives. Livepeer enables users to get their voices heard through the power of decentralization.

* Lower Cost Streaming

By leveraging GPUs from users across the globe, Livepeer can provide HD quality streaming services in a cost-efficient manner. Lowering the cost of broadcasting and streaming will enable more opportunities for technological advancements in the sector. It will also improve profit margins for content creators. As of late, content creators have been repeatedly bullied by large streaming services. Livepeer seeks to end this mistreatment.

## Technology 

### The Livepeer Media Server

The Livepeer Media Server is a key component in the protocol tech stack. It is important to understand that when users are streaming video (live or otherwise) – they each have different hardware capabilities which means that the video output (bitrate and quality) need to be able to match. The Livepeer media server is capable of taking in video and audio input streams, and transcoding them (converting them to a suitable format for output – different output formats, bitrates etc.) so that any device, can stream the video. 

### The Livepeer Network

The Livepeer network is a collection of nodes that run the Livepeer media server, and operates on two requests: publishing streams and requesting them. 
* Publish Stream: Request to transcode a live video with certain parameters. 
* Stream Request: Request to access a current live stream that is on the network. 

<img width="600" alt="image" src="https://user-images.githubusercontent.com/96482943/173525397-ab41b629-0ef3-4203-91a0-a93b0bb90b59.png">


When a node submits a stream to the network, one can assume that the stream has been transcoded into the format that was requested (and paid for) and that the network will be able to distribute that stream to whoever on the network requests it. 

Nodes will manage their own peer and will test their peers for latency and throughput capacity to ensure that streams can be relayed through the network with minimal delay. When a stream is requested from a node who currently isn’t yet consuming it, they will either pass on the request to a node who is already consuming it and has relay capacity, or they will become a relay node themselves, consuming the stream in order to pass it on to subsequent requesters. The protocol will dictate the routing procedure to follow for requesting a stream from the proper node and routing transcoding and verification jobs to the proper nodes.
Network Participants

* Node - anyone who runs the full Livepeer software and participates in the protocol. All subsequent roles are also nodes. 

* Broadcaster - the node who is publishing a stream. They pay the network in ETH for transcoding services.

* Transcoder - a node who is currently transcoding a stream into a newly formatted stream. They get paid for this service by the broadcaster, and increase their proportion of newly generated token. Transcoder is a special role that is delegated towards by other nodes. They not only transcode video, but also participate in the security protocol of verifying work and distributing new token. 

* Consumer - a node who is consuming an output stream to watch the video or to serve it over a gateway to additional users outside of the protocol. 

* Relay node - a node who is merely passing on video without the intent of watching or serving it itself.

 <img width="600" alt="image" src="https://user-images.githubusercontent.com/96482943/173525110-4622407e-120e-4e82-8d64-f6c6e13e323e.png">


## Consensus

There are two levels of consensus in the Livepeer Protocol. The first, the state of the current ledger of the Livepeer Token balances, and validation of all transactions which transfer token from one account to another, is provided via the consensus algorithm in the underlying blockchain that the Livepeer token is issued on, i.e. Ethereum.

The second level of consensus is unique to the Livepeer protocol, and will govern how the newly generated Livepeer Token is distributed in proportion to the amount of work that nodes in the network performed in order to transcode and verify live streams. This will operate on a delegated proof of stake consensus algorithm (DPOS). 

Transcoders will be elected to play a special role in the network consisting of two responsibilities: Run highly efficient and reliable hardware and networking setups to fulfil the demand for transcoding on the network. Including proof of proper transcoding transactions on chain, which the protocol will use as input to determine the allocation of newly minted Livepeer Token. Essentially, transcoders will play an analogous role to block producers. They will earn a portion of the block reward for playing this role, and will be incentivized to act honestly, lest they lose the valuable position of holding this role.

## Tokenomics: 

* ETH is the medium of exchange token in the Livepeer network. (that is, all fees paid for use of the Livepeer network, are paid out in ETH)

* The Livepeer Token will be a protocol token for staking, used by those who want to perform work on the network, that serves the following purposes: 

1.	It serves as a bonding mechanism in a delegated proof of stake system, in which stake is delegated towards transcoders (or validators) who participate in the protocol to transcode video and validate work. 
2.	Services such as DVR, closed captioning, ad insertion/monetization, and analytics can all plug into the Livepeer ecosystem and potentially make use of the security provided by staking LPT. 
3.	This will be an inflationary token in which new token is generated by nodes who run the Livepeer Media Server and perform transcoding, in proportion to the amount of work that they contributed to the network. 
4.	Nodes who don't perform work correctly or attempt to cheat will have their token stakes slashed. This will have the effect of routing more future work, and fees, towards the nodes who have successfully performed work in the past. 
5.	Assuming competition amongst nodes to win broadcasting business and the associated fees in ETH, any increase in proportional amount of token, and hence future work, that can be earned for performing transcoding will equate to a drop in the cost that must be charged to the broadcaster. This creates a positive economic effect for broadcasters looking to transcode live video through the Livepeer Network.

## Incentive Mechanics: 

* Transcoding nodes want to transcode so that they can receive fees and increase their share of future work. 
* Transcoding nodes don’t want to cheat at transcoding, because they will be caught and get their stake slashed by a higher amount than they can expect to gain by cheating. 
* Nodes want to stake their token in order to earn fees and future work in proportion to their stake. 
* Nodes want to vote for properly acting transcoders because it ensures the efficient performance of the protocol, therefore increasing the usefulness of the network.


