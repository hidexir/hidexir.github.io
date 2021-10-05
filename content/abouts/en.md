---
title: "Introduce Yourself"
date: 2020-12-16T01:14:24+09:00
draft: false
--- 

# Info
# Intro
Thank you for your interest.  
I'm a software engineer. I like computer basics to applications.  
I also have a [FAQ]({{< ref "/blogs/faq.md" >}}), so I hope you will have a look at that.

## Basic
- Born in 1995

## Carrier
- [Yapuri Corporation](https://yappli.co.jp/) 2020~    
- [CyberAgent, Inc.](https://www.cyberagent.co.jp/) 2019~2020
    - [New subsidiary company Cyber Pal Inc. established by new graduates](https://www.cyberagent.co.jp/news/detail/id=23000)
    - [The result of introducing gke istio to a small organization](https://cyberagent.ai/blog/pr/culture/5649/) [Hideaki Goto (Cyber Pal Inc.)
    - [Abema TV Inc](https://abema.tv/) 2018~2019
- [UUUM Corporation](https://www.uuum.co.jp/) 2017~2018
- [deBit Corporation](https://debit.co.jp/) 2017~2018

# Picking up *Content is more than technology.
## Tech lead work in live streaming.
Developing a 1:1:N live streaming service with an expected load of over 5000 RPS.  
Because of the large scale of the project, we used Go language and Kubernetes (GKE) for the backend infrastructure. We also tried to use istio for the entire network. It was a tough project with load tests and security requirements, but it was developed by a small group of people.  
Originally, we tried to create our own streaming video distribution using m3u8, but in the end, all the important internal parts were created using Go, such as the combination of infrastructure costs and the use of external SDKs for the distribution part.  
We also tuned the performance of Go itself and achieved 1000RPS in 1core for READ. We also achieved 100 to 300 RPS for writing, using all the resources of the machine.  
For security, I was mainly in charge of the infrastructure and backend, including the vendor. We used burpsuite to double-check the impact on the service in case of communication tampering, SQL, CSRF, authentication, etc. with the vendors based on the attacks.  
## Data pipeline construction
We aggregated more than 3TB of data daily and created a dashboard (like a management screen where you can see various data) for a multi-tenant platform.  
Because of the large amount of data, we adopted GCP's data flow. The reason is that it is cheap and fully managed.  
Also, there were a lot of internal conversion processes, so I used Apache beam SDK (java) to create my own templates. Also, to speed up the process, I used Avro to serialize the internal data, which greatly reduced the amount of data and increased the speed.  
For reference, see [Mercari case study](https://engineering.mercari.com/blog/entry/mercari-dataflow-template/) and [open source](https://github.com/mercari/). DataflowTemplate).  
# Back born
I have always liked computers since I was little. At that time, I mainly surfed the net and read books on simple programs to see what I could do.  
When I was in college, I took a front-end job and started working on the back-end and infrastructure more seriously.  
I built a json parser with Rust for a virtual currency business and developed ads for Abema TV.  
At the time, I had a vague idea of becoming a Google engineer because I liked the lower layers, but I felt that I didn't have the algorithms or English skills, so I joined CyberAgent to develop Abema, thinking that it would give me the most power in Japan.  
# Publish
- Up-and-coming white hackers and anti-virus software go head-to-head! Report on the end of the battle](https://news.mynavi.jp/kikaku/20180720-665544/)
- [istio-ingressgateway ssl https certificate intermediate certificate I'll introduce](https://qiita.com/hidexir/items/645b6d6cabf239d870d0)
- [Implementing an authentication proxy with Nginx and nodejs *Not basic authentication!] (https://qiita.com/hidexir/items/6d2da4e431641cbf0122)
- [The story of istio installation in GKE](https://hidexir.hatenablog.com/)

# Skill
In general, I have a lot of skills when I'm working properly, so I'm focusing on what I like and what I'm good at.
# # Cloud 
I can do DB, network, storage, and system design for creating AWS and GCP services. I've also done on-premise development (VPS).
## Lang
Go Rust Python Java Scala C++ TypeScript
## Keywords
Kubernetes Terraform Fastly Nginx Istio Envoy
## editor
If you like vim, let's talk.
# Hobby
## [ISUCON10](https://isucon.net/archives/55008744.html)
I got rather high rank.
rank #166 team yagyu
## ISUCON9
I think I was about halfway there.
## [x86 emulator](https://github.com/hidexir/x86emu)
I made a full-scratch emulator of the execution environment for the x86 architecture with rust.
The scrap is here: https://zenn.dev/hidexir/scraps/e110b61cdf1857
## [Sports knowledge sharing service](https://wantty.app/)
This is a video distribution service. Trainers and athletes can upload their videos and watch them as streams. Mainly around video distribution and infrastructure.
## Service using Ethereum tokens.
As a hobby, I mainly worked on the server side using the Solidity framework.
## [Personality assessment service](https://www.zelfium.com/ja/)
There are a lot of patterns for personality assessment, so please try it. I thought a lot about the algorithm and the data structure behind the algorithm to classify the answers to the questions from the users as fast as possible.
I mainly used a tree structure and succeeded in speeding it up.
## [Zombie game](https://apps.apple.com/jp/app/escape-from-uncle/id1444505240)
I created this game with my classmate from CyberAgent. [An explanation blog was written!] (https://gameappch.com/app/?app=06132), and I was very happy to see that some people were even doing it.
I mainly purchased the 3D objects and implemented the internal logic, map layout, and camera viewpoint control.
