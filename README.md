# MEMO Desktop Assistant (memo-da) — Release v0.0.1

Official distribution release of **MEMO Desktop Assistant**, powered by MEMOROUTER.

## 🚀 Downloads

| Asset | Description |
|---|---|
| [📦 MEMO-Desktop-Assistant-Setup-v0.0.1.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.1/MEMO-Desktop-Assistant-Setup-v0.0.1.exe) | Windows Inno Setup Full Installer |
| [⚡ MEMO-Desktop-Assistant-v0.0.1.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.1/MEMO-Desktop-Assistant-v0.0.1.exe) | Windows Portable Executable (No installation required) |
| [🤖 memo-da.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.1/memo-da.exe) | Standalone Binary for MEMO Desktop Add-on execution |
| [🔐 AIBrainDevCert.crt](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.1/AIBrainDevCert.crt) | Code Signing Certificate |
| [📜 install-cert.bat](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.1/install-cert.bat) | Certificate Installer Script |

---

## 📝 Release Notes
<!-- lang:en -->
**Summary:** Initial alpha release of MEMO Desktop Assistant (memo-da) v0.0.1-alpha.
**Highlights:**
- Interactive desktop companion fully integrated with MEMOROUTER agent endpoints.
- Inno Setup modern Windows installer with multilingual support, automatic Defender exclusions, and persistent data management.
- Standalone portable executable and modular add-on support for MEMO Desktop ecosystem.
- Clean development certificate code signing for Windows SmartScreen compliance.
<!-- lang:pt -->
**Resumo:** Lançamento da versão alpha inicial do MEMO Desktop Assistant (memo-da) v0.0.1-alpha.
**Destaques:**
- Assistente virtual interativo para desktop totalmente integrado com os endpoints e agentes da MEMOROUTER.
- Instalador Windows Inno Setup moderno com suporte multi-idiomas, exclusões automáticas no Defender e gerenciamento de dados persistentes.
- Executável portable standalone e suporte modular para distribuição e auto-execução via add-on no MEMO Desktop.
- Assinatura digital com certificado de desenvolvimento compatível com o Windows SmartScreen.

---

## 🛡️ Windows SmartScreen Installation Guide

Because this application uses a self-signed development certificate:
1. Download `AIBrainDevCert.crt` and `install-cert.bat` into the same folder.
2. Right-click `install-cert.bat` and select **"Run as Administrator"**.
3. Run the installer or portable `.exe` directly without any security warnings.
