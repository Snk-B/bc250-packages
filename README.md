# AMD BC-250 CachyOS Pacman Repository

Official pre-compiled rolling-release package repository for the **AMD BC-250 (Sony PS5 Oberon APU)** running **CachyOS Linux**.

---

## ?? Quick Setup

Add the repository to `/etc/pacman.conf`:

```bash
sudo tee -a /etc/pacman.conf << 'EOF'

[bc250-cockpit]
SigLevel = Optional TrustAll
Server = https://snk-b.github.io/bc250-packages/$arch
EOF
```

Synchronize package databases and install:

```bash
sudo pacman -Sy bc250-cockpit-pro
```

---

## ?? Available Packages

| Package | Version | Description |
| :--- | :--- | :--- |
| **`bc250-cockpit-pro`** | **1.1.1-1** | Industrial-grade telemetry daemon, standalone Web dashboard & native KDE Plasma 6 Cyber Widgets Suite. |

---

*Maintained by [Davidson Braga (Snk-B)](https://github.com/Snk-B).*
