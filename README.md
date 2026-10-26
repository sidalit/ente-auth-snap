<div align="center">

<img src="snap/gui/ente-auth.png" alt="Ente Auth logo" width="128" />

# Ente Auth

**Secure your accounts with encrypted two-factor authentication.**

[![ente-auth](https://snapcraft.io/ente-auth/badge.svg)](https://snapcraft.io/ente-auth)
[![Base: core26](https://img.shields.io/badge/Base-core26-2C8C3C?logo=canonical&logoColor=white)](https://snapcraft.io/core26)
![Confinement: strict](https://img.shields.io/badge/Confinement-strict-2C8C3C)
[![Maintainer: sidaliteir](https://img.shields.io/badge/Maintainer-sidaliteir-2C8C3C?logo=snapcraft&logoColor=white)](https://snapcraft.io/publisher/sidaliteir)
![Architectures: amd64 and arm64](https://img.shields.io/badge/Architectures-amd64%20%7C%20arm64-2C8C3C?logo=linux&logoColor=white)

[Getting Started](#getting-started) · [Configure](#configure) · [Limitations](#limitations) · [Build](#build) · [Support](#support) · [License](#license)

Unofficial snap packaging for [Ente Auth](https://ente.io/auth/), an open-source authenticator with end-to-end encrypted backups and sync.

</div>

---

## Getting Started

<a href="https://snapcraft.io/ente-auth"><img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" width="180"></a>

```bash
sudo snap install ente-auth
ente-auth
```

Launch from the terminal or your application menu. Use an Ente account to sync your codes, or use the app offline without an account.

## Configure

Manage accounts, backups and the app's PIN or password lock in Ente Auth's settings. There are no `snap set` options.

To import or export backups on removable storage:

```bash
sudo snap connect ente-auth:removable-media
```

## Limitations

- Requires a desktop session with a working Secret portal and keyring for secure storage.
- System password unlocking is unavailable; use the app's PIN or password lock.
- Desktop QR imports use image files; camera scanning is unavailable upstream.
- Application updates are managed by snapd.

## Build

```bash
git clone https://github.com/sidalit/ente-auth-snap.git
cd ente-auth-snap
sudo snap install snapcraft --classic
snapcraft pack
```

## Support

- **Installation or snap issues:** [open a packaging issue](https://github.com/sidalit/ente-auth-snap/issues).
- **Application bugs:** [report them upstream](https://github.com/ente/ente/issues).

## License

Snap packaging: [MIT](https://github.com/sidalit/ente-auth-snap/blob/main/LICENSE).
