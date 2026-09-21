# How to Set Up WaveBot: One Chat Feed From Every Platform You Stream To

> Set up WaveBot to pull chat from Twitch, Kick, YouTube, TikTok, Rumble and more into one feed, put it on your stream as an OBS overlay, and read it aloud.

*Also published in the [WorldsWave Help Center](https://worldswave.help.center/article/1012-how-to-set-up-wavebot-chat).*

---

**WaveBot is the chat and overlay companion to WaveDeck.** WaveDeck sends your video out to every platform; WaveBot brings every platform's chat back in. Connect each service once and all of their messages land in a single feed you can put on screen, read aloud, and moderate from one place.

This guide covers connecting WaveBot to your account, adding each chat platform, and putting the merged feed on your stream.

## WaveBot at a glance

- **Where to find it:** worldswave.com/apps/wavebot/
- **Cost:** free for everyone with a WorldsWave account. Wavium credits cover the AI features
- **Runs:** in any browser, or as a custom browser dock inside OBS
- **Chat sources:** 11 — WorldsWave, Twitch, YouTube, Kick, Facebook, TikTok, Rumble, X, Trovo, Blaze (Instagram is listed but not possible)
- **No key needed for:** WorldsWave, TikTok, Blaze
- **One-click login for:** YouTube, Facebook
- **Output:** a transparent browser-source URL for OBS, styled in the dock
- **Also does:** text-to-speech, an AI co-host, alerts, goals, mini games and chat commands

## What is WaveBot?

WaveBot is WorldsWave's chat engine, overlay builder and stream control surface. It reads chat from every platform you broadcast to, merges it into one feed tagged with the site each message came from, and gives you a browser-source URL to put that feed on screen.

**WaveBot does not handle restreaming.** Sending your video to Twitch, Kick, YouTube and the rest is WaveDeck's job, set up under Settings → Multi-Stream Setup on WorldsWave. WaveBot handles the chat coming back the other way. The two are designed to be used together.

## How do I connect WaveBot to my WorldsWave account?

Open **worldswave.com/apps/wavebot/**. If you are already signed in to WorldsWave in the same browser, WaveBot picks up your key automatically and you are done. If it shows a **Connect WaveBot** screen, copy your WaveBot API key from **Dashboard → Static Stream Key** on WorldsWave and paste it in.

Your WaveBot API key sits under the **WAVEBOT** heading at the bottom of the Static Stream Key page, with a Copy button. It looks like `ww_live_…`.

Once connected, the Dashboard shows **World's Wave API connected** and **All features unlocked**, and a **Getting Started** checklist tracks what is left:

1. **Configure API keys** — your WorldsWave credentials
2. **Alerts configured** — every alert event has defaults, so this is done out of the box
3. **Connect OBS** — optional, only needed if you want WaveBot to drive scenes
4. **Add a stream destination** — WorldsWave or a restream target

### Should I sync my keys to my account?

In **Settings → Account & API Access** there is a **Sync my keys to my World's Wave account** toggle. Off, your platform keys stay in that one browser. On, they follow you to any other device you open WaveBot on. Keys are stored encrypted either way.

Turn it on if you stream from more than one machine, or if you run WaveBot inside OBS as well as in a normal browser tab. Inside OBS the dock cannot see your WorldsWave login, so the key has to be pasted once — after that it is remembered.

## Which chat platforms can WaveBot pull from?

WaveBot supports eleven chat sources. WorldsWave is connected by default, TikTok and Blaze need only your channel name, YouTube and Facebook use a one-click login, and the rest need a key pasted in by hand. Instagram is listed but cannot work.

| Platform | What it needs | Notes |
|---|---|---|
| **WorldsWave** | Nothing | Already connected. No key. |
| **Twitch** | Chat OAuth token + channel | Token from the Twitch dev console, or twitchapps.com/tmi |
| **YouTube** | Connect with Google + channel ID or handle | The Google login gives reliable live-chat access |
| **Kick** | Channel name | An API token is only needed for *posting*, not reading |
| **Facebook** | Connect with Facebook | Finds your active Live video on your profile or a Page you manage |
| **TikTok** | Your @username | No developer key or app. You must be live when it connects |
| **Rumble** | Stream API key + channel | Via Rumble's Live Stream API URL and key |
| **X (Twitter)** | Handle, bearer optional | Live-chat support on X is limited |
| **Trovo** | Client ID + channel | |
| **Blaze** | Channel name | No key. Must be live when it connects. Emotes included |
| **Instagram** | — | **Not possible.** Meta does not expose IG Live comments. Use Facebook for FB Live instead |

Each row has a **Test** button so you can confirm a source works before you go live, and a status badge reading **CONNECTED** or **NOT SET UP**.

## How do I connect each chat platform?

Go to **Stream Dashboard → Chat APIs**. Every platform is a row on that page. Fill in what it asks for, press **Test**, and look for the status to flip to CONNECTED.

### The ones that need nothing

**WorldsWave** is connected the moment your account is linked. **TikTok** needs only your @username typed in, and **Blaze** only your channel name — both read the public live chat the same way Social Stream Ninja does. The catch with both: you have to already be live when WaveBot connects, so start your stream first, then hit Test.

### The ones with a login button

**YouTube** and **Facebook** have a **Connect (login)** button. Click it, authorise with Google or Facebook, and WaveBot handles the rest. For YouTube, also fill in your channel handle or ID. For Facebook, WaveBot finds whichever Live video is currently running on your profile or a Page you manage and pulls its comments automatically.

### The ones that need a key

**Twitch, Kick, Rumble, X and Trovo** each need a value pasted in. Every one of those rows has a **Get key** button that opens the right page on that platform, so you are not hunting for it.

- **Twitch** — a chat OAuth token plus your channel name
- **Kick** — just your channel name for reading chat; the optional API token only matters if you want WaveBot to post messages
- **Rumble** — the stream API key and channel from Rumble's Live Stream API
- **X** — your handle, with an API bearer optional
- **Trovo** — a client ID and your channel

## How do I put the merged chat on my stream?

Open **Chat Overlay** in the sidebar and copy the **generated overlay URL**. Add it to OBS as a **Browser Source at 1920×1080 with a transparent background**. Everything you change in the dock — font, opacity, filters — updates that source live.

The panel has a **Live Preview** with a **Send test message** button, so you can style the overlay before anyone is watching.

### Styling options

- **Background opacity** — defaults to 75%
- **Font size** — defaults to 16px
- **Message fade-out** — defaults to 45 seconds
- **Font** — Inter, Roboto, Poppins, JetBrains Mono or Bebas Neue
- **Username accent** — a colour for usernames
- **Custom CSS** — injected straight into the browser source

### Filters

- **Colour every username with the accent** — off gives each chatter their own colour
- **Hide bot commands** — hides messages starting with `!`
- **Hide bot accounts** — Nightbot, StreamElements and similar
- **Show badges** — puts the platform logo on each message, so you can see at a glance who came from where
- **Animate new messages** — slide and fade in

If the overlay stops updating, press **Reload Source** in the dock rather than removing and re-adding it in OBS.

## How do I add WaveBot as a dock inside OBS?

In OBS, go to **Docks → Custom Browser Docks**, give it a name, paste **https://worldswave.com/apps/wavebot/** as the URL, and click Apply. WaveBot then lives inside OBS as a panel you can drag and dock anywhere in your layout.

The dock cannot see your WorldsWave browser session, so the first time it opens you will need to paste your WaveBot API key once. Turning on **Sync my keys to my World's Wave account** beforehand saves you repeating that on other machines.

Two dock display options sit in **Settings → Dock**: **Collapse navigation** shows an icon rail instead of full labels, and **Keep stats sidebar open** pins the live stats panel on narrow docks. Both are worth turning on if your dock is a narrow column.

## How do I let WaveBot control OBS?

Enable **obs-websocket** in OBS under **Tools → WebSocket Server Settings**, then in WaveBot go to **Stream Dashboard → Control**, enter the address (`ws://127.0.0.1:4455` by default) and password, and press **Test**. This is optional.

**Without a control surface WaveBot still runs overlays, alerts, chat and TTS.** It just cannot drive OBS itself. Connecting obs-websocket unlocks three things that are otherwise locked:

- Switching scenes from the dock
- Controlling the audio mixer
- Starting and stopping recording

WaveBot supports **obs-websocket 5.x and 4.x**, and **vMix Web Controller** as an alternative. The connection is local — the password stays on your PC and nothing about your scene collection leaves the machine. There is a **Reconnect to OBS on launch** toggle so it connects itself every time the dock opens.

## Can WaveBot read chat out loud?

Yes. **ElevenLabs TTS** in the sidebar handles text-to-speech, and **Windows SAPI is built in**, so you have working voices with no account and no API key. The panel has four tabs: Voices, Providers, Routing & Rules, and a queue.

- **Voice Library** — lists every voice across your providers, with a **Use** button. Windows SAPI ships with David and Zira
- **Delivery** — rate and pitch. The panel only shows the controls the chosen provider actually supports
- **Queue Manager** — shows pending lines, with **Skip Current** and **Clear Queue**
- **Routing & Rules** — decides what gets spoken

Bring your own ElevenLabs account if you want better voices than the built-in ones. There is also a **TTS Queue → Clear** button in the right-hand rail for when the queue runs away from you mid-stream.

## Can WaveBot reply to chat on its own?

Yes — the **AI Chat Engine** gives WaveBot a co-host personality that answers viewers in your live chat as WaveBot. It is off behind a master switch, and every reply costs **Wavium credits**.

Pick a ready-made persona — **Hype Co-Host**, **Chill Surfer** or **Game Analyst** — or write your own system prompt of up to 2,000 characters. A **Sample Exchange** box lets you send a line as a viewer and see how it answers before you let it loose.

**Engine settings:**

- **Auto-reply in chat** — answers without being tagged
- **Reply when mentioned** — always answers @WaveBot
- **Model** — WorldsWave Fast, WorldsWave Pro, or a local model via Ollama

**Reply tuning:** reply frequency as a percentage of messages, a cooldown between replies, a maximum reply length, and a creativity slider.

**Safety:** a safety threshold, a switch to block links in AI replies, a hard block on financial and medical advice, and a free-text list of blocked topics. Moderators can override with `!ai`.

Start with a low reply frequency and a hard cooldown. An AI co-host answering a third of all messages reads as noise very quickly.

## What else is in WaveBot?

The chat pipeline is one part of the dock. The rest, one line each:

- **Mod Dashboard** — watch chat and moderate; timeout, ban and set chat rules
- **Clips** — grab highlight clips and choose where they save or post
- **Alerts** — design the pop-ups for follows, subs, tips and raids
- **Goals** — follower, sub and tip goal bars on stream
- **Emotes** — emote wall explosions and your custom chat emotes
- **Scroller** — a scrolling ticker of messages along your overlay
- **Looper** — loop a background video or GIF behind your scene
- **Mini Games** — trivia, giveaways, polls and a viewer queue in chat
- **Chat Commands** — create `!commands` with permissions and cooldowns
- **Discord** — post go-live announcements and sync roles
- **AI Media Studio** — generate alert art, video and music, paid in Wavium credits

The **Stream Dashboard** also carries a program preview, **Stream Health** (connection, viewer trend, CPU, dropped frames, bitrate), an **Audio Mixer** that connects to Elgato Wave Link, and **Quick Actions** for muting the mic, pausing alerts, refreshing overlays and running an ad break.

## WaveBot troubleshooting

### Why does WaveBot say my API key was not accepted?

The dock's stored key no longer matches your account. Copy the current key from **Dashboard → Static Stream Key** on WorldsWave and paste it into the Connect screen. This happens if you clicked **Generate New Key** on WorldsWave without updating the dock, and it is the same fix either way.

### Why is chat from one platform not coming through?

Open **Chat APIs** and press **Test** on that row. TikTok and Blaze only connect while you are actually live, so start the stream first. Twitch tokens expire and need re-pasting. For YouTube and Facebook, the login can lapse — click **Connect (login)** again.

### Why can't I get Instagram chat?

You can't, and it is not a WaveBot problem. Meta does not expose Instagram Live comments through any public API. If you are live on Facebook, connect Facebook instead.

### Why is my chat overlay blank in OBS?

Check the browser source is using the **generated overlay URL** from the Chat Overlay panel, set to 1920×1080 with a transparent background. If the URL is right but nothing appears, press **Reload Source** in the dock. Remember the overlay only shows messages that arrive while you are live.

### Why are scene switching and recording greyed out?

No control surface is connected. WaveBot defaults to **Manual**, which is read-only. Connect obs-websocket under **Stream Dashboard → Control** to unlock scene switching, the audio mixer and recording.

### Why is WaveBot not replying in chat?

Check the **AI engine enabled** master switch, then **Auto-reply in chat**. If both are on and it is still quiet, you may be out of **Wavium credits** — each reply costs credits, and the balance is in the right-hand rail.

### How do I stop everything at once?

**Panic Stop** on the Dashboard. **Restart Bot** sits next to it for a softer reset. The Dashboard's **Recent Activity** log records every WaveBot event in the session and has a **Copy log** button, which is the first thing to grab if you need to report a bug.

## Frequently asked questions

**Is WaveBot free?**
Yes. **WaveBot is free for everyone with a WorldsWave account** — every plan, no upgrade needed. That includes all eleven chat sources, the chat overlay, the OBS dock, obs-websocket control and text-to-speech. **Wavium credits** are what WaveBot's AI features run on: the AI co-host's replies and AI Media Studio generations. Credits are separate from **Wavium**, the WorldsWave currency used for superchats, money gifts and buying things on the site.

**Can WaveBot help me get a free plan?**
Not directly — WaveBot itself is already free on every plan. But the streaming it supports does earn points, at 15 points an hour, and the **top five on the all-time points leaderboard get a Pro plan for free**: ranks 1–3 take Wave Prime, ranks 4–5 take World+. See [Points and Leaderboards](https://worldswave.help.center/article/1014-points-and-leaderboards).

**Do I need WaveDeck to use WaveBot?**
No, but they are built for each other. WaveDeck sends your video out to multiple platforms; WaveBot brings those platforms' chat back into one feed. Using one without the other works, but you lose half the point.

**Does WaveBot need to be installed?**
No. WaveBot runs in the browser. Inside OBS you add it as a custom browser dock pointing at the same URL — still nothing to install.

**Can WaveBot post messages back to other platforms, or only read them?**
Reading is the default everywhere. Posting needs write access on that platform — on Kick, for example, the optional API token is what enables posting rather than just reading.

**Do I have to be live for chat to connect?**
For **TikTok** and **Blaze**, yes — both read the live chat directly and need the stream running when they connect. The others can be connected in advance.

**Where is my WaveBot API key?**
On WorldsWave, under **Dashboard → Static Stream Key**, at the bottom under the WAVEBOT heading. Keep it private — anyone with it can drive your dock.

**What happens if I regenerate my WaveBot API key?**
The old key stops working immediately, so re-paste the new one into the dock straight afterwards or your chat and overlays will stop syncing.

**Can I use WaveBot on more than one computer?**
Yes. Turn on **Sync my keys to my World's Wave account** in Settings and your platform keys follow you to any device you open WaveBot on.

**Does WaveBot work with vMix?**
Yes. Alongside obs-websocket, WaveBot supports the vMix Web Controller as a control surface.

**Can my moderators turn off the AI co-host?**
Yes. Moderators can override the AI engine in chat with `!ai`.

## WaveBot quick reference

- **Connect WaveBot to my account** — paste the key from Dashboard → Static Stream Key
- **Add a chat platform** — Stream Dashboard → Chat APIs
- **Put chat on stream** — Chat Overlay → copy the overlay URL into an OBS browser source
- **Run WaveBot inside OBS** — Docks → Custom Browser Docks → worldswave.com/apps/wavebot/
- **Let WaveBot drive OBS** — Stream Dashboard → Control → OBS WebSocket
- **Read chat aloud** — ElevenLabs TTS
- **Turn on the AI co-host** — AI Chat Engine
- **Moderate chat** — Mod Dashboard
- **Make !commands** — Chat Commands
- **Stop everything** — Panic Stop on the Dashboard

## Still need help?

Use the **Report A Bug** button on any WorldsWave page, or contact the WorldsWave team through this help center. If you are reporting a WaveBot problem, grab the **Copy log** button on the Dashboard's Recent Activity panel first — it saves a lot of back and forth.
