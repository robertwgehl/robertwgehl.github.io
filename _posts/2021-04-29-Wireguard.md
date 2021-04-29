---
layout: post
author: RWG
title: Messin' with Wireguard 
tag:
    - Wireguard
comments: true
---

I've been messin' about with [Wireguard](https://www.wireguard.com/) and -- after some hiccups -- I have a small network of peers connected. I now have a couple laptops, a desktop, a phone, and a Raspberry Pi all networked, with the connection remaining persistent even as the mobile devices move across wi-fi networks. 

![The Wireguard logo](/assets/images/wireguard.svg)

<!-- more -->

My proudest achievement is connecting this network to a [Pi-hole](https://pi-hole.net/) installation on a Digital Ocean VPS. Now all those Internet ads cannot reach me, not matter where on the network I am. I should probably allow ads, since I am a media studies scholar and [ads are stable object of media studies](https://xroads.virginia.edu/~DRBR2/rwilliams.pdf). But then again, I'm addicted to things like [actually being able to read websites](https://marketingland.com/pop-up-ads-why-everyone-hates-them-and-why-theyll-never-die-273343), having them [load quickly](https://thetechieguy.com/ad-blocker-impact-internet-speed/), and [not being tracked](https://brianchristner.io/how-a-single-raspberry-pi-made-my-home-network-faster/), so... yeah, I'll pass on the ads.

Wireguard is billed as faster and easier to work with than OVPN, and in my view, it's living up to the billing. 
Setting things up initially took a long while, with my mistakes including not setting up rules in my firewalls (I use UFW). Once I figured out how to allow connections from the network I was building, it began to work quite well. And it is fast -- the network speed is nearly as fast as without the VPN in place. (In fact, I'm pretty sure my ISP, Suddenlink, is dropping packets from internet radio streams -- but with Wireguard, those packets aren't dropping). 

One tip I can offer: I discovered a need for a "PersistentKeepalive" on that Pi-hole server. This appears to be a bit of a no-no with Wireguard, which is built on the idea that "silence is golden" -- i.e., the less packets flying aorund the better. But the Pi-hole peer kept dropping off the network, and thus my DNS lookups wouldn't happen. By adding 

    PersistentKeepalive = 25

to the Pi-hole [Peer] section of the client config file, the connection stays active.

If any of you are itchin' to try some Wireguard, I have found the tutorial at [ServerSide Up](https://serversideup.net/courses/gain-flexibility-and-increase-privacy-with-wireguard-vpn/) to be really helpful. That, and my old friend "trying stuff until it works"...

![A parody of O'Reilly tech books. This cover says "Trying Stuff Until It Works"](/assets/images/try.jpg)


