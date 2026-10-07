# Rex Browser

**An AI browser for Windows, Linux and Android, with the REX agent built in.**

Rex Browser is a fast, private web browser with an AI agent in a side panel. The agent can read
pages, click, type, fill forms and call APIs to automate real work — while you watch and can take
over at any moment. Everyday browsing and web search are free and need no account; the agent uses
your [rxdsec](https://rxdsec.tech) account.

> This repository hosts the released builds. Download the latest from the
> **[Releases page »](https://github.com/rxdsec634/rex-browser/releases/latest)**

---

## Download

| Platform | File | Notes |
|---|---|---|
| **Windows 10/11** (x64) | `rex-browser-setup-<version>.exe` | Installer. Auto-updates. |
| **Linux** — Debian/Ubuntu/Kali | `rex-browser-<version>-amd64.deb` | Installs to `/opt/Rex Browser`. Auto-updates. |
| **Linux** — any distro | `rex-browser-<version>-x64.tar.gz` | Extract and run. Manual updates. |
| **Android 8.0+** | `rex-browser-<version>.apk` | Sideload. Auto-updates. |

### Install

**Windows** — run the `.exe`. It isn't code-signed yet, so Windows SmartScreen may warn:
click **More info → Run anyway**.

**Linux (.deb)**
```bash
sudo apt install ./rex-browser-<version>-amd64.deb
rex-browser
```

**Linux (tarball)**
```bash
tar -xzf rex-browser-<version>-x64.tar.gz
cd rex-browser-<version>-x64
./rex-browser
```

**Android** — enable "Install unknown apps" for your browser/files app, then open the `.apk`.
If you installed an earlier test build, uninstall it first (the signing key changed).

---

## What's inside

- **The REX agent, built in** — web, browser and HTTP tools with 40+ model providers and
  adjustable thinking effort. Pause and take over mid-task; it never acts behind your back.
- **Security** — malware and phishing site blocking, automatic HTTPS upgrades, warnings before
  risky downloads, and secure DNS (desktop).
- **Privacy** — ad and tracker blocking (Shields), Global Privacy Control / Do Not Track, and a
  private browsing mode the agent cannot see. Your data stays on your device; page content is sent
  only to the AI provider you choose, only when you use the agent.
- **Everywhere** — Windows, Linux and Android, with one rxdsec account across them all.

## Accounts

Browsing and web search are free and need no sign-in. The **agent** needs an rxdsec account —
the same one used by the [REX agent](https://rxdsec.tech). Sign in from the agent panel.

## Updates

Rex Browser updates itself from this repository's releases. Every download is verified against the
SHA-256 checksum GitHub publishes for the asset before it is installed; a mismatch is discarded.
On Android, the system installer asks you to confirm each update.

## Verify a download (optional)

Each release lists a SHA-256 for every file. To check one yourself:

```bash
# Windows (PowerShell)
Get-FileHash .\rex-browser-setup-<version>.exe -Algorithm SHA256

# Linux / macOS
sha256sum rex-browser-<version>-amd64.deb
```

## Security & responsible use

The browser's agent includes an optional web security-testing toolset. It is **off by default** and
does nothing until you enable it and name in-scope targets in **Settings → Agent → Security
testing**. Only test systems you own or are explicitly authorized to assess.

Found a security issue? Please report it privately via https://rxdsec.tech rather than opening a
public issue.

## Links

- Website: **https://rxdsec.tech**
- REX agent: **https://github.com/rxdsec634/REX**

## License

See [LICENSE](LICENSE). The published builds are free to download and use; the source is not
distributed in this repository.
