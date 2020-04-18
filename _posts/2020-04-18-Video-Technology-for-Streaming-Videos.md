---
layout: post
comments: false
title: Video Technology for Streaming Videos
permalink: /video-tech/Video-Technology-for-Streaming-Videos
---

At the most and at vast, video technology is being used to deliver videos over the Internet. Delivering videos to the users using Internet is what we call video streaming. This delivery is achieved by the continuous and real time transmission of media from server to client, let media be video or audio. It can deliver already produced videos also (VoD) or Live Streaming of events also. The most notable early use of video streaming was live streaming of *Summer Olympic Games in August 2008* using Microsoft's Smooth Streaming protocol, millions of people around the globe watched with millions of hours consumption.

## Technologies Involved
There are lots of sub-technologies involved in making video streaming possible. Here some high-level technologies used for video streaming:
- Video Encoding: Compressing original videos to reduce storage size, adding security
- Delivery Network: Video and security key storages, CDN Networks
- Streaming Protocols: Like ABR, Progressive Downloads
- Video Player: Software program on devices to decode and play delivered videos  
(Will see in more details about each of these in coming posts.)

## Streaming Protocols
Streaming protocols are responsible for putting all these technologies together on same page. These protocols defines how video should be encoded, how it should be stored, how it should be delivered and how it should be decoded and played on device.  
There are two major protocols categories are being used, ABR and Progressive Download. Out of these, progressive download is not much efficient.

### Adaptive Bitrate (ABR) Streaming
ABR Streaming is achieved by chunk-based delivery of multiple versions (wrt frame resolution and bitrate) of the same video, with the ability of player to dynamically choose the bitrate to play. And all this is done over an HTTP protocol, enabling to use existing Internet infrastructure without any changes.  
There are few common, most used ABR protocols:
- HTTP Live Streaming (HLS) by Apple
- Microsoft Smooth Streaming (MSS) by Microsoft
- HTTP Dynamic Streaming (HDS) by Adobe
- MPEG Dynamic Adaptive Streaming over HTTP (MPEG-DASH) by MPEG group

There are very tough challenges which are being tackled using ABR streaming, like:
- Reducing required bandwidth to play high quality videos
- Maintaining video quality with weak networks
- Uninterrupted playback in peak network traffics and fluctuations
- Reducing delivery network and infrastructure costs
- And many more

Ever wondered how OTT apps like Netflix, Amazon Prime Video, Apple TV+ works so smoothly? This is the technology they are using behind the scene!

Will explore more about every technology and protocol mentioned here, stay tuned at [Video Technology Posts](http://d4ttatraya.me/video-tech/).


