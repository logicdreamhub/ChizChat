# ChizChat

**A peer-to-peer messenger.** Your messages and files travel directly from your device to the
other person's device — there is no ChizChat server in the middle holding your conversations.

Current version: **3.0.5** · Android · Windows · Linux

---

## Download

### Android

[**Get it on Google Play**](https://play.google.com/store/apps/details?id=com.sagitta.chizchat) — with automatic updates.

### Windows and Linux

| Platform | File | Size |
|---|---|---|
| **Windows** | [`ChizChat.Setup.3.0.5.exe`](https://github.com/logicdreamhub/ChizChat/releases/latest) | 129 MB |
| **Linux (Debian/Ubuntu)** | [`chizchat_3.0.5_amd64.deb`](https://github.com/logicdreamhub/ChizChat/releases/latest) | 120 MB |

Both are on the [**latest release**](https://github.com/logicdreamhub/ChizChat/releases/latest) page.

Installing on Linux:

```sh
sudo apt install ./chizchat_3.0.5_amd64.deb
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

## First run

There is no account, no password, and no registration. You type a display name and tap
**INITIALIZE**; ChizChat generates a **Peer ID** for your device (something like
`chizchat-a3f19c02d8b41e77`), which is your address on the network.

Your identity lives on that device. Installing ChizChat on a second device creates a *different*
identity — your friends there will need to add you again.

## Privacy

- **Messages and files go device-to-device.** They are not stored on a ChizChat server, because
  there isn't one.
- **A signalling service introduces two devices to each other** for internet chats (Firebase
  Realtime Database). It carries connection metadata so two devices can find each other — not your
  messages or files.
- **Nearby and Workspace use no internet at all.** Traffic stays on your local network.
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

*Built by Sagitta Technologies.*
