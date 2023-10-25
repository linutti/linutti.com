---
title: "Self-hosted Email Using Linode and Mail in a Box"
description: "In this blog post I outline the process of me setting up a self hosted email service for myself. The reasons are simple: more pirvacy, more flexibility and, perhaps most importantly, more fun."
hidedescription: false
date: 2023-07-29T12:20:39+03:00
tags: ["email", "privacy"]
category: ["blog"]
draft: true
toc: true
disableanchors: false
disablebreadcrumbs: false
disablereadingtime: false
disablewordcount: false
editPost:
    disabled: false
---
The idea of self-hosting an email server had never really occurred to me as a possibility before.
It always seemed like one of those things that someone else should take care of
and that I would just set myself up for a world of hurt if I tried to do it myself.
But like the good old saying goes - if you want something done right, you gotta do it yourself.

I guess there's no single thing that I can point to and say *"this is the reason why I want to self-host my own email server"*.
Rather, it's a combination of a general interest in technology, increased privacy
concerns with email service providers and/or limitations of limitations within their products.

I've been a customer with Proton Mail for some time now, and I have been quite pleased with the service.
It's privacy focused (at least they claim it is, mkay) and works well for sending and receiving emails.
However, when it comes to features, it leaves a little something to be desired.
For insctance, on the **Unlimited** plan for 12,99€/month you get to use 3 custom domains and a total of 15 aliases.
The 15 aliases are enough for most people, but problems arise when you want to have separation between the aliases and your account.
The alises are configured to be able to be used to log into your account with the *"master"* password.
What if I want to set up aliases to use for account separation on other services I use?

In this case I want aliases that are either configured to not be able to log in OR inboxes separated from my main email inbox all together.
Proton makes it quite easy to set up new email accounts, which are separate from your main inbox, but as of the day I'm writing this there
is no way to actually forward all incoming email from that address to your main inbox. Cool 👍

Also, I'm not interested in having a whole suite of apps at my disposal when I pay for an email service.
I actually just want a solid ***email*** expeience. Go figure...

So then, why don't we set that up?

## Prerequisits