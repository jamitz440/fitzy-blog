---
title: 'De-Googling my life in 2025'
description: 'A dive into the decisions I made to remove google from my life after becoming a dad.'
pubDate: 'Jan 10 2026'
tags: ["privacy", "tech"]
---

### Why 2025 forced a privacy rethink

I have always been privacy-conscious but in 2025, a big change happened in my life that affected how I saw the world. I had a daughter. I wanted to have a secure way to share and store photos of her milestones with my family, which led me down the path of self-hosting away from the private giants and the AI boom.

This year I saw the rollout of invasive technologies. Mass surveillance systems such as the network of flock cameras in the United States were among them[^1]. At the same time the private giants, Google and Meta, put profits before privacy. It was a model that I didn't want to be a part of. I wanted to take control of as much of my information and data that I could, which led me to open-source, transparent applications that I can self-host.

### De-googling my phone 

The first part of the big switch was reducing my reliance on Google. I didn't trust that Google wouldn't use every part of my phone to compile data or train AI models with my emails and photos. That was a risk I wasn't willing to take now that I had a daughter. She has the right to autonomy over her digital data.

Severing my ties to the tech giants was a major shift. I have had a Google account and, have used Google software for 15 years. My phone is also a Google Pixel so it's safe to say I was deeply ingrained in their ecosystem. However, having a Pixel turned out to be a blessing. 

Ironically, the privacy-focused [GrapheneOS](https://grapheneos.org/) only works on Pixel phones. It's an OS which goes out of its way to protect your data. It doesn't bundle any Google services, instead it provides its own core apps (camera, messages, etc.) and gives you the ability to sandbox any Google processes you wish to reinstall.

If you're undecided or don't have a Pixel, this [comparison chart by eylenburg](https://eylenburg.github.io/android_comparison.htm) may help you decide what's right for you.

### Emails & cloud storage

With the operating system sorted, there was still the issue of apps. I still relied on Google for email, photos, cloud storage - basically everything.

Getting a new email account is easy; both [Tuta](https://tuta.com/secure-email) and [Proton](https://proton.me/l/free-private-email) are great choices. The laborious part is updating that email in every service you use. I chose Proton because it also offers an encrypted cloud storage giving me an alternative to Google Drive eliminating one more Google service from my roster.

### Self-hosting media

Next up to be replaced is Google photos. The replacement needed to be a service hosted on my own hardware with the ability to share pictures with my family. This is where my home server comes in. A few years prior, I had moved to self-host my own media after seeing [this](https://www.youtube.com/watch?v=RZ8ijmy3qPo) Jeff Geerling video. I run a 2 bay Synology NAS with a Jellyfin server. Synology has its own photo storage solution. I went with an open-source alternative instead: **Immich**. It's not as simple to set up on a Synology NAS as its own photos app is. If you're comfortable using Docker, it's worth it. Immich has a much cleaner UX, native phone apps, local AI image recognition, and organisation. I'll likely need to upgrade my NAS soon, the dual-core CPU is getting pushed to its limit by the AI features. Importantly, it passed the wife test - she found it just as easy to use as Google photos.
 
### Messaging

Messaging is a pain point. Not because the alternatives to WhatsApp aren't good, it's that Meta has such a hold on people that it has had to stick around. I've been able to get my wife to download Signal, an end to end encrypted messaging service, but I've had no such luck with everyone else. I was hoping I'd be able to drop WhatsApp as it's my only tie to Meta. I rely on WhatsApp for work chats, so it has to stay for now - but at least it's sandboxed in GrapheneOS. 

### Maps

Maps weren't an issue for me, I haven't used google maps in years. No maps app needs to see my web browsing history[^2]. I've been using [OsmAnd](https://osmand.net/) and [Organic Maps](https://organicmaps.app/). OsmAnd is the mobile client for OpenStreetMap and has a lot more information such as bus timetables and seemingly better pedestrian navigation. However, I have found Organic Maps to work better for navigating in the car with a cleaner UX making it easier to just glance at.

That's the full details of my 2025 privacy shift. I'll be writing an in-depth post about my home-server setup and its limitations, software I have hosted on a VPS, a self-hostable end to end encrypted notes app I am building, and any problems or solutions I have come across in the world of software. 

[^1]: [This is a great in-depth video into the flock cameras by Benn Jordan](https://www.youtube.com/watch?v=vU1-uiUlHTo)  

[^2]: Google maps requires excessive permissions including [web browsing history](https://play.google.com/store/apps/datasafety?id=com.google.android.apps.maps&hl=en_GB)
