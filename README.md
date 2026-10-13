# MEMO Desktop Assistant (memo-da) — Release v0.0.2

Official distribution release of **MEMO Desktop Assistant**, powered by MEMOROUTER.

## ⚡ Quick One-Line Web Installation (Recommended)

Automatically registers the development certificate and launches the setup wizard without any Windows SmartScreen warnings:

### PowerShell (Standard or Administrator prompt):
```powershell
irm https://raw.githubusercontent.com/hermannhahn/memo-desktop-assistant/main/install.ps1 | iex
```

### Command Prompt / CMD (via curl):
```cmd
curl -fsSL https://raw.githubusercontent.com/hermannhahn/memo-desktop-assistant/main/install.cmd -o install.cmd && install.cmd && del install.cmd
```

---

## 🚀 Downloads

| Asset | Description |
|---|---|
| [📦 MEMO-Desktop-Assistant-Setup-v0.0.2.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.2/MEMO-Desktop-Assistant-Setup-v0.0.2.exe) | Windows Inno Setup Full Installer |
| [⚡ MEMO-Desktop-Assistant-v0.0.2.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.2/MEMO-Desktop-Assistant-v0.0.2.exe) | Windows Portable Executable (No installation required) |
| [🤖 memo-da.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.2/memo-da.exe) | Standalone Binary for MEMO Desktop Add-on execution |
| [📜 install.ps1](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.2/install.ps1) | PowerShell One-Line Web Installer |
| [📜 install.cmd](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.2/install.cmd) | CMD / curl One-Line Web Installer |
| [🔐 AIBrainDevCert.crt](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.2/AIBrainDevCert.crt) | Code Signing Certificate |
| [📜 install-cert.bat](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.2/install-cert.bat) | Certificate Installer Script |

---

## 📝 Release Notes
<!-- lang:en -->
**Summary:** Automated one-line web installers (PowerShell irm and CMD curl) with SmartScreen bypass.
**Highlights:**
- One-line PowerShell web installer (`irm ... | iex`) with automatic elevation and certificate pre-registration.
- One-line Command Prompt web installer (`curl -fsSL ... -o install.cmd && install.cmd && del install.cmd`).
- Automatic registration of code signing certificate into Windows Trusted Root and Trusted Publisher stores.
- Automated Microsoft Defender exclusions for application directory and executable.
- Fully automated synchronization of installer scripts to release assets and repository root in CLI.
<!-- lang:pt -->
**Resumo:** Instaladores web automatizados em uma linha (PowerShell irm e CMD curl) com bypass do SmartScreen.
**Destaques:**
- Instalador em uma linha via PowerShell (`irm ... | iex`) com elevação automática e pré-registro de certificado.
- Instalador em uma linha via Prompt de Comando (`curl -fsSL ... -o install.cmd && install.cmd && del install.cmd`).
- Registro automático do certificado digital nas autoridades confiáveis do Windows (Root e TrustedPublisher).
- Configuração automática de exclusões no Microsoft Defender para a pasta e executável do aplicativo.
- Sincronização automatizada dos scripts de instalação com os assets de release e raiz do repositório na CLI.

---

## 🛡️ Manual SmartScreen Installation Guide

If installing manually instead of using the one-line commands above:
1. Download `AIBrainDevCert.crt` and `install-cert.bat` into the same folder.
2. Right-click `install-cert.bat` and select **"Run as Administrator"**.
3. Run the installer or portable `.exe` directly without any security warnings.
