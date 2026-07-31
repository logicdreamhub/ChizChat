# ChizChat

**A peer-to-peer messenger.** Your messages and files travel directly from your device to the
other person's device — there is no ChizChat server in the middle holding your conversations.

Current version: **2.4.38** · Android · Windows · Linux

---

## Download

| Platform | File | Size |
|---|---|---|
| **Android** | [`chizchat_2.4.38.apk`](https://github.com/logicdreamhub/ChizChat/releases/latest) | 10.7 MB |
| **Windows** | [`ChizChat.Setup.2.4.38.exe`](https://github.com/logicdreamhub/ChizChat/releases/latest) | 120 MB |
| **Linux (Debian/Ubuntu)** | [`chizchat_2.4.38_amd64.deb`](https://github.com/logicdreamhub/ChizChat/releases/latest) | 120 MB |

All downloads are on the [**latest release**](https://github.com/logicdreamhub/ChizChat/releases/latest) page.

Installing on Linux:

```sh
sudo apt install ./chizchat_2.4.38_amd64.deb
```

On Android you'll need to allow installing from unknown sources to sideload the APK.

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
- **Your history is local.** Uninstalling removes it. There is no backup and no account recovery.
- **Nothing is auto-accepted.** Friend requests, file transfers, calls and screen shares all
  require you to say yes.

Known limitations are documented honestly in the [user guide](USER_GUIDE.md#19-known-limitations).

---

## Documentation

The full **[User Guide](USER_GUIDE.md)** covers every feature, all four connection modes,
permissions, and troubleshooting.

## Issues

Report a problem via [GitHub Issues](https://github.com/logicdreamhub/ChizChat/issues).

---

*Built by Sagitta Technologies.*
