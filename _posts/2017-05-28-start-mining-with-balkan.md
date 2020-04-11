---
layout: post
title: "Start mining with Nimiq Balkan Pool"
description: "Everything you need to start mining with Nimiq Balkan Pool"
categories: [demo]
tags: [demo, jekyll]
redirect_from:
  - /2017/05/27/
---

> This is code blocks and highlighting test page for [Simple Texture][Simple Texture] theme.

* Kramdown table of contents
{:toc .toc}
# About Balkan Mining Pool

Balkan Mining Pool is a NIMIQ Pool founded in March 2020 by a group of friends in order to support and share knowledge about NIMIQ throughout Balkan countries. 

Minimum payout is 10 NIM and payouts happen automatically every 2 hours.

Current pool fee is 1% and we don't plan on increasing it.

# Create A Nimiq Address

Visit [Nimiq's Wallet](https://safe.nimiq.com) to create an address. Always verify you are visiting https://safe.nimiq.com

Remember to store your private key by saving your Login File, Password and 24 words. **If you lose your 24 words you lose your NIM**. Keep it safe.

Once you have a Nimiq Address, store it for later.

# Install the Nimiq Miner

- **With CPU**: Download the [community GPU miner](https://github.com/tomkha/nq-miner)
- **Windows Miner**: Try out Nimiq Desktop, a graphical miner built by the community.
- **Linux Miner and Windows Terminal**: Download the official [Nimiq Miner](https://www.nimiq.com/developers/downloads/).

# Configure the miner

By adding '//' at the beginning of a line you disable it. This is called commenting a line

Comment the following lines:

	cert: “./my.domain.cer”, -> //cert: “./my.domain.cer”,
	key: “./my.domain.key” -> //key: "./my.domain.key"

Configure this line (note that you also need to uncomment it) :

	//protocol: “wss”, -> protocol: “dumb”,

In the miner section, configure the miner to be enabled (you only have to uncomment it):

	//enabled: “yes”, -> enabled: “yes”,

In the pool mining section, enable pool mining by uncommenting the line:

	//enabled: “yes”, -> enabled: “yes”,

Configure Balkan Pool

	//host: “pool.domain”, -> host: “balkanminingpool.com:8444”,

Add your address

And finally start the miner.
