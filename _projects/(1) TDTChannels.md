---
name: TDTChannels
tools: [Platform, Web, Android, React]
image: https://pbs.twimg.com/profile_banners/1247826931732578306/1586354529/1500x500
description: Community-driven platform to discover Spanish TV and radio streams, legally and for free.
featured: true
status: active
---

**TDTChannels** is a community-driven platform that allows users to discover and watch Spanish
free-to-air TV channels and listen to radio streams online, legally and at no cost.

The platform focuses on providing a simple and reliable way to access public broadcasts over the
internet, without ads, paywalls, or proprietary ecosystems. It is actively maintained and evolves
based on both user feedback and changes in broadcasters’ streaming availability.

At its core, TDTChannels is powered by an **open-source database** published on GitHub, where the
community can propose new streams or updates. All submissions are reviewed and validated before
being published, ensuring quality, consistency, and legal compliance.

TDTChannels operates at production scale and serves thousands of users on a daily basis. Around the
platform, an active community has formed, particularly through its Telegram channel, where users
share feedback, report issues, and discuss updates.

## Web Platform

The web version of TDTChannels is implemented as a client-side application built with **React**
and **GoHugo**, designed to be lightweight, fast, and easy to use across devices. The application
consumes the curated channel data (via our architecture and backend) and runs entirely in the browser.

Although the web client itself is closed source, its behavior and logic can be inspected in the
browser, as all execution happens on the client side.

![preview](https://pbs.twimg.com/media/EgC8Gk4X0AUgRtU?format=jpg)

## Android App

TDTChannels is also available as a **native Android application**, providing a tailored experience
for mobile devices and Android TV (including SmartTVs and FireTV devices).

In addition to consuming the main channel list, the app includes a custom discovery mechanism to
surface additional legally available streams. The Android app is actively maintained and distributed
through official channels.

Earlier versions of the app were open source; the last public release remains available on GitHub
for reference, while the current version is maintained as a closed-source application.

<div>
<img style="float: left" src="https://www.tdtchannels.com/tdtchannels_android_tv_1.png" width="400"/>
<img style="float: right" src="https://www.tdtchannels.com/tdtchannels_android_tv_2.png" width="400"/>
</div>

<br>

## Architecture & Infrastructure

In addition to the client applications, TDTChannels relies on a small, purpose-built backend service
implemented in **Python**, responsible for serving a curated and validated JSON feed consumed by
both the web and Android clients.

This lightweight backend acts as a stable integration layer between the open-source database and
the different client applications, allowing controlled updates, validation, and distribution of
the data without exposing the raw source directly.

The platform is delivered behind **Cloudflare** and served through **Nginx**, providing caching,
basic protection, and reliable content delivery. This setup allows TDTChannels to remain simple
in its architecture while being robust enough to handle production traffic and daily usage spikes.

<p class="text-center">
{% include elements/button.html link="https://tdtchannels.com/" text="Visit TDTChannels" %}
</p>
