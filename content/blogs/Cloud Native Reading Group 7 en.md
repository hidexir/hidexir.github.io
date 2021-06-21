---
title: "Cloud Native Reading Group #7: runc"
date: 2021-05-19T20:00:00+09:00
draft: false
---
# Introduction
This is a blog about my daily life.

Hello, I attended this event through the introduction of Mr. Ohtsubo of wantedly.

You can see the content of the day here.

https://zenn.dev/potsbo/scraps/f6bad62e1ac6ac


# text
I'm sure many of you are not familiar with the term "runc".

I've been working with docker as an engineer for a while now, and there are many cases where I touch it unconsciously.

A simple history of docker can be found here.

https://eng-blog.iij.ad.jp/archives/1478

Originally, docker had the same name for its engine and runtime.

Originally, docker had the same name for the engine and runtime, but there was a movement to separate the interface from the runtime inside. The reason for this is that it was originally separated as a module, and the background is to increase versatility.

Kubernetes and other container orchestrations also want to handle runc internally, so it is not surprising that they are starting to provide it as an API.

And runc is called low level runtime, which is the lowest layer.

These are very interesting.

There is a Japanese container runtime, Hakoniwa https://github.com/haconiwa/haconiwa.
The above is probably not OCI compliant. The above is probably not OCI compliant, so it may not be usable for Kuber's runtime.

There is also gVisor, a secure container made by Google.

This is a document presented by a friend of mine, and it is very easy to understand.

https://speakerdeck.com/moricho/gvisordeshi-xian-surukorekarafalsekontenasekiyuritei


# Impressions
It was very useful for me because I wanted to know about runc as the most important project! Thank you very much.
# Reflection
I would like to get my own room at night time and have more conversations.