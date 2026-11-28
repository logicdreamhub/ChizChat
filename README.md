# ChizChat

**A peer-to-peer messenger.** Your messages and files travel directly from your device to the
other person's device whenever they can — your conversations are not kept on a ChizChat server.

Current version: **3.3.3** · Android · Windows · Linux

---

## Download

All files are on the [**latest release**](https://github.com/logicdreamhub/ChizChat/releases/latest) page.

| Platform | File | Size |
|---|---|---|
| **Android** | [Google Play](https://play.google.com/store/apps/details?id=com.sagitta.chizchat) (automatic updates), or [`ChizChat-3.3.3.apk`](https://github.com/logicdreamhub/ChizChat/releases/latest/download/ChizChat-3.3.3.apk) | 11 MB |
| **Windows** | [`ChizChat.Setup.3.3.3.exe`](https://github.com/logicdreamhub/ChizChat/releases/latest/download/ChizChat.Setup.3.3.3.exe) | 148 MB |
| **Linux (Debian/Ubuntu)** | [`chizchat_3.3.3_amd64.deb`](https://github.com/logicdreamhub/ChizChat/releases/latest/download/chizchat_3.3.3_amd64.deb) | 130 MB |

**Installing the APK:** download it on your phone, open it, and allow your browser or file manager
to install unknown apps when Android asks. Android 7.0 or newer. If you already have ChizChat from
Google Play, keep updating it there: Android won't install the APK over the Play version. To switch,
make a backup under **Me** first, uninstall, install the APK and restore. The APK doesn't update
itself, so download each new release from this page.

**Installing on Linux:**

```sh
sudo apt install ./chizchat_3.3.3_amd64.deb
```

---

## What it does

ChizChat gives you four ways to reach people, and you can use all of them at once:

| Mode | Needs internet? | Best for |
|---|---|---|
| **Friends** | Yes | Everyday chat with people anywhere |
| **Nearby** | **No** — two Android phones need no network at all; a laptop needs shared Wi-Fi | Chat and fast, large file transfers between people in the same place |
| **Rooms** | Yes | Quick, throwaway group chat — anyone with the room name can join |
| **Workspace** | **No** — office LAN | Colleagues and teams on the same office network |

Alongside messaging: voice and video calls, screen sharing, voice messages, photo/file/folder
transfer, read receipts, QR-code pairing, threads, and notes and checklists.

## New in 3.3.3

3.3.3 chats with 3.3.3 as before. Threads need 3.3.3 on every member's device: friends on
older versions are marked in the invite list and join once they update.

**Threads**
- A chat about **one topic** (a trip, an event, an order) with the friends it concerns. They
  don't need to know each other. Find them under **Groups**.
- **Polls**, **task lists** everyone can tick off, and **events** with Going / Maybe / Can't go
  and a reminder.
- **Mark decisions** so nobody has to scroll for them. Photos, files, voice messages,
  reactions, edits, and *Seen by*.
- **Close** a thread with an outcome when it's done, reopen it any time, and **export a
  summary** to keep or print.
- There is no server: the creator's phone passes messages on, so they move while the creator
  is online.

**Notes and checklists**
- Keep a checklist or a plain note with each chat, with due dates and pinning.
- **Long-press** any message → *Add to notes*. Send a copy to a friend, who can save it as
  their own.

**Chats**
- **Edit** messages you sent, and **pin** up to three messages in a chat.
- Search jumps **straight to the message** and highlights it.
- Unsent text is kept as a **draft** for each chat.
- **Paste** screenshots, photos and files into a chat, with a preview before sending.
- Files: **Open with…**, **Save to device** and **Show in folder**.

**Support for businesses**
- **Tickets** in one-to-one chats: open, waiting, resolved, closed, with a rating at the end.
- Customers can send **device info** (they see and choose every part first).

**Rooms**
- Leave a room and rejoin it later from the list of rooms you've joined.
- Safer rooms: nobody can post as someone else.

**Remote control** (desktop screen sharing in direct chats)
- Allowing control now works: mouse, clicks, scrolling and typing. A phone can control a
  computer with touch gestures and its own keyboard row.

**Workspace**
- Team files reach every member who accepts. Reactions reach workmates and teams.
- Team messages show **who they did not reach**.

**Nearby**
- **Reactions** now reach the other phone.
- Friend requests can't be faked: only someone you asked can accept.
- The radar only counts people who are actually around, and says when a request can't reach
  someone.

**Fixes**
- Local Wi-Fi chats (Nearby and Workspace) **reconnect on their own** after an app restart.
  Before, messages could be lost while showing as sent.
- On tablets and wide windows, the long-press menu now opens beside the message instead of
  hiding under the chat list.

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
- **A signalling service introduces two devices to each other** for internet chats: ChizChat's
  own relay at `quiver.conewer.com`. It carries connection metadata so two devices can find each
  other — not your messages or files.
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
