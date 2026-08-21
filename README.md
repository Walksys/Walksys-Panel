# Walksys Panel 🚀

Welcome to **Walksys Panel**, a game server management & container orchestration platform built for Minecraft and generic game servers.

**Created & Maintained by [Walksys](https://github.com/Walksys)**

**Version:** `v3.1.0`

---

## ✨ Features

* ⚡ **Dual Runtime Modes**: Run servers natively via host processes or isolated Docker containers (`itzg/minecraft-server`, generic node/python images).
* ☕ **Multi-Version Java Engine**: Built-in support for Java 8, 11, 16, 17, and 21 with automatic version detection.
* 🛡️ **Enhanced Security & Safeguards**:
* Strict 32+ char `JWT_SECRET` requirement in production environments.
* IP-based rate limiting on authentication routes to prevent brute-force attacks.
* Granular RBAC enforcing owner assignment privileges exclusively to administrators.
* Least-privilege POSIX file modes across server files, folders, and archives (anti-`0o777`).
* Pre-flight `DataVersion` world corruption safety check with admin-gated bypass.
* Configurable Socket.IO and Express CORS origin allowlisting via `ALLOWED_ORIGINS`.
* 2GB upload protection with HTTP 413 error handling to prevent disk-fill DoS.


* 📡 **Telemetry & Nodes**: Live CPU, RAM, and Disk telemetry graphs and support for Pterodactyl Wings daemons.
* 🌐 **Built-in Playit.gg Tunnels**: Allocate public IPs and custom hostnames without opening router ports.
* 💻 **Real-Time Web Terminal**: WebSocket console stream with color-coded log parsing and live command execution.
* 📁 **Complete File Manager**: Web-based file explorer, syntax-highlighted code editor, chunked uploads, zip/unzip, and SFTP support.
* 🔄 **One-Click Updates**: Automated background self-updating script (`update.sh`).

---

## 📦 Quick Installation

Run the automated installer on your VPS / Linux machine:

```bash
bash install.sh

```

This opens an interactive menu that sets up all dependencies (Node.js, Docker, Java runtimes, firewall rules) and creates your initial Administrator credentials.

---

## 🔄 Updating

To pull the latest changes and update the panel, simply run:

```bash
bash update.sh

```

---

## 🗑️ Uninstallation

To uninstall the panel while safely preserving your game server worlds and files in `.data/`:

```bash
bash uninstall.sh

```

---

## 🚀 Highlights & Improvements (v3.1.0)

* **🛡️ Stronger Security**: Safer Login | Secure JWT | Protected Accounts | Safe File Access
* **🌍 World Protection**: Version Safety | Downgrade Block | Safer Server Boot
* **📁 Upload Safety**: 2GB Limit | Safe Permissions | Secure Downloads
* **📈 Accurate Resources**: Real Server RAM | No VPS RAM | Better CPU Stats
* **🔗 Playit Upgrade**: Tunnel Health | Port Checks | Safe Recovery | Player Protection
* **🤖 Smart Recovery**: No Blind Restarts | Player-Safe Restart | Auto Retry
* **🔐 Safer Logs**: Hidden Tokens | Protected Keys | Clean Diagnostics
* **✅ Fully Verified**: 18 Tests Passed | Build Checked | Ready to Use

---

## 📄 License & Attribution

This project is licensed under the **MIT License** with attribution requirements.

> **Important**: You are free to use, modify, host, and distribute this project, but you **MUST give proper attribution and credit to the original author (Walksys / Walksys Panel)** in all copies or derivative works.

See the [LICENSE](/LICENSE) file for complete license terms.

---

If u want to report some issues and bugs, please let me know on the report channel or via a ticket.

**Update Command:**

```bash
bash <(curl -s https://raw.githubusercontent.com/Walksys/Walksys-Panel/refs/heads/main/install.sh)

```
