<div align="center">

<img src="beam-icon.png" width="128" alt="Beam"/>

# Beam

**🇬🇧 English** · [🇫🇷 Français](README.fr.md) · [🇪🇸 Español](README.es.md)

Fast, native macOS screen-sharing & remote control — Mac to Mac.

[**⬇︎ Download Beam.dmg**](https://github.com/Titi257/beam/releases/latest/download/Beam.dmg)

</div>

---

See and **control** another Mac (mouse + keyboard), on your local network or over the Internet, end-to-end encrypted. **Universal** app (Intel + Apple Silicon).

- **Three connection modes, chosen automatically — nothing to configure:**
  - **Local network (LAN)**: two Macs on the same network connect **directly**, no server, lowest latency.
  - **Direct (P2P)**: over the Internet, Beam tries a direct peer-to-peer link to bypass the relay when the network allows.
  - **Relay (Internet)**: otherwise, traffic goes through the **nearest** relay (multi-region) — works behind any router, from anywhere.
- Connect from anywhere by **ID** — no IP or server address to type.
- **Full remote control** (mouse + keyboard), or **read-only mode** (view without controlling).
- **AnyDesk-style pairing**: "Share my screen" gives a **9-digit ID** that's stable per machine; the other Mac types it.
- **End-to-end encrypted** (X25519 ECDH + AES-GCM) — neither the LAN link nor the relay ever sees anything but ciphertext. A **security code** shown on both sides can be compared aloud to detect an active man-in-the-middle.
- **Shared clipboard** (text + image) and a live **quality readout** (FPS, throughput, latency, direct vs relay).
- **Automatic updates** built in.

## Requirements

- **macOS 14 (Sonoma) or newer.**
- **Intel or Apple Silicon Mac** — universal, native on both.

## Install

1. Download **`Beam.dmg`** from the [latest release](https://github.com/Titi257/beam/releases/latest).
2. Open it and drag **Beam** into **Applications**.
3. Launch **Beam** from Applications.

> The app is signed & notarized by Apple — no "unidentified developer" warning.

## Use

In the single window:

- **Share my screen** → you get an **ID**. Give it to whoever should see your screen. On connect you get an **Accept / Deny** prompt; accepting grants keyboard/mouse control (unless **read-only** is on).
- **Control another Mac** → type the other Mac's **ID** and click **Connect**.

There's **nothing to configure**: Beam connects directly on your local network when possible, and otherwise uses its built-in relay automatically (picking the nearest one). A relay address lives in an optional **advanced** section you normally never need to touch.

First use prompts for **Screen Recording**, **Accessibility**, and (LAN mode) **Local Network** — macOS only asks the side that needs each.

## Updates

Beam checks for updates automatically and offers **App ▸ Check for Updates…**. Each update is cryptographically signed and verified before it installs.

## Privacy & security

Media is **always end-to-end encrypted**. The relay (Internet mode) only ever sees ciphertext. The code has been **reviewed for security** (frame-size limits, hardened key-verification code), but it has **not had a formal independent audit** — treat it accordingly.
