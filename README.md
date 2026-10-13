# MEMO Desktop Assistant (memo-da) — Release v0.0.4

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
| [📦 MEMO-Desktop-Assistant-Setup-v0.0.4.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.4/MEMO-Desktop-Assistant-Setup-v0.0.4.exe) | Windows Inno Setup Full Installer |
| [⚡ MEMO-Desktop-Assistant-v0.0.4.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.4/MEMO-Desktop-Assistant-v0.0.4.exe) | Windows Portable Executable (No installation required) |
| [🤖 memo-da.exe](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.4/memo-da.exe) | Standalone Binary for MEMO Desktop Add-on execution |
| [📜 install.ps1](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.4/install.ps1) | PowerShell One-Line Web Installer |
| [📜 install.cmd](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.4/install.cmd) | CMD / curl One-Line Web Installer |
| [🔐 memo-certificate.crt](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.4/memo-certificate.crt) | Code Signing Certificate |
| [📜 install-cert.bat](https://github.com/hermannhahn/memo-desktop-assistant/releases/download/v0.0.4/install-cert.bat) | Certificate Installer Script |

---

## 📝 Release Notes
<!-- lang:en -->
**Summary:** Client-side prompt injection cleanup and character settings simplification.
**Highlights:**
- Removed hardcoded mascot system instructions and persona prompt injections from `/v1/responses`, ensuring clean delegation to server-side MEMOROUTER agent personas.
- Streamlined Character settings tab: retained speech bubble positioning coordinates (Bubble left, top, width) and desktop motion settings; removed name, personality, director summary, and memory/continuation editors.
- Removed "Add a character" card and legacy avatar generation/import flows.
- Updated unit and integration tests to align with the streamlined interface layout.
<!-- lang:pt -->
**Resumo:** Remoção de injeções de prompt no cliente e simplificação das configurações de personagens.
**Destaques:**
- Removidas instruções hardcoded de mascote e injeção de persona do cliente na API `/v1/responses`, garantindo delegação limpa às personas dos agentes configurados no MEMOROUTER.
- Simplificada a aba de configurações de Personagem: mantidas as coordenadas de posicionamento dos balões de fala (Bubble left, top, width) e movimento; removidos campos de persona, resumo do Character Director e editores de memória/continuação.
- Removido o card "Add a character" e fluxos legados de importação e geração de avatar.
- Atualizados os testes unitários e de integração para validação contínua da nova interface.

---

## 🛡️ Manual SmartScreen Installation Guide

If installing manually instead of using the one-line commands above:
1. Download `memo-certificate.crt` and `install-cert.bat` into the same folder.
2. Right-click `install-cert.bat` and select **"Run as Administrator"**.
3. Run the installer or portable `.exe` directly without any security warnings.
