# ChizChat

**A peer-to-peer messenger.** Your messages and files travel directly from your device to the
other person's device whenever they can — your conversations are not kept on a ChizChat server.

Current version: **3.1.2** · Android · Windows · Linux

---

## Download

All files are on the [**latest release**](https://github.com/logicdreamhub/ChizChat/releases/latest) page.

| Platform | File | Size |
|---|---|---|
| **Android** | [Google Play](https://play.google.com/store/apps/details?id=com.sagitta.chizchat) (automatic updates), or [`ChizChat-3.1.2.apk`](https://github.com/logicdreamhub/ChizChat/releases/latest/download/ChizChat-3.1.2.apk) | 11 MB |
| **Windows** | [`ChizChat.Setup.3.1.2.exe`](https://github.com/logicdreamhub/ChizChat/releases/latest/download/ChizChat.Setup.3.1.2.exe) | 144 MB |
| **Linux (Debian/Ubuntu)** | [`chizchat_3.1.2_amd64.deb`](https://github.com/logicdreamhub/ChizChat/releases/latest/download/chizchat_3.1.2_amd64.deb) | 129 MB |

**Installing the APK:** download it on your phone, open it, and allow your browser or file manager
to install unknown apps when Android asks. Android 7.0 or newer. If you already have ChizChat from
Google Play, keep updating it there: Android won't install the APK over the Play version. To switch,
make a backup under **Me** first, uninstall, install the APK and restore. The APK doesn't update
itself, so download each new release from this page.

**Installing on Linux:**

```sh
sudo apt install ./chizchat_3.1.2_amd64.deb
```

---

## What it does

ChizChat gives you four ways to reach people, and you can use all of them at once:

| Mode | Needs internet? | Best for |
|---|---|---|
| **Friends** | Yes | Everyday chat with people anywhere |
| **Nearby** | **No** — one shared Wi-Fi network | Fast, large file transfers between devices in the same place |
| **Rooms** | Yes | Quick, throwaway group chat — anyone with the room name can join |
| **Workspace** | **No** — office LAN | Colleagues and teams on the same office network |

Alongside messaging: voice and video calls, screen sharing, voice messages, photo/file/folder
transfer, read receipts, and QR-code pairing.

## New in 3.1.2

**Everyone needs to update.** Since 3.0.10, ChizChat finds friends through its own relay instead
of Firebase, so 3.0.9 and older can't see 3.1.2, and the other way round.

**Reactions and emoji**
- **Long-press** a message for a quick reaction bar (❤️ 😂 😮 😢 🙏 👍, and **+** for more).
  **Double-tap** sends ❤️.
- Reactions sit neatly under the message, grouped with a count. **Tap one** to see who reacted
  and take yours back.
- Fresh, modern emoji throughout your chats, sharp at every size. One to three emoji sent alone
  show large.
- **Text faces** like :D and <3 turn into emoji (switch it off in Settings → Appearance).

**Forwarding**
- Forward to **up to 10** friends, groups, Rooms or Workspace teams at once, with an optional note.
- Forwarding **photos and files** works again, and receivers see a *Forwarded* label.

**Connections and calls**
- Adding friends is faster and much more reliable.
- Chats and calls carry on when you switch between **Wi-Fi and mobile data**.
- Messages that didn't arrive are **sent again automatically**.
- **New call screens**: quick replies, video calls and call history in the chat. Group calls in
  Rooms let people join and leave without ending the call.
- Calling someone whose app is closed: you **hear it ring**, and answering opens the call.

**Android**: the app icon now fills its shape on your home screen.

## Run your own Quiver server

**[Quiver](https://github.com/logicdreamhub/quiver)** is the open-source server behind offline
delivery. *The mailbox that can't read your mail.*

- 🏢 **Companies**: run it on the office network, so colleagues' messages arrive even when a laptop
  is shut, and nothing leaves the building.
- 💼 **Hosting providers**: offer offline delivery as a subscription, with access codes built in.
- 👨‍👩‍👧 **Communities and families**: a small VPS is all it takes.

It's one command with Docker, and there's a
[step-by-step VPS guide](https://github.com/logicdreamhub/quiver/blob/main/docs/deploy-vps.md).

## First run

There is no account, no password, and no phone number. You type the name friends should see and
tap **Get started**; ChizChat generates a **Peer ID** for your device (something like
`chizchat-a3f19c02d8b41e77`), which is your address on the network. You'll find it under
**Settings → About**.

Your identity lives on that device. Installing ChizChat on a second device creates a *different*
identity — your friends there will need to add you again.

## Privacy

- **Messages and files go device-to-device** whenever the two devices can reach each other, and
  they are encrypted in transit either way.
- **When a direct link isn't possible** (often on mobile data), the connection goes through a relay
  run by ChizChat. The relay passes encrypted traffic along; it can't read your messages, calls or
  files and doesn't store them.
- **A signalling service introduces two devices to each other** for internet chats (Firebase
  Realtime Database). It carries connection metadata so two devices can find each other — not your
  messages or files.
- **Nearby and Workspace use no internet at all.** Traffic stays on your local network.
- **Offline delivery** uses ChizChat's own Quiver server by default, or one you choose, or none if
  you disconnect. Messages left there are end-to-end encrypted: the operator can't read them or see
  who sent them, and unread ones are deleted after 30 days.
- **Labels, notes, quick replies and your catalog stay on your device** (and in your backup).
  A business profile is shared only with your own contacts, device to device. Payment details go
  only to the chats you send them to.
- **Your history is local.** Uninstalling removes it. There is no account recovery — only a
  password-protected backup you made yourself brings it back.
- **Nothing is auto-accepted unless you turn it on.** Friend requests, calls and screen shares
  always require you to say yes; file transfers do too, unless you enable auto-accept for a contact.

Known limitations are documented honestly in the [user guide](USER_GUIDE.md#19-known-limitations).

---

## Documentation

The full **[User Guide](USER_GUIDE.md)** covers every feature, all four connection modes,
permissions, and troubleshooting.

## Issues

Report a problem via [GitHub Issues](https://github.com/logicdreamhub/ChizChat/issues).

---

*Developed by Sagitta Technologies.*
