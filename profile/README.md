<p align="center">
  <img src="https://raw.githubusercontent.com/pbolt-dev/.github/main/assets/pbolt-logo.svg" alt="pbolt logo" width="160" height="160" />
</p>

<h1 align="center">pbolt</h1>

<p align="center">
  <strong>Fast, automation-friendly CLI, Go SDK, and in-memory credential agent compatible with Passbolt.</strong>
</p>

<p align="center">
  <a href="https://github.com/pbolt-dev/go-pbolt-cli"><img src="https://img.shields.io/badge/CLI-go--pbolt--cli-0bddec?style=flat-square&logo=go" alt="go-pbolt-cli" /></a>
  <a href="https://github.com/pbolt-dev/go-pbolt"><img src="https://img.shields.io/badge/SDK-go--pbolt-199ee9?style=flat-square&logo=go" alt="go-pbolt" /></a>
  <a href="https://github.com/pbolt-dev/go-pbolt-cli/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-fdae15?style=flat-square" alt="License: MIT" /></a>
</p>

---

## ⚡ Overview

**pbolt** is a community-driven fork of the official Passbolt Go CLI and SDK. It is built for engineers, DevOps teams, and automation workflows that require frictionless security without compromising cryptographic integrity.

While fully maintaining wire-format and server API compatibility with [Passbolt](https://www.passbolt.com), **pbolt** eliminates daily friction points in local dev loops, shell scripts, and CI/CD pipelines.

---

## 🚀 Key Highlights & Enhancements

- 🔑 **Interactive Auth Agent (`pbolt auth agent`)**: In-memory token caching daemon with session TTL. Authenticate once with your passphrase and 2FA/TOTP; subsequent commands reuse the active session seamlessly.
- ⚡ **Zero-Plaintext Integration (`--raw` Output)**: Output secret values directly to stdout without formatting overhead, enabling zero-disk-storage token chaining with CLIs like `hcloud` (`token_command`), `curl`, and custom scripts.
- 🛠️ **Full Administrative API Coverage**:
  - Complete user lifecycle management (activate, suspend, delete, recover).
  - Organization settings inspection and configuration.
  - Group membership administration (safe demotions, member management, detail views).
- 🔄 **Drop-in Compatibility**: Command aliases and compatibility symlinks allow `pbolt` to serve as a seamless drop-in replacement for `passbolt`.

---

## 📦 Projects

| Repository | Description |
| :--- | :--- |
| [**`go-pbolt-cli`**](https://github.com/pbolt-dev/go-pbolt-cli) | Feature-complete CLI and authentication agent for Passbolt. |
| [**`go-pbolt`**](https://github.com/pbolt-dev/go-pbolt) | Robust Go SDK / API client supporting all administrative and user endpoints. |

---

## 💻 Quick Install

Download ready-to-run release binaries for Linux, macOS, and Windows from our [Releases page](https://github.com/pbolt-dev/go-pbolt-cli/releases), or install via Go:

```bash
go install github.com/pbolt-dev/go-pbolt-cli@latest
```

---

## ⚖️ Trademark Notice

*Passbolt is a registered trademark of Passbolt SA. **pbolt** is an independent community project and is not affiliated with, endorsed by, or sponsored by Passbolt SA.*

---

<p align="center">
  <sub>Built with ❤️ by the open-source community for developers who love automation.</sub>
</p>
