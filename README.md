# Awesome-Hardware-AI-Agents

## Top Hardware AI Agents Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Wearable AI Devices, Embedded Agent Runtimes & Self-Hosted Hardware Automation*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Hardware AI Agents**. These tools and devices embed autonomous AI capabilities into physical hardware—pendants, glasses, pins, microcontrollers, and phones—enabling agents to perceive the environment, make decisions, and act on the user's behalf without relying entirely on cloud services.



**Examples** include Rabbit R1, Humane AI Pin, Limitless Pendant, Ray-Ban Meta, Brilliant Monocle, Plaud Note, Apple Vision Pro, and Meta Quest 3 (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, resurrecting abandoned hardware, and running agent loops on microcontrollers—ideal for makers, embedded engineers, and users who refuse to let proprietary devices become e-waste. The open-source landscape is anchored by **ESP32 iPhone Agent** (turning a $7 board into an iPhone-controlling agent), **OpenPin** (reviving bricked Humane AI Pins), **PycoClaw** and **ESP-Claw** (full agent runtimes on ESP32), and **Open Study Buddy** (a low-cost educational agent platform).



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)



## Sector Overview & Market Dynamics

The wearable AI and hardware agent market is estimated at USD $35B‑$45B and projected to exceed USD $200B+ by the 2030s, expanding at a CAGR of 25%–35%. The sector is **moderately to highly fragmented**, characterized by big-tech platform ecosystem dominance (Apple, Meta) competing against specialized startup form factors (smart audio/lifeloggers, AI pins, and AR monocles) where software orchestration and multi-modal edge execution remain unstandardized.



## SaaS/Hosted Platforms

| Company / Product | Valuation / Revenue | Starting Pricing Tier | Free Tier Limits | Description |
| :--- | :--- | :--- | :--- | :--- |
| **[Apple Vision Pro](https://www.apple.com/apple-vision-pro/)** (Apple) | **~$3.5T Market Cap** / $391B Annual Revenue | $99/year (Apple Developer Program starting tier; hardware starts at $3,499) | Xcode SDK & visionOS simulator free forever; on-device personal testing free without App Store distribution | Spatial computing headset with high-resolution displays and eye/hand tracking, running visionOS with native apps and AI features. |
| **[Meta Quest 3](https://www.meta.com/quest/)** (Meta Platforms) | **~$1.7T Market Cap** / $164B Annual Revenue | $7.99/month (Meta Quest+ / Horizon+ game & app catalog subscription) | 1-month free trial for standalone signups; 3 to 6-month free trial bundled with eligible headset purchases | Mixed reality headset with passthrough cameras and hand tracking, supporting VR/AR spatial apps and Meta AI integration. |
| **[Ray-Ban Meta](https://www.meta.com/smart-glasses/)** (Meta Platforms / EssilorLuxottica) | **~$1.7T Market Cap** (Meta) / $164B Annual Revenue | $19.99/month (Meta One Premium for expanded AI audio features) | 3 hours/month free for AI Conversation Focus voice isolation; standard capture/voice queries free forever | Smart glasses with built-in camera, spatial audio, and Meta AI voice query integration. |
| **[Plaud Note](https://www.plaud.ai/)** (Plaud / Nicebuild) | **~$1B‑$2B Valuation** / $100M ARR | $17.99/month (or $99.99/year for Plaud Pro) | 300 minutes/month free transcription & summarization resets monthly on Starter plan | Credit-card-sized AI voice recorder with transcription, speaker labeling, and AI summarization templates. |
| **[Humane AI Pin](https://humane.com/)** (Acquired by HP) | **$116M Acquisition Price** ($850M Peak Private Valuation) | $24/month (Humane monthly service plan; discontinued post-HP buyout) | 90-day free trial initially bundled with hardware purchase before service shutdown (now requires community servers like OpenPin) | Screenless wearable pin with laser projection display and cloud multimodal AI. Acquired by HP in early 2025. |
| **[Rabbit R1](https://www.rabbit.tech/)** (Rabbit Inc.) | **~$30M Total Funding** Raised (Venture-backed) | $0/month (No recurring subscription; $199 one-time hardware purchase) | Free forever with no token caps for core OS queries, translations, and summaries (user provides cellular SIM/data) | Standalone AI companion device with rotating camera, push-to-talk button, and cloud Large Action Model navigation. |
| **[Brilliant Monocle](https://brilliant.xyz/)** (Brilliant Labs) | **~$6M Total Funding** Raised (Venture-backed) | $0/month introductory tier (Planned future paid tiers for high-volume API use) | Free daily usage cap for multimodal queries/translations via the Noa companion app | Open-source-friendly wearable monocle with an AR micro-OLED display and open developer APIs. |
| **[Limitless Pendant](https://www.limitless.ai/)** (Acquired by Meta) | **~$350M Peak Valuation** (Acquired by Meta in late 2025) | $19/month (Limitless Pro subscription for power users) | 1,200 minutes (20 hours)/month free voice transcription and lifelog search on Free tier | Wearable AI pendant focused on ambient listening, meeting summaries, and conversational lifelog memory. |


## Open-Source GitHub Projects



- **[ESP32 iPhone Agent](https://github.com/onehumanbeing/esp32-iphone-agent)**  

  Let an AI model use a real iPhone with a **$7 ESP32-S3 board**. The board acts as an **AirPlay receiver** (eyes) and **USB HID mouse/keyboard** (hands), while an iPhone app runs the agent loop: decodes the screen stream, sends screenshots to any OpenAI-compatible vision model, and executes taps, swipes, and typing via AssistiveTouch . **No jailbreak, no developer account, no Mac required at runtime**. MIT licensed. Best for demonstrating that autonomous phone control doesn't require expensive hardware—just a microcontroller and a vision model.



- **[OpenPin](https://github.com/MaxMaeder/OpenPin)**  

  Open-source project to **revive bricked Humane AI Pins**. Provides a replacement server system so the device can function again after HP shut down Humane's infrastructure. Requires an **interposer** (small adapter) to link the Pin to the new server; PCBs can be ordered and 3D-printed parts made by users with technical skills . Restores features like assistant queries, photo analysis, and translation. Best for AI Pin owners who want to avoid e-waste and regain partial functionality.



- **[PycoClaw](https://github.com/jetpax/pycoclaw)**  

  A **fully featured MicroPython implementation of OpenClaw** running on a **$5 ESP32-S3**. Not a simple prompt wrapper—it's a proper agent loop with recursive tool calling, context compaction, persistent memory (TF-IDF + vector search on SD card), multi-model routing, background tasks, and async architecture. **Hardware**: any ESP32-S3 with 8MB flash + PSRAM; ESP32-P4 also works . Best for embedded developers who want a complete agent runtime on microcontroller hardware without cloud dependency.



- **[ESP-Claw](https://github.com/Xinyuan-LilyGO/esp-claw)**  

  Espressif's **"Chat Coding" AI agent framework for IoT devices**, inspired by OpenClaw and reimplemented in C. Defines device behavior through conversation and runs the agent loop **locally on ESP32 chips**. Features: IM integration (Telegram, QQ, Feishu, WeChat), structured memory, **MCP communication** (Server and Client), and event-driven architecture with millisecond response. Supports ESP32-S3, ESP32-P4, ESP32-C5, and ESP32-S31 boards . Best for developers building IoT devices that need local decision-making and tool use without cloud latency.



- **[Open Study Buddy](https://github.com/dmccreary/open-study-buddy)**  

  An interactive intelligent textbook for building a **low-cost, fully open personal AI agent device** for students. Pairs a **Raspberry Pi Pico 2 W** with a round 360×360 display, I2S microphone, speaker, and three buttons. Students write every line of MicroPython themselves, learning agent architecture, audio processing, and privacy considerations. The device listens, displays what it heard, speaks answers, and connects to a school-controlled agent backend . Best for education, maker programs, and anyone who wants to understand hardware AI from the ground up.



- **[Foqsee/S1-app](https://github.com/Foqsee/S1-app)**  

  An **open-source alternative to the Rabbit R1** that runs directly on your phone. Repurposes the R1 concept as a mobile app, avoiding the need for dedicated hardware . Best for users who want R1-style functionality without buying a proprietary device.



### Additional Strong Open-Source Options



- **Meta Muse Gadgets SDK** — Meta's Apache 2.0 licensed SDK for connecting ESP32 boards and Linux devices (including Raspberry Pi) to its Muse agent. Supports displays, buttons, sensors, and local HTTP APIs. **Security caveat**: community pairing lacks manufacturer verification and is vulnerable to MITM attacks; SDK tokens are identifiers, not passwords . Best for developers already in the Meta Muse ecosystem.

- **WearGPT** — Runs OpenAI's GPT models on WearOS smartwatches. Best for smartwatch-based AI interaction .

- **Frameworks for building custom systems**: Use **ESP32 iPhone Agent** for phone control automation, **PycoClaw** or **ESP-Claw** for microcontroller agent runtimes, **OpenPin** for hardware revival, and **Open Study Buddy** for educational builds. For Linux-based agents (Raspberry Pi), Meta's Muse SDK provides a bridge to the Muse agent .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- **Hardware AI agents are often cloud-dependent**: Rabbit R1, Limitless, and Ray-Ban Meta require subscriptions and server connectivity. When the vendor shuts down (as with Humane), devices can be bricked—open-source revival projects like OpenPin exist to mitigate this, but require technical effort .

- **Microcontroller agent runtimes** (PycoClaw, ESP-Claw) are constrained by hardware: limited memory, no GPU, and reliance on external APIs for vision models. They demonstrate feasibility, not production-grade performance.

- **Security risks are real**: ESP32-based agents expose USB HID and network interfaces; Meta's own SDK documentation warns of MITM vulnerability in community pairing and recommends treating SDK tokens as identifiers, not secrets . Review security implications before deploying in sensitive environments.



---



**Made for embedded developers, hardware hackers, AI Pin owners, and anyone building physical devices that think for themselves.**  

Let's make hardware AI agents more open, revivable, and accessible.
