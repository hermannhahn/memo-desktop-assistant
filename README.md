# MEMO Desktop Assistant (memo-da) — Release v0.0.3

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
| [📦 MEMO-Desktop-Assistant-Setup-v0.0.3.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.3/MEMO-Desktop-Assistant-Setup-v0.0.3.exe) | Windows Inno Setup Full Installer |
| [⚡ MEMO-Desktop-Assistant-v0.0.3.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.3/MEMO-Desktop-Assistant-v0.0.3.exe) | Windows Portable Executable (No installation required) |
| [🤖 memo-da.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.3/memo-da.exe) | Standalone Binary for MEMO Desktop Add-on execution |
| [📜 install.ps1](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.3/install.ps1) | PowerShell One-Line Web Installer |
| [📜 install.cmd](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.3/install.cmd) | CMD / curl One-Line Web Installer |
| [🔐 memo-certificate.crt](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.3/memo-certificate.crt) | Code Signing Certificate |
| [📜 install-cert.bat](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.3/install-cert.bat) | Certificate Installer Script |

---

## 📝 Release Notes
<!-- lang:en -->
**Summary:** Update feed redirection, installer terminal decoupling, and certificate standardization.
**Highlights:**
- Redirected internal update checker from upstream to official repository `hermannhahn/memo-desktop-assistant`.
- Decoupled application post-install launch from shell console handles using `runasoriginaluser` in Inno Setup to prevent terminal hanging.
- Standardized code signing certificate naming to `memo-certificate.crt` across CLI, web installers (`install.ps1`, `install.cmd`), and batch helpers.
- Updated documentation and tasks reflecting certificate architecture and distribution channels.
<!-- lang:pt -->
**Resumo:** Redirecionamento de updates para o repositório oficial, desvinculação de terminal no instalador e padronização do certificado.
**Destaques:**
- Redirecionada a verificação interna de atualizações para o repositório oficial `hermannhahn/memo-desktop-assistant`.
- Desvinculada a execução pós-instalação dos handles de console do terminal via flag `runasoriginaluser` no Inno Setup.
- Padronizado o nome do certificado digital para `memo-certificate.crt` na CLI, instaladores web (`install.ps1`, `install.cmd`) e scripts auxiliares.
- Atualizada a documentação técnica e tarefas refletindo a nova arquitetura do certificado e canais de distribuição.

---

## 🛡️ Manual SmartScreen Installation Guide

If installing manually instead of using the one-line commands above:
1. Download `memo-certificate.crt` and `install-cert.bat` into the same folder.
2. Right-click `install-cert.bat` and select **"Run as Administrator"**.
3. Run the installer or portable `.exe` directly without any security warnings.
