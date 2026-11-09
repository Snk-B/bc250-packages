# AMD BC-250 CachyOS Pacman Repository

Official pre-compiled rolling-release package repository for the **AMD BC-250 (Sony PS5 Oberon APU)** running **CachyOS Linux**.

---

## ?? Quick Setup (Universal for Fish, Bash & Zsh)

Add the official repository to `/etc/pacman.conf`:

```bash
printf "\n[bc250-cockpit]\nSigLevel = Optional TrustAll\nServer = https://snk-b.github.io/bc250-packages/\$arch\n" | sudo tee -a /etc/pacman.conf
```

Synchronize package databases and install:

```bash
sudo pacman -Sy --overwrite "*" bc250-cockpit-pro
```

*(Note: `--overwrite "*"` ensures a clean migration if you previously installed via manual git clone).*

---

## ?? Available Packages

| Package | Version | Description |
| :--- | :--- | :--- |
| **`bc250-cockpit-pro`** | **1.1.1-3** | Industrial-grade telemetry daemon, GDDR6 memory collector, standalone Web dashboard & native KDE Plasma 6 Cyber Widgets Suite. |

---

*Maintained by [Davidson Braga (Snk-B)](https://github.com/Snk-B).*
