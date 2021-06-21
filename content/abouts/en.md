---
title: "Introduce Yourself"
date: 2020-12-16T01:14:24+09:00
draft: false
--- 

# Info

# Basic
1995 Kanagawa, Japan

## Back born
I think the first time I became an engineer was when I saw Bloody Monday in elementary school.

My grandmother gave me a book on hacking, which cost about 8,000 yen at the time, and that was the starting point of my career.

I still like to understand how things work, and I think it is important to understand and implement things correctly in my work.

My favorite areas of technology are security, performance tuning, networking, and Linux Kernel.

I also think that algorithms are very important.

# Picking up the work so far
- I implemented a service with an expected load of 5000 RPS references, 100 RPS writes, infrastructure design, security requirements, and load testing with about 3 development members. The implementation had a lot of reads, so we used edge caching. For the load test, we used wrk2 because it was hard to put a load on it.
- Building a data pipeline with more than 10 million records Using apaceh beam, we implemented a storm infrastructure and built an ETL/ELT infrastructure using bigquery with datastore. In order to run beamSDK more quickly, we incorporated avro and gson.
- For on-demand video delivery, we implemented our own delivery infrastructure and m3u8 converter, mainly using AWS for load balancing and optimal size video conversion.

## What I've tried to do down the road.
- OSS
- Global (English speaking environment, etc.)
- Startup
- Growth
- Security
- High Performance Tuning

# Carrier
## Company
- [Yapuri Corporation](https://yappli.co.jp/) 2020    
- [CyberAgent, Inc.](https://www.cyberagent.co.jp/) 2019~2020
    - [Established a new subsidiary company Cyber Pal Inc. by new graduates informal offer](https://www.cyberagent.co.jp/news/detail/id=23000)
    - [The result of introducing gke istio to a small organization](https://cyberagent.ai/blog/pr/culture/5649/) [Hideaki Goto (Cyber Pal Inc.)

## intern
- [Abema TV Corporation](https://abema.tv/) 2018~2019
- [UUUM Corporation](https://www.uuum.co.jp/) 2017~2018
- [deBit Corporation](https://debit.co.jp/) 2017~2018

## University
- Graduate from Musashino University, Faculty of Economics, 2019
- Research Topics Game Theory Matching Theory
- Graduation Thesis The Spread of Search Engines and Consumer Behavior

# Publish
- [Up-and-coming white hackers and anti-virus software slug it out! Report on the outcome of the battle](https://news.mynavi.jp/kikaku/20180720-665544/)
- [istio-ingressgateway ssl https certificate intermediate certificate I'll introduce](https://qiita.com/hidexir/items/645b6d6cabf239d870d0)
- [Implementing an authentication proxy with Nginx and nodejs *Not basic authentication!] (https://qiita.com/hidexir/items/6d2da4e431641cbf0122)
- [The story of istio installation in GKE](https://hidexir.hatenablog.com/)

# Skill
## Lang
- Go
- Rust
- Python
- Java
- Scala
- C++
- TypeScript

## Infra
- AWS
- GCP
- Kubernetes

## editor
vim emacs (for writing Japanese)

# My Project

## [ISUCON10](https://isucon.net/archives/55008744.html)
rank #166 top 30% team yagyu

## [x86 emulator](https://github.com/hidexir/x86emu)
I made a full scratch emulator of x86 architecture execution environment with rust.

## [Video distribution service](https://wantty.app/)
This is a video distribution service. Trainers and athletes can upload their videos and watch them as streams.

## [Service using Ethereum tokens](https://www.peace-coin.org)
I was mainly in charge of the server side using the Solidity framework.

## [Personality assessment service](https://www.zelfium.com/ja/)
There are a lot of patterns for personality assessment, so please try it once. I thought a lot about the algorithm and the data structure behind the algorithm to classify the answers to the questions from the users as fast as possible.
I mainly used a tree structure and succeeded in speeding it up.

## [Zombie game](https://apps.apple.com/jp/app/escape-from-uncle/id1444505240)
Created by me and my classmate from CyberAgent days. I was very happy to see that there were even people doing [commentary](https://gameappch.com/app/?app=06132).
I mainly purchased the 3D objects and implemented the internal logic, map layout, and camera viewpoint control. Translated with www.DeepL.com/Translator (free version)