# ChizChat — User Guide

**Version 2.4.38** · Android · Windows · Linux

---

## Contents

1. [What ChizChat is](#1-what-chizchat-is)
2. [Getting started](#2-getting-started)
3. [Finding your way around](#3-finding-your-way-around)
4. [Your profile](#4-your-profile)
5. [Friends — chatting over the internet](#5-friends--chatting-over-the-internet)
6. [Sending messages](#6-sending-messages)
7. [Read receipts — what the ticks mean](#7-read-receipts--what-the-ticks-mean)
8. [Photos, files and folders](#8-photos-files-and-folders)
9. [Voice and video calls](#9-voice-and-video-calls)
10. [Screen sharing](#10-screen-sharing)
11. [Nearby — offline sharing over local Wi-Fi](#11-nearby--offline-sharing-over-local-wi-fi)
12. [Rooms — ephemeral group chat](#12-rooms--ephemeral-group-chat)
13. [Workspace — workmates and teams on the office LAN](#13-workspace--workmates-and-teams-on-the-office-lan)
14. [When someone is offline](#14-when-someone-is-offline)
15. [Notifications](#15-notifications)
16. [Permissions ChizChat asks for](#16-permissions-chizchat-asks-for)
17. [Troubleshooting](#17-troubleshooting)
18. [Privacy and how your data travels](#18-privacy-and-how-your-data-travels)
19. [Known limitations](#19-known-limitations)

---

## 1. What ChizChat is

ChizChat is a **peer-to-peer messenger**. Your messages and files travel **directly from your
device to the other person's device**. There is no ChizChat server in the middle holding your
conversations.

That one fact explains almost everything about how the app behaves:

- **Nothing is stored on a server.** Your chat history lives on your device and theirs.
- **A message to someone who is offline stays on your phone** until they are reachable again.
  It is not "in the cloud waiting for them" — see [When someone is offline](#14-when-someone-is-offline).
- **Deleting the app deletes your history.** There is no account to log back into.

ChizChat gives you four ways to reach people, and you can use all of them at once:

| Mode | Needs internet? | Best for |
|---|---|---|
| **Friends** | Yes | Everyday chat with people anywhere |
| **Nearby** | **No** — one shared Wi-Fi network | Fast, large file transfers between devices in the same place |
| **Rooms** | Yes | Quick, throwaway group chat — anyone with the room name can join |
| **Workspace** | **No** — office LAN | Colleagues and teams on the same office network |

---

## 2. Getting started

### Installing

- **Android** — install from Google Play, or sideload the APK if you were given one.
- **Windows** — run the installer (`.exe`).
- **Linux** — run the `AppImage`, or install the `.deb` package.

### First run

On first launch you'll see the **setup screen**:

1. Type a **display name**. This is what other people see — it is not a username, there is no
   password, and nothing is registered anywhere.
2. Tap **INITIALIZE**.

That's it. ChizChat generates a **Peer ID** for your device (something like
`chizchat-a3f19c02d8b41e77`). This ID is your address on the network. You can see and copy it any
time from the sidebar, just under your name.

> **Keep in mind:** your identity lives on this device. Installing ChizChat on a second device
> creates a *different* identity — your friends there will need to add you again.

---

## 3. Finding your way around

### PERSONAL and WORK

At the very top of the sidebar there are two pills: **PERSONAL** and **WORK**. These are two
separate spaces with their own contacts, their own profile, and their own chats. Tap to switch.

### The PERSONAL tabs

Below your profile there are three tabs:

- **FRIENDS** — people you chat with over the internet.
- **NEARBY** — people you've paired with over local Wi-Fi, plus the radar.
- **ROOMS** — join or create an ephemeral group room.

### The WORK tabs

- **WORKMATES** — colleagues added by their local IP address.
- **TEAMS** — groups of workmates you've organised.

### The connection bar

A thin strip along the bottom of the app always tells you your current connection state:

| Bar | Meaning |
|---|---|
| **● Connected** (green) | You're online over Wi-Fi or a wired network |
| **● Connected via Mobile Data** (blue) | You're online, but on cellular |
| **◐ Connecting… / Reconnecting…** (yellow) | Establishing the connection |
| **○ Failed to connect** (red) | No connection right now |

### On a phone

The sidebar slides away on small screens. Tap the **☰ menu** icon in the top bar to bring it
back, and the **‹ back arrow** inside a chat to return to the list.

---

## 4. Your profile

Tap your avatar or the **⚙ gear icon** at the top of the sidebar to open **Edit Profile**.

- **Display Name** — change it any time; your contacts see the new name.
- **Avatar** — three ways to set one:
  - **PRESETS** — pick from the built-in set.
  - **CUSTOMIZE** — choose a background colour and a face style to generate your own.
  - **UPLOAD** — use any JPG, PNG or WebP from your device. It is automatically shrunk to a small
    thumbnail before being shared, so it costs almost nothing to send.

Tap **Save Profile** when you're done.

Your **Work profile** (name and avatar) is separate — edit it from the gear icon inside the WORK
space. Use it for something like `John Doe (Frontend)` while your personal name stays casual.

### Copying your Peer ID

Under your name in the sidebar is your Peer ID, shortened. Tap it to copy the full ID to your
clipboard.

---

## 5. Friends — chatting over the internet

### Adding a friend

Tap **Add Friend** in the FRIENDS tab. You have two options, and one of you does each:

**If you're sharing your code:**
1. Tap **Generate My Code**.
2. A six-digit code appears (e.g. `482-913`). Read it out, message it, whatever is easiest.
3. Wait — the screen says *"Waiting for friend to connect…"*.

**If you're entering their code:**
1. Type their code into the box.
2. Tap the **→** arrow.

Once it connects, you both appear in each other's friends list. Codes are one-time and
short-lived; generate a fresh one for each person.

> **If it hangs for more than ~25 seconds,** a *"Still not connecting?"* note appears with a
> **Reconnect and try again** button. This renews your device's connection identity and restarts
> the app in place. Nothing is lost — you just start the code over.

### Reading the friends list

Each friend has a small dot on their avatar:

| Dot | Meaning |
|---|---|
| **Solid green** (glowing) | Connected right now — your message sends *instantly* |
| **Hollow green ring** | Online, but no direct channel yet — the first message spends a few seconds connecting |
| **Grey** | Offline — see [When someone is offline](#14-when-someone-is-offline) |

Under the name you'll see `Online`, or `Last seen 12m ago`.

A **red badge** on the right shows unread messages.

### Other things you can do here

- **Search** — the box at the top filters by name or Peer ID.
- **Refresh** (⟳ next to *Add Friend*) — re-checks who's online.
- **Delete a contact** — the 🗑 icon on their row. This also **permanently deletes your chat
  history with them**, and asks you to confirm first.

---

## 6. Sending messages

Open a chat by tapping a friend. The message box is at the bottom.

### Text

- Type and press **Enter** (or the **➤ send** button) to send.
- **Shift+Enter** inserts a new line. The box grows up to five lines.

### Formatting

ChizChat understands **Markdown**. If your message contains headings, lists, quotes, tables,
links, or fenced code blocks, it is rendered as formatted text rather than raw characters.

It also **auto-detects pasted code**. Paste a function, a SQL query, some JSON or an HTML
fragment, and ChizChat wraps it in a code block for you.

**Pasting from a web page or a document** converts the formatting (bold, lists, tables, links)
into Markdown automatically, rather than dumping plain text.

### The ChizChat thumb 👍

The button next to the send button sends a **thumbs up** — ChizChat's own chunky neon hand, drawn
for the app rather than borrowed from your device's font. Send it on its own and it appears
sticker-sized in the conversation.

### Voice messages

When the message box is empty, the send button becomes a **🎤 microphone**.

1. Tap **🎤** to start recording. A red timer appears.
2. Tap **➤** to send, or the **🗑 bin** to throw the recording away.

Received voice messages play inline with a scrubber.

### What you can do with a message

**Long-press** (or right-click on desktop) any message to open its menu:

- **React** — six custom ChizChat emoji along the top: ❤️ love, 😂 laugh, 😮 wow, 😢 sad, 😠 angry,
  👍 like. Tap one to react; it appears on the message for both of you.
- **Copy Message** — copies the text to your clipboard.
- **Select Text** — opens the message in a view where you can select and copy just part of it.
- **Reply** — quotes the message above your reply box. Tap **✕** to cancel.
- **Forward** — pick a friend to forward it to, with a search box to find them.
- **Delete Message** — removes it from your device.

### Clearing a conversation

The **🗑 icon in the chat header** clears the whole conversation. You'll be asked to confirm.

### Scrolling back

Chats load the most recent messages first. **Scroll up** and older messages load automatically —
you'll see *"Loading previous chats…"*, and *"Beginning of chat history"* when you reach the top.

---

## 7. Read receipts — what the ticks mean

Under each message you send there is a small status icon:

| Icon | State | Meaning |
|---|---|---|
| 🕐 Clock (yellow) | **Pending** | Still on your device — the other person isn't reachable |
| ✓ Single tick (grey) | **Sent** | It left your device |
| ✓✓ Double tick (green) | **Delivered** | It reached their device and their device confirmed it |
| ✓✓ Double tick (blue) | **Read** | They actually opened the chat and saw it |
| ✕ (red) | **Failed / rejected** | It didn't go through, or a file offer was declined |

The blue tick means what it says: it only turns blue when the *other person* opens the
conversation. Opening your own chat never marks your own messages read.

Receipts work on **every** transport:

| | Delivered | Read |
|---|---|---|
| Friends (internet) | ✔ | ✔ |
| Nearby (local Wi-Fi) | ✔ | ✔ |
| Workspace workmate | ✔ | ✔ |
| Rooms and Workspace teams | — | **"Seen by N"** |

### "Seen by N" in groups

Group rooms and teams don't have a fixed membership — people come and go — so instead of a tick,
your own messages show **"Seen by 3"**. **Tap it** to expand the list of names, in the order they
read it. The count only ever goes up; someone leaving can't un-see what they already saw.

> **Talking to someone on an older version?** They simply see no ticks. Nothing breaks and no
> stray messages appear in their chat.

---

## 8. Photos, files and folders

### Sending

Two buttons sit to the left of the message box:

- **🖼 Image** — opens your photo/video picker.
- **📎 Paperclip** — opens the general file picker. You can select **multiple files**.

On desktop you can also **drag files onto the chat window** — a *"Drop files here"* overlay
appears.

Multiple files sent together arrive as a **folder card** showing the item count and total size,
with up to four thumbnails.

### Receiving

A file is **never** downloaded without your say-so. When someone sends you something you'll see
the offer with **Accept All** and **Decline** buttons.

While a transfer runs you get:

- A **live progress bar** with percentage, transfer speed and total size.
- **⏸ PAUSE** / **▶ RESUME** — suspend and continue a transfer.
- **✖ CANCEL** — abandon it.

> Very large transfers over local Wi-Fi use a faster "pull" method that can't be paused — the
> pause button simply isn't offered for those.

The sender sees *"Waiting for recipient to accept…"*, or *"Recipient declined the file transfer."*

### Where received files go

On Android and desktop, accepted files are saved into a **ChizChat** folder inside your
**Documents** directory. If a file with the same name already exists, a numbered copy is made
rather than overwriting anything.

### Viewing what you've received

- **Tap an image** to open the full-page viewer. From there you can also **forward** it.
- **Tap a folder card** to open the gallery, where each file has its own **⬇ download** button.

---

## 9. Voice and video calls

Tap the **📞 phone icon** in a chat header to call.

**On the receiving end** the phone rings with ChizChat's ringtone and shows **Accept** /
**Decline**.

During a call you have:

- **📹 Camera** — turn your camera on or off. Turning it on makes it a **video call**; the screen
  header changes from *VOICE CALL* to *VIDEO CALL*. Your own preview appears in the corner.
- **🎙 Mute / Unmute** your microphone.
- **🔊 Speaker / Earpiece** — switch the audio route.
- **📞 End Call** (red).
- **Minimize to Chat** — shrink the call so you can keep typing while it continues.

A **call timer** runs at the top. If the connection drops mid-call it shows *RECONNECTING…*
rather than hanging up on you.

On Android the call keeps running when you leave the app or the screen turns off — an ongoing
**"ChizChat Call — Call in progress…"** notification is shown for the whole call, and disappears
the moment it ends.

> **Note:** calls need a working path between the two devices. Both being on the same local
> network is the most reliable case — see [Known limitations](#19-known-limitations).

---

## 10. Screen sharing

On **desktop**, a **🖥 Share Screen** button appears in the chat header (and in a room).

1. Tap it. The other person gets a **Screen Share Request** with Accept / Decline.
2. While you wait you'll see *"Waiting for … to accept screen share…"*.
3. Once accepted, they see your screen live. A banner shows sharing is active so you can't forget
   it's on.

Screen sharing is **view-only** — the other person can see, not touch.

---

## 11. Nearby — offline sharing over local Wi-Fi

**Nearby is for moving large files fast between devices in the same place, with no internet at
all.**

### The one rule

**Both devices must be on the same Wi-Fi network.** That's the entire requirement. No internet is
needed on that network — it just has to connect the two devices.

The radar screen states this up front and shows your **network name** and **IP address** so you
can check against the other device.

### Opening the radar

Go to the **NEARBY** tab and tap **Nearby radar**.

You'll see a sweeping radar with yourself in the middle and every discovered device around you.
Below, a row of chips lists everyone by name, and a counter says *"3 devices nearby"* — or
*"Looking for people nearby…"*.

Radar controls (top right):

- **👁 Eye** — toggle **discoverable**. When hidden, others can't find you on the radar; friends
  you've already paired with can still reach you.
- **⟳ Refresh** — scan again.
- **▣ QR** — add someone by code instead (see below).
- **✕** — close the radar. Your existing links stay up.

### The network panel

At the top of the radar, a panel tells you what network you're on:

- **Pink** — you're on a network, name and IP shown.
- **Amber** — you're not on a network yet.

Tap it to expand a short explanation. On Android the **network name needs location permission**
to display; if it's missing, the panel says so and points you at the IP instead — compare the
first three blocks (e.g. `192.168.1.x`) on both devices.

### No Wi-Fi around? Use a hotspot

Tap **"No Wi-Fi network around? Use a phone hotspot"** for step-by-step instructions:

1. On one phone, turn on **Personal Hotspot**.
2. On the other phone, join that hotspot from Wi-Fi settings.
3. Open Nearby on both — you'll now see each other on the radar.

The hotspot only creates a local network between the two phones. **Mobile data is never used**, so
this works with no signal and costs nothing.

### Adding a nearby friend

1. **Tap someone** on the radar (or their chip).
2. A card slides up with their name and whether a Wi-Fi link is open.
3. Tap **Add Friend**.
4. They get a prompt: *"[Your name] wants to connect with you"* with **Accept** / **Decline**.
   Nothing happens until they accept — discovery never auto-connects.
5. Once accepted you both appear in each other's **NEARBY** list.

The card shows the state as it changes: **Request sent** (with a clock), **Request declined**, or
a **Chat** button once you're paired.

### Adding by QR code

If someone doesn't show up on the radar but you're both on the same network, tap the **▣ QR**
icon:

- **My Code** — shows your QR code for them to scan.
- **Scan** — opens the camera to scan theirs. No camera? **Upload Image QR** reads a screenshot
  or photo of the code instead.

Scanning grants no special trust: it just seeds the identity and address, then the normal friend
request runs and the other side still sees the Accept prompt.

### Nearby contacts and chats

Nearby friends live in the **NEARBY** tab with their own status:

- **Green dot + WI-FI DIRECT** — connected directly, ready to move data.
- **Grey dot + OUT OF RANGE** — not reachable right now.
- **GLOBAL FRIEND** badge — this person is also in your internet friends list.

Inbound requests appear above the list under **WANTS TO CONNECT** so you can't miss them.

Nearby chats work exactly like normal chats — text, voice messages, reactions, replies, files,
read receipts. The difference is the route: everything travels straight across the local Wi-Fi.

**Deleting a nearby contact** (🗑 on their row) also wipes your nearby chat history with them, and
asks first. It does **not** remove them from your internet friends list.

> **Desktop works too.** The Windows and Linux apps take part in Nearby over the same LAN, so
> phone → laptop transfers work the same way.

---

## 12. Rooms — ephemeral group chat

Rooms are throwaway group chats. **Anyone who knows the room name can join** — there is no owner,
no invite list and no membership.

### Joining or creating

1. Go to the **ROOMS** tab and tap **Join / Create Room**.
2. Type a room name (it starts you off with `chizchat-lobby`).
3. Tap **JOIN ROOM**.

Creating and joining are the same action: if the room exists you join it, and if it doesn't, it
now does.

### Inside a room

- Everyone's messages are labelled with their name.
- Text, voice messages, files, reactions and replies all work as in a direct chat.
- Your own messages show **"Seen by N"** — tap to see who.
- A **peers panel** lists everyone currently in the room, with a **Search peers…** box.
- **🖥 Share Screen** and **🗑 Clear History** are in the header.

If the room shows **"No other peers connected."** but you know people are there, use the
**reconnect** button on that notice — it renews your connection identity, which fixes the case
where your device's registration has gone stale.

> Rooms are **ephemeral**. There is no history for anyone who wasn't there, and no server keeping
> the room alive.

---

## 13. Workspace — workmates and teams on the office LAN

Workspace is the work counterpart to Nearby: **colleagues on the same office network, no internet
required.** Switch to it with the **WORK** pill at the top of the sidebar.

### Your work identity

The WORK sidebar shows your **work name**, your **work avatar**, and your **device's IP address**
— tap the IP to copy it. The gear icon edits your work profile independently of your personal one.

**Exit Workspace** (the ⎋ icon) takes you back to the personal side.

### Adding a workmate

Colleagues are added by **IP address**, not by code:

1. Tap **Add Workmate**.
2. Ask your colleague for their IP — it's shown under their name in their WORK sidebar.
3. Type it in (e.g. `192.168.1.50`) and tap **Send Request**.
4. They get a **connection request** to accept.

You'll see **"Request sent! Wait for them to accept."** on success, or **"Unable to connect. Check
the IP."** if the address is wrong or they're on a different network.

Workmates show a green/grey dot for presence, with a **⟳ Refresh Presence** button above the list.

Each workmate row has:

- **👤+ Add to Team** — put them in one of your teams.
- **🗑 Delete Workmate** — remove them and their chat history (confirmed first).

### Teams

Teams group workmates for a project.

1. Go to the **TEAMS** tab and tap **Create Team**.
2. Give it a name (e.g. `Engineering`, `Design Sync`) and a short description.
3. Add workmates from their rows, or from the team's edit screen.

Team chats behave like rooms: everyone in the team receives messages, files and replies, and your
own messages show **"Seen by N"**.

Teams sync automatically to the workmates in them, so everyone sees the same team list. Only the
person who created a team can edit or delete it.

### Work chats and file transfer

Workmate and team chats support the same messaging, voice messages, reactions, replies and file
transfer as everywhere else — all over the LAN, with no internet. This is the fastest path for
large files between an Android phone and a desktop.

On Android, an ongoing **"Workspace LAN — Listening for LAN connections"** notification is shown
while the app is available to receive; it stops when you sign out or close the app.

---

## 14. When someone is offline

This is the part of ChizChat that behaves differently from a normal messenger, so it's worth
understanding.

When you write to someone who is offline, the message **stays on your device**. There is no server
holding it for them. The message box even changes its hint to *"Type a message (will send when
online)…"*, and the message shows the yellow **🕐 pending** clock.

**The first time this happens**, ChizChat explains it with a *"Saved on your phone"* card. You can
tick **Don't show this again** once you've got the idea.

**When they come back online** and you open that chat, ChizChat asks:

> **3 unsent messages** — [Name] was offline when you wrote these, so they never left your device.
> **[Name] is online now.** Send them?

- **Send now** — delivers them.
- **Not now** — keeps them queued for later. This is the safe default.
- **Delete these messages instead** — the small link at the bottom; this is the only irreversible
  option, which is why it's the quietest one on the card.

Nothing is ever delivered silently hours later without you deciding to send it.

### Connection status inside a chat

While a direct channel is being established, a banner names each step so the wait is explained
rather than just endured:

- *"Checking your connection…"*
- *"Reconnecting…"*
- *"Connected directly — messages send instantly"* (green)
- *"Couldn't reach [Name] right now. Your message is saved on this device and will send when
  they're back."* (amber)

The **⟳ Refresh Connection** button in the chat header retries on demand.

---

## 15. Notifications

ChizChat notifies you about:

- **New messages** — in any mode.
- **Nearby friend requests** — *"[Name] wants to connect with you"*, with **Accept** and
  **Decline** buttons right on the notification.
- **Accepted requests** — *"[Name] accepted your request"*.
- **Incoming calls**.

Unread counts appear as red badges next to each contact in the sidebar.

On Android, ChizChat also shows **ongoing notifications** while a background feature is genuinely
running — a call in progress, or the LAN listener during file transfers. These are how Android
lets those features keep working with the screen off; they disappear as soon as the feature stops.

---

## 16. Permissions ChizChat asks for

ChizChat only asks for a permission when you first use the feature that needs it.

| Permission | Why it's needed |
|---|---|
| **Notifications** | Message, call and transfer alerts |
| **Microphone** | Voice calls and voice messages |
| **Camera** | Photos in chat, video calls, and scanning QR codes |
| **Photos / Media / Files** | Attaching files, and saving received ones |
| **Location** | Android requires it to read the **Wi-Fi network name**. ChizChat never collects, stores or transmits your location — if you decline, Nearby still works; you just compare IP addresses instead of network names. |
| **Nearby Wi-Fi devices** | Discovering other ChizChat devices on your local network |

---

## 17. Troubleshooting

### "I can't see anyone on the Nearby radar"

The radar itself tells you most of this after 20 seconds, but in order of likelihood:

1. **Different networks.** Compare the **IP** on both devices — the first three blocks should
   match (`192.168.1.**x**`). This is by far the most common cause.
2. **The other person isn't discoverable.** Check the 👁 eye icon on their radar.
3. **The other device doesn't have ChizChat open.**
4. **A guest or public Wi-Fi network is blocking devices from reaching each other.** Many hotel,
   café and corporate guest networks do this deliberately. **Use a phone hotspot instead** — it
   sidesteps the problem entirely and uses no mobile data.

### "A pairing code never connects"

Wait 25 seconds and the **Reconnect and try again** button appears. Tap it — this renews your
device's connection identity, which is the fix when a registration has gone stale. The app
restarts in place and puts you back where you were; then generate a fresh code.

### "My friend is online but my message says pending"

The first message to someone with no open channel spends a few seconds connecting — that's the
difference between the **hollow** and **solid** green dot. Watch the banner in the chat header; if
it ends on *"Couldn't reach…"*, they were reachable a moment ago but aren't now, and your message
is saved for when they're back.

### "A room says no other peers connected"

Use the **reconnect** button on that notice. The room may also just be empty — a room with a
typo'd name is a different room.

### "Adding a workmate fails"

- Check the IP is current — IP addresses change when a device rejoins the network.
- Check you're both on the **same** office network (not one on Wi-Fi guest, one on the main LAN).
- Make sure they have ChizChat open and are in the **WORK** space.

### "I restarted the app and my sent photos look different"

Previews of media *you sent* survive a restart as thumbnails, but the full-resolution original
can't always be recovered — see [Known limitations](#19-known-limitations). Files you *received*
and accepted are on disk in `Documents/ChizChat` and are unaffected.

### "Nothing works and the connection bar is red"

You have no network. For **Friends** and **Rooms** you need internet. For **Nearby** and
**Workspace** you only need to be on the same local network as the other person — a hotspot is
enough.

---

## 18. Privacy and how your data travels

- **Messages and files go device-to-device.** They are not stored on a ChizChat server, because
  there isn't one.
- **A signalling service is used to introduce two devices to each other** for internet chats
  (Firebase Realtime Database). It carries connection metadata so two devices can find each other
  — not your messages or files.
- **Nearby and Workspace use no internet at all.** Traffic stays on your local network.
- **Your history is local.** Uninstalling removes it. There is no backup and no account recovery.
- **Nothing is auto-accepted.** Friend requests, file transfers, calls and screen shares all
  require you to say yes.
- **Location is never collected**, despite the permission — Android only requires it to expose the
  Wi-Fi network name.

---

## 19. Known limitations

Being honest about the edges:

- **Full-resolution originals of media *you sent*** can't always be recovered after an app
  restart; the stored thumbnail stands in. Keeping every sent file would double your storage use,
  which defeats the point of a large-file feature.
- **Voice calls are most reliable when both devices are on the same local network.** There is no
  relay path for audio.
- **Nearby is Android and desktop only**, over local Wi-Fi.
- **Rooms have no history for people who weren't there**, and no moderation — anyone with the name
  can join.
- **The signalling database has no authentication.** It cannot be enumerated (a caller must know
  an exact key), but this is a known gap on the roadmap.
- **Read receipts require both sides on a recent version.** Older builds simply show no ticks —
  nothing breaks.

---

*ChizChat 2.4.38 — built by Sagitta Technologies.*
*Report an issue: https://github.com/logicdreamhub/ChizChat*
