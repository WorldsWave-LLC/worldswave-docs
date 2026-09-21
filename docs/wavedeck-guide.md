# How to Use WaveDeck, Powered by WorldsWave: The Complete Live Streaming and Multistreaming Guide

> Learn how to use WaveDeck, WorldsWave's live streaming studio: go live from your browser or OBS and multistream to Twitch, Kick, YouTube and Rumble at once.

*Also published in the [WorldsWave Help Center](https://worldswave.help.center/article/1011-how-to-use-wavedeck-multistreaming-guide).*

---

**WaveDeck is the live streaming studio built into WorldsWave.** You can go live from your browser or from OBS, broadcast to Twitch, Kick, YouTube, Rumble and other platforms at the same time, bring guests on screen, and read chat from every platform in one merged feed. It is included with every WorldsWave account.

This guide covers every WaveDeck feature, from your first stream to advanced multistream setups.

## WaveDeck at a glance

- **Where to find it:** worldswave.com/wavedeck
- **Cost:** included with every WorldsWave account. World+ and Wave Prime raise the limits
- **Two ways to go live:** browser Studio, or any RTMP encoder such as OBS or Streamlabs
- **Multistream destinations:** Twitch, Kick, YouTube, Rumble, X, Trovo, TikTok, Odysee, Facebook, Blaze and Custom RTMP
- **Destinations at once:** 4 on Default, 6 on World+, 8 on Wave Prime
- **Simultaneous streams:** 1 on Default, 2 on World+, 3 on Wave Prime
- **Guests on screen:** up to four people, no software required for them
- **Merged chat:** every platform in one feed, powered by WaveBot
- **Recording:** optional VOD saved automatically when you finish

## What is WaveDeck?

WaveDeck is WorldsWave's built-in live streaming studio and multistreaming tool. It replaces the usual stack of separate apps: you get a broadcast studio, a restream service, a guest room and a multi-platform chat reader in one place, reachable from any browser without installing anything.

WaveDeck is not a separate product you sign up for. If you have a WorldsWave account, you already have WaveDeck. Your streams appear on your WorldsWave profile, and the same broadcast is pushed out to whichever other platforms you connect.

## What are the WaveDeck limits on each plan?

Every WorldsWave account includes WaveDeck. Your plan decides two things: how many platforms you can multistream to at once, and how many streams you can run at the same time. Every other feature, including the Studio, guests, scenes, recording and merged chat, is available on all plans.

- **Default** — 4 multistream destinations, 1 stream slot
- **World+** — 6 multistream destinations, 2 stream slots
- **Wave Prime** — 8 multistream destinations, 3 stream slots

A **multistream destination** is one outbound platform, such as Twitch or Kick. A **stream slot** is one broadcast running at a time, so two slots let you run two separate streams side by side.

**You can also earn a higher plan instead of buying one.** The top five on the all-time points leaderboard get a Pro plan free — ranks 1–3 take Wave Prime, ranks 4–5 take World+ — and streaming is worth 15 points an hour. See [Points and Leaderboards](https://worldswave.help.center/article/1014-points-and-leaderboards).

## How do I start streaming on WaveDeck?

Go to worldswave.com/wavedeck and choose one of three buttons: **Open Studio** to go live from your browser, **Use Stream Key** to go live from OBS or another encoder, or **Schedule Stream** to set one up in advance. Every stream you start gets its own dashboard and its own private link.

Underneath those buttons you will see your **stream slots**, showing how many simultaneous streams you have running out of your plan's allowance: 1 on Default, 2 on World+ and 3 on Wave Prime.

- **Open Studio** — webcam, mic and screen share straight from the browser. Best for interviews, podcasts, reaction streams and anything with guests.
- **Use Stream Key** — connect OBS, Streamlabs or any RTMP encoder. Best for gaming, custom overlays and anything that needs scenes and sources.
- **Schedule Stream** — publishes an upcoming stream so followers know when to show up.

## How do I go live from my browser with WaveDeck Studio?

Click **Open Studio**, turn on your camera, mic or screen share, enter a title and pick a category, then press **Go live**. The Studio opens in preview mode first, so nothing is broadcast until you press that button. You need no software beyond your browser.

### Step 1: Turn on your sources

- **Start camera** — turns on your webcam
- **Mic** — unmutes your microphone
- **Share screen** — shares a window, a browser tab, or your whole screen
- **Stop all** — kills every source at once

The label under the preview reads "Preview only — nothing is broadcast yet" until you go live, so take as long as you need to get set up.

### Step 2: Fill in your stream details

- **Title (required)** — what people see in the feed and in notifications
- **Description** — context, links, or a rundown of what you are doing
- **Category (required)** — Free Speech, Politics, News, Gaming, Technology, Religion, Finance, Music, Sports, Fitness, Entertainment or Travel/IRL
- **Thumbnail (16:9)** — click **Upload image** to set the preview card
- **Record** — switch on to save the broadcast as a VOD

### Step 3: Pick a scene

Scenes control how you and your guests are laid out on screen. You can switch scenes live mid-stream and viewers see the change instantly.

- **Solo** — just you, full frame
- **Two-up** — you and one guest side by side
- **PiP** — one main source with a smaller picture-in-picture inset
- **Screen** — your screen share as the main view
- **3-up** — three people on screen
- **4-up** — four people on screen

### Step 4: Go live

Press **Go live**. Your status changes from Offline to live, the stats bar starts filling in, and your stream appears on WorldsWave. **Start recording** captures the session, and **Start studio session** gets the studio running for guests before you broadcast.

## How do I stream to WaveDeck from OBS?

Click **Use Stream Key** on the WaveDeck dashboard, copy the **Server URL** into OBS under Settings → Stream → Server, then click **SHOW** and **COPY** on the Stream Key and paste it into the Stream Key field. Press Start Streaming in OBS and your feed appears in WaveDeck within a few seconds.

Until your encoder connects, the room page shows "Waiting for your encoder." Once the feed arrives, the **Waiting for encoder** button becomes your Go Live button. The same steps work for Streamlabs, vMix, Prism Live Studio, or any other software that accepts an RTMP server address and key.

### Should I use a static stream key or a per-stream key?

Use a static key if you want to set OBS up once and never touch it again. Use a per-stream key if you would rather each broadcast have its own disposable key. The **Static Key** toggle sits next to your key in the Livestream Setup panel.

- **Static Key ON** — your key never changes. Configure OBS once. This is what most streamers want.
- **Static Key OFF** — a fresh key is generated for every stream. More secure, but you re-paste into OBS each time.
- **Reset** — issues a brand new key if you think yours has leaked

Treat your stream key like a password. Anyone who has it can broadcast to your profile.

### What do the live stats mean?

While you are live, the bar under the player tracks six numbers: **Uptime, Views, Started, FPS, Resolution and Outputs Active**. If viewers report stuttering, check FPS first. If a platform is missing your stream, check Outputs Active against the number of destinations you switched on.

## Which platforms can WaveDeck multistream to?

WaveDeck can push one broadcast to Twitch, YouTube, Kick, Rumble, X (Twitter), Trovo, TikTok, Odysee, Facebook and Blaze, plus any other service through Custom RTMP. Twitch, YouTube and Kick connect automatically with one click. The rest need their stream key pasted in by hand.

- **Twitch** — one-click connect, imports your stream key. Your Twitch login is never stored.
- **YouTube** — one-click connect via Google, imports your key. Your Google login is never stored.
- **Kick** — one-click connect, imports both your key and your ingest URL.
- **Rumble** — click Get Rumble Key. It opens your Rumble static keys in a new tab and pre-fills the form. Rumble has no API, so paste the key yourself.
- **X (Twitter)** — click Get X Key to open X Media Studio Producer. X issues a different server address per source, so copy both the RTMP URL and the key.
- **Trovo** — click Get Trovo Key, then copy the stream URL and key out of Trovo Studio.
- **TikTok** — requires LIVE permission on your TikTok account, and TikTok issues a fresh key each time.
- **Odysee, Facebook and Blaze** — paste the RTMP URL and key.
- **Custom RTMP** — anything else that accepts an RTMP URL and key.

How many you can broadcast to at once depends on your plan: 4 on Default, 6 on World+, 8 on Wave Prime.

## How do I set up multistreaming on WaveDeck?

Go to **Settings → Multi-Stream Setup**, connect or add each destination once, then use the **Multistream Outputs** panel to switch destinations on before you go live. Saved destinations stay on your account, so you only set each platform up a single time.

The Multistream Outputs panel appears on the dashboard, in the Studio and in the encoder room, so you can change destinations wherever you are working.

- Each destination has its own **ON/OFF** toggle
- The **ALL** switch turns every destination on or off at once
- The pencil icon edits a destination
- **Add Output** adds a new one

**Switch your destinations on before you press Go live.** A destination toggled on mid-stream may not pick up a broadcast that is already in progress.

## How do I add a guest to my WaveDeck stream?

In the Studio, click **Invite guest**, copy the link WaveDeck generates under **INVITE LINKS**, and send it to your guest. They open it in any browser, allow camera and mic, and appear in your studio. Then pick a multi-person scene to put them on screen.

Your guest installs nothing. Everyone currently connected is listed under **IN THE STUDIO**. Guests see the same stage preview and studio chat you do, minus the host-only controls.

## How does WaveDeck chat work across platforms?

WaveDeck pulls chat from every platform you are live on into one feed inside the Studio. That merge is powered by **WaveBot**. Add your API details for Kick, YouTube, Twitch, TikTok, Rumble and Trovo under **WaveBot → Chat APIs**, and their messages appear in your WaveDeck chat automatically.

Until WaveBot is connected, the chat panel shows "No external chat connected" and you will only see WorldsWave messages.

- **Overlay: On** — shows chat as an overlay on your broadcast so viewers on other platforms can follow along
- **Test** — fires a test message so you can check your layout before going live
- **Send** — lets you talk to your viewers as the host

WaveBot also runs as a browser dock inside OBS and can connect to your local OBS WebSocket to control OBS directly.

### Where is my WaveBot API key?

Open **Settings → Static Stream Key** and look under the WAVEBOT heading. Click **Copy** and paste the key into WaveBot's API key field to unlock backend features and sync your settings across devices. **Generate New Key** issues a fresh one and immediately stops the old one working.

If you regenerate, update WaveBot straight afterwards or your merged chat will stop. Keep this key private.

### How do I put my WaveDeck chat in OBS or Social Stream Ninja?

Go to **Settings → Static Links** and copy the **Live Chat (for Social Stream Ninja / OBS)** link. Add it once as an OBS browser source, or paste it into Social Stream Ninja. It follows you to whatever stream you go live on next, so you never swap in a new chat link again.

Between streams the link shows a waiting screen and picks up your next stream on its own. Do not copy the chat URL from an individual stream page, because that one expires when the stream ends.

## How do I add moderators to my streams?

Go to **Settings → Moderators** and search for a user by name or @username. Moderators added here are permanent: they are automatically a moderator on **every** stream you start. They can mute viewers in live chat, block viewers, and approve join requests.

## What are WaveDeck static links?

Static links are permanent addresses that point at you rather than at one particular stream. You share them once and they never need updating. Find them under **Settings → Static Links**.

- **Live Link** (worldswave.com/YourName/live) — your forever-link. Sends people to your stream when you are live and to your newest replay when you are not.
- **Live Chat** — your chat as a browser source for OBS or Social Stream Ninja
- **All Streams** (worldswave.com/YourName/livestreams) — every stream and replay you have, newest first
- **Profile** (worldswave.com/YourName) — your WorldsWave profile page

## How do I schedule a stream on WaveDeck?

Use **Schedule Stream** on the WaveDeck dashboard for a one-off broadcast, or **Settings → Weekly Schedule** for a recurring show. The weekly schedule automatically creates and posts an upcoming stream 24 hours before each window opens.

1. Toggle the feature **ON** at the top right
2. Enable each day you stream
3. Set a **From** and **to** window for that day

All times are shown in your own local timezone.

## Where do I find my WaveDeck recordings?

Go to **Settings → My VODs** to see recordings of your finished live streams. A recording only appears there if **Record** was switched on before you went live. Your VODs are also reachable through your All Streams static link.

## How do I see how my streams are performing?

Go to **Settings → Stream Stats**. You can view **7D**, **30D** or **90D**, switch between a graph and a **Table**, download the chart with **Save graph**, or export the raw numbers with **CSV**.

Tracked measurements include **Total Streams**, **Stream Views** and **Avg Stream Views**. Click a measurement tile to add it to the chart and click again to remove it.

Your wider account numbers — Total Views, Likes, Followers, Shares, Comments and Messages/DMs — live on **Dashboard → Overview**.

## What stream options can I turn on?

- **Record Broadcast** — saves the stream as a VOD when you finish
- **Allow Viewers To Comment** — turns live chat on or off
- **Allow Tips** — lets viewers tip you during the stream
- **Allow Gifts** — lets viewers send virtual gifts

## How do stream templates work?

Stream templates save your title, description, category, thumbnail and options so you do not rebuild them every broadcast. Set everything the way you want it, click **Save as new…** under STREAM TEMPLATE and name it. Next time, pick it from the dropdown and click **Load**.

## WaveDeck troubleshooting

### Why does WaveDeck say "Waiting for your encoder"?

Your encoder has not connected yet. Check that the Server URL and Stream Key in OBS exactly match the Livestream Setup panel, and that you actually pressed Start Streaming. If you recently reset your key, OBS is still sending the old one.

### Why does it say my stream key could not be read?

Reload the page. If the message persists, the live service is not reachable from the site right now. Report it with the **Report A Bug** button.

### Why is one platform not receiving my stream?

Open the Multistream Outputs panel and confirm that destination's toggle is ON and the ALL switch is not off. Check Outputs Active in the stats bar. Platforms that rotate keys, TikTok especially, often need a fresh key before each stream.

### Why is chat from other platforms not showing?

WaveDeck shows "No external chat connected" until WaveBot is set up. Add your platform APIs under WaveBot → Chat APIs. If merged chat stopped working, check whether you regenerated your WaveBot API key without updating WaveBot.

### Why is my chat overlay missing in OBS?

Use the Live Chat link from Static Links as your browser source rather than a URL copied from an individual stream page.

### Why can't my guest get on screen?

Check that they allowed camera and microphone permissions, that they appear under IN THE STUDIO, and that you have selected a multi-person scene. Solo shows only the host.

### Why is there no recording after my stream?

Recordings only save when **Record** was switched on before you went live. It cannot be enabled retroactively.

## Frequently asked questions

**Is WaveDeck free?**
Yes. WaveDeck is included with every WorldsWave account at no extra cost. The World+ and Wave Prime plans raise two limits — multistream destinations and simultaneous streams — but the studio itself, guests, scenes, recording and merged chat are on every plan.

**How many platforms can I multistream to at once?**
Four on the Default plan, six on World+ and eight on Wave Prime.

**Can I run more than one stream at a time?**
Default gives you one stream slot, World+ two and Wave Prime three.

**Do I need OBS to use WaveDeck?**
No. WaveDeck Studio runs entirely in your browser. OBS is only needed for custom scenes, overlays or capture cards.

**Can I stream to Twitch, Kick, YouTube and Rumble at the same time?**
Yes. Add each platform under Settings → Multi-Stream Setup, then switch its toggle on before you go live.

**Does WaveDeck work on mobile?**
WaveDeck Studio runs in a mobile browser, and any phone streaming app that supports RTMP can send to your WaveDeck stream key.

**How many guests can I have on a WaveDeck stream?**
Up to four people can be on screen at once using the 4-up scene.

**Does my stream key change every time?**
Only if you want it to. With Static Key switched on, your key stays the same forever.

**Can I save a recording of my stream?**
Yes. Switch **Record** on before you go live, and it appears under Settings → My VODs.

**Can moderators from one stream carry over to the next?**
Yes. Moderators added under Settings → Moderators are permanent.

## WaveDeck quick reference

- **Stream from my browser** — Open Studio
- **Stream from OBS** — Use Stream Key
- **Add Twitch, Kick, YouTube or Rumble** — Settings → Multi-Stream Setup
- **Get my permanent OBS key** — Settings → Static Stream Key
- **Get a link for my bio** — Settings → Static Links → Live Link
- **Put chat in OBS** — Settings → Static Links → Live Chat
- **Add a permanent moderator** — Settings → Moderators
- **Find my replays** — Settings → My VODs
- **Check my performance** — Settings → Stream Stats
- **Set my streaming hours** — Settings → Weekly Schedule
- **Merge chat from every platform** — WaveBot → Chat APIs
- **Bring someone on screen** — Studio → Invite guest

## Still need help?

Use the **Report A Bug** button in the top right of any WaveDeck page, or contact the WorldsWave team through this help center.
