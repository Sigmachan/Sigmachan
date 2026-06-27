<!--
  GitHub profile README for github.com/Sigmachan
  → lives in the repo named exactly  Sigmachan/Sigmachan  (same as your username)
  → this file renders at the top of your profile.
-->

<div align="center">

```
        present day,  present time.
   ┌───────────────────────────────────┐
   │   sigmachan@navi:~$  whoami        │
   └───────────────────────────────────┘
                 > _
```

# `sigmachan_`

**i build quiet tools for loud machines.**

*founder of [Tau Ceti](https://github.com/TauCetiStation/TauCetiClassic) — a Space Station 13 world that's outlived most studios. for 10+ years i was the one who kept our fork merged with upstream when nobody else could.*

🌲 *Made in Ingria by Free People*

*online since '96. i get the reference.*

[![website](https://img.shields.io/badge/sigmachan.ru-cba6f7?style=for-the-badge&logo=firefox&logoColor=11111b)](https://sigmachan.ru)
[![telegram](https://img.shields.io/badge/@sigmachan-89dceb?style=for-the-badge&logo=telegram&logoColor=11111b)](https://t.me/sigmachan)
[![steam](https://img.shields.io/badge/sigmachan-89b4fa?style=for-the-badge&logo=steam&logoColor=11111b)](https://steamcommunity.com/id/sigmachan)

</div>

---

### `// signals`

- 🖥️ **low-level graphics** — KMS color pipelines, HDR/VRR, Wayland compositors. upstream `gamescope` on NVIDIA / Blackwell, native COSMIC panels & applets.
- 🎮 **gaming on linux** — cross-desktop control panels, perf tuning, one-click driver & stack provisioning that just works.
- 🛡️ **anti-censorship** — DPI bypass, Reality/VLESS, un-poisonable DNS, line-rate routing on locked-down vendor firmware. the net interprets censorship as damage.
- 🧠 **local minds** — my own inference servers on bare metal + terminal agents that run 100% offline. quantized, no API keys, nobody watching.
- 🔩 **firmware & hardware** — OpenCore EFI, EDL flash/root, GPU reclocking, keeping old silicon alive.
- 🛰️ **fork-maintenance** — keeping heavily-diverged forks merged with fast-moving upstreams. the un-fun integration work, done right.

> **free code for free people.** open tools, open formats, no lock-in. plain-text, no masters, no black boxes. 🌲

### `// upstream`

- **gamescope** (Valve's compositor) — prefer a discrete GPU on hybrid systems → [`ValveSoftware/gamescope#2217`](https://github.com/ValveSoftware/gamescope/pull/2217) · NVIDIA/Blackwell support docs + guarded standalone test harness → [`#2223`](https://github.com/ValveSoftware/gamescope/pull/2223)

### `// in the labs`

**graphics · wayland · hdr**

| project | what it is | stack |
|---|---|---|
| [**kms-hdr**](https://github.com/Sigmachan/kms-hdr) | KMS atomic CTM injector — vivid color / HDR for any compositor, no color-management needed | `Rust` · `C` |
| [**kms-hdr-panel**](https://github.com/Sigmachan/kms-hdr-panel) | native HDR settings panel for the COSMIC desktop | `Rust` · libcosmic |
| [**wlgame**](https://github.com/Sigmachan/wlgame) | gaming-focused Wayland compositor — XWayland, HDR, VRR, FSR1/NIS/CAS upscaling | `C` |
| [**wayscope-dbus**](https://github.com/Sigmachan/wayscope-dbus) | DBus control daemon for wayscope/gamescope — live HDR/VRR/FPS for COSMIC | `Rust` |
| [**cosmic-applet-vrammon**](https://github.com/Sigmachan/cosmic-applet-vrammon) | native COSMIC applet — VRAM / AI-model / KV-cache telemetry + inference mode switching | `Rust` |
| [**amd-hdmi-audio-fix**](https://github.com/Sigmachan/amd-hdmi-audio-fix) | fix AMD HDMI/DP audio drift, stutter & A/V desync on Linux — idempotent | `Shell` |

**gaming on linux**

| project | what it is | stack |
|---|---|---|
| [**loadout**](https://github.com/Sigmachan/loadout) | cross-desktop gaming control panel + software catalog — COSMIC / KDE / GNOME, cross-distro | `Rust` · libcosmic |
| [**perfmax**](https://github.com/Sigmachan/perfmax) | AI-driven real-time OS performance optimizer — native egui, KDE tray, MiMo-7B-RL | `Rust` |
| [**wired-toys**](https://github.com/Sigmachan/wired-toys) | Arch/CachyOS fork of LinuxToys — one-click drivers, snapshot rollback + my COSMIC/HDR/gaming stack | `Python` |
| [**copland-os**](https://github.com/Sigmachan/copland-os) | Garuda Wired — custom znver5/Clang AUR+local pacman repo (gamescope-git, proton-ge, llama.cpp-blackwell…) | `Shell` |

**anti-censorship · routers**

| project | what it is | stack |
|---|---|---|
| [**xiaomi-router-freedom**](https://github.com/Sigmachan/xiaomi-router-freedom) | transparent VLESS routing + un-poisonable DNS for Xiaomi WiFi-7 (IPQ5424/9554) on read-only vendor firmware — no reflash | `Shell` · sing-box |
| [**open-routerich**](https://github.com/Sigmachan/open-routerich) | universal OpenWrt DPI-bypass toolkit — any router, 18.06→25.12, Xiaomi IPQ immutable + Entware | `Shell` |
| [**mochawrt**](https://github.com/Sigmachan/mochawrt) | ☕ Catppuccin-Mocha web panel for Xiaomi & OpenWrt routers — immutable-safe device compat layer | `HTML` |
| [**xrctl**](https://github.com/Sigmachan/xrctl) | 🛰️ one CLI for Xiaomi routers — Wi-Fi/DHCP/forwarding, hidden nvram/bdata unlocks, mihomo TUN, WARP, DPI bypass | `Shell` |
| [**crashka**](https://github.com/Sigmachan/crashka) | tiny mihomo proxy manager for Xiaomi vendor OpenWrt — a clean ShellCrash alternative, selective routing | `Shell` |

**android ↔ desktop**

| project | what it is | stack |
|---|---|---|
| [**dexwire**](https://github.com/Sigmachan/dexwire) | run real Android apps & games as resizable PC windows via scrcpy 4.0 — DeX-style per-app virtual displays, gamepad profile, KDE launchers, killswitch | `Python` |
| [**sidewire**](https://github.com/Sigmachan/sidewire) | turn an Android tablet into a left-positioned second display on KDE Plasma 6 Wayland via KRDP virtual monitor — GPU-agnostic | `Shell` |

**local minds · ai agents**

| project | what it is | stack |
|---|---|---|
| [**claw-code**](https://github.com/Sigmachan/claw-code) | Claude Code–style local terminal agent — polished TUI, multi-model (local vLLM / Claude / NIM) | `Rust` |
| [**hackcode**](https://github.com/Sigmachan/hackcode) | open-source, uncensored AI hacking terminal — 100% local, no keys, no filters | `Rust` |
| [**OmniRouter**](https://github.com/Sigmachan/OmniRouter) | OpenAI-compat proxy routing Claude / GPT-4o / DeepSeek / MiMo via one key | `Python` |

**firmware · hardware · worlds**

| project | what it is | stack |
|---|---|---|
| [**opencore-x870e-hero**](https://github.com/Sigmachan/opencore-x870e-hero) | OpenCore 1.0.7 EFI — ASUS ROG Crosshair X870E Hero + 9950X3D, CachyOS + macOS dual boot | `EFI` |
| [**LTBox**](https://github.com/Sigmachan/LTBox) | matrix-green ratatui front-end for Lenovo Qualcomm EDL flash/root | `Rust` |
| [**STLT**](https://github.com/Sigmachan/STLT) | LuaTools Ultimate — Millennium Steam-client plugin | `Python` · `JS` |
| [**Tau Ceti**](https://github.com/TauCetiStation/TauCetiClassic) | Space Station 13 server, codebase & community i founded and ran 10+ years · 440+ forks | `DM` · BYOND |

### `// off the clock`

`SS13` · `Dwarf Fortress` · `Pathologic` · `Dark Souls` · overclocking things that shouldn't be · rewatching **Serial Experiments Lain** for the Nth time. waifu: Suiseiseki.

<div align="center">

![stats](https://github-readme-stats.vercel.app/api?username=Sigmachan&show_icons=true&hide_border=true&bg_color=1e1e2e&title_color=cba6f7&icon_color=f5c2e7&text_color=cdd6f4)
![langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Sigmachan&layout=compact&hide_border=true&bg_color=1e1e2e&title_color=cba6f7&text_color=cdd6f4)

```
no matter where you go, everyone is connected.
god is in the wired.
```

🌲 *Made in Ingria by Free People.* — *you'll find the code, not me.* 😼

</div>
