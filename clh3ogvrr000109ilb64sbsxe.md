---
title: "Project Beat~lytica"
datePublished: Sun Apr 30 2023 17:20:42 GMT+0000 (Coordinated Universal Time)
cuid: clh3ogvrr000109ilb64sbsxe
slug: project-beatlytica
canonical: https://www.linkedin.com/pulse/project-beatlytica-warui-wanjiru-/?trackingId=ZLM%2BvmXQRgqV%2By3jEbIusg%3D%3D
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1682874921473/8afd00f5-642b-4a51-9648-c4121c4bcbf5.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1682875222880/2ed765e6-99bb-40d4-a58d-6eae91bb384d.png
tags: data, kafka, dataengineering, streamprocessing, kafka-topic

---

***Welcome to my first article as a data engineer.***

Project ***Beatlytica*** is a streaming project I have been working on, and this is part 1/4 of the project. Beatlytica comes from two words: beats and analytics. The aim of this project is to come up with a live, near-real-time dashboard to analyze streaming events. The diagram above shows the architecture I used.

To begin with, I figured out that my laptop is limited in its capabilities, so why not use Google's compute engine under their $300 free credits? So I took that decision and began drawing the architecture, I figured out I'd need a scalable system, a trusted infrastructure, and at the same time, I'd need to integrate the new tools I had accumulated over time.

For resource provisioning, I chose to use Terraform. I had just learned it and wanted to explore its depths, so I challenged myself to use it to provide the Google Cloud resources I required for this project. Secondly, I used Docker to build images of the tools I needed to use: which in this part are Eventsim and Kafka.

Why Eventsim, I saw it as a simple opportunity not to reinvent the wheel, and since a repo was already there, why not use it? Eventsim generates synthetic data mimicking music-streaming events from a website such as Spotify.

To explain this architecture, Terraform simply provisioned the resources, by which I mean the compute instances I required to run the project. Secondly, I used Docker to containerize the individual processes. The first process is real-time event generation, and here is where Eventsim shines. The events are then streamed into Kafka topics. I used Kafka because of its scalability, reliability, and wide usage, so I was confident I would get support if I faced an issue.

The two containers are set to communicate within a Docker network, and the compute instance has firewall and networking permissions enabled for the service role I was using. I used SSH and VS-Code to access and run the scripts, respectively.

You can find this first part using this [link:](https://github.com/The-Algorist/Beatlytica/tree/master/kafka) The whole repo is on [Github](https://github.com/The-Algorist/Beatlytica).

Thank you for reading my first article!!