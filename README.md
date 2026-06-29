# Photoshop Scripts

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Photoshop](https://img.shields.io/badge/Photoshop-2023+-ff00ff)
![Status](https://img.shields.io/badge/status-active-success)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow)

Professional collection of JSX/ExtendScript automation scripts for Adobe Photoshop. Engineered for retouchers, photographers, and designers who require precision automation and workflow optimization.

[![Skills](https://skillicons.dev/icons?i=js,ps&theme=dark&perline=2)](https://skillicons.dev)

---

## Contents

- [Overview](#overview)
- [Scripts](#scripts)
- [Installation](#installation)
- [Usage](#usage)
- [Technical Specifications](#technical-specifications)
- [License](#license)
- [Support](#support)

---

## Overview

Minimum viable collection of production-grade automation tools for Adobe Photoshop. Non-destructive, batch-capable, cross-platform compatible.

### Capabilities

- Production-ready implementation
- Non-destructive operations
- Batch processing at scale
- Cross-platform support (macOS, Windows)
- Extensive version compatibility

---

## Scripts

| Script | Description | Application | Minimum Version |
|--------|-------------|-------------|-----------------|
| Smart Path Crop | Batch crop to clipping path with standard canvas extension | Product photography | CS6+ |
| Layer Cleanup | Automated removal of empty and invisible layers | Document optimization | CC 2020+ |
| PathTransfer | Transfer clipping paths between file formats by filename | Workflow automation | CS6+ |
| DocInfo Engine | Embed document technical specifications as text layer | Metadata documentation | CC 2020+ |
| Document Info Extractor v2 | Advanced version with proportional text overlay | Professional documentation | CC 2022+ |
| Stack in PSD | Reverse layer hierarchy and export to PSD format | Mass processing | CS6+ |

---

## Installation

### macOS

```bash
git clone https://github.com/TheMaestr-o/Photoshop-Scripts.git
cp -r *.jsx ~/Library/Application\ Support/Adobe/Adobe\ Photoshop\ [VERSION]/Presets/Scripts/
```

Paths by version:
- Photoshop 2025: `~/Library/Application Support/Adobe/Adobe Photoshop 2025/Presets/Scripts/`
- Photoshop 2024: `~/Library/Application Support/Adobe/Adobe Photoshop 2024/Presets/Scripts/`
- Photoshop 2023: `~/Library/Application Support/Adobe/Adobe Photoshop 2023/Presets/Scripts/`

### Windows

```bash
git clone https://github.com/TheMaestr-o/Photoshop-Scripts.git
copy *.jsx "C:\Program Files\Adobe\Adobe Photoshop [VERSION]\Presets\Scripts\"
```

Paths by version:
- Photoshop 2025: `C:\Program Files\Adobe\Adobe Photoshop 2025\Presets\Scripts\`
- Photoshop 2024: `C:\Program Files\Adobe\Adobe Photoshop 2024\Presets\Scripts\`

### Quick Setup

1. Download script files
2. Open Photoshop
3. File → Scripts → Browse
4. Select script
5. Execute

---

## Usage

### Method 1: Photoshop Menu

```
File → Scripts → Other Scripts → [Script Name]
```

### Method 2: Scripts Panel

1. Window → Scripts
2. Locate script
3. Double-click

### Method 3: ExtendScript Console

```javascript
#include "/path/to/script.jsx"
main();
```

---

## Technical Specifications

### System Requirements

| Component | Specification |
|-----------|---------------|
| Operating System | macOS 10.14+ / Windows 10+ |
| Photoshop | CC 2020+ (CS6+ for most scripts) |
| Runtime | ExtendScript (included with Photoshop) |
| Dependencies | None |

### Compatibility Matrix

| Script | CS6 | CC 2015 | CC 2020 | CC 2024 | CC 2025 |
|--------|-----|--------|--------|---------|---------|
| Smart Path Crop | ✓ | ✓ | ✓ | ✓ | ✓ |
| Layer Cleanup | ✓ | ✓ | ✓ | ✓ | ✓ |
| PathTransfer | ✓ | ✓ | ✓ | ✓ | ✓ |
| DocInfo Engine | — | ⚠ | ✓ | ✓ | ✓ |
| Document Info v2 | — | — | ⚠ | ✓ | ✓ |
| Stack in PSD | ✓ | ✓ | ✓ | ✓ | ✓ |

---

## FAQ

**Q: Script not appearing in Photoshop menu**

A: Verify installation path for your Photoshop version. Restart Photoshop. Confirm .jsx file extension.

**Q: DocInfo Engine missing extension**

A: Rename to "DocInfo Engine.jsx" manually.

**Q: Batch processing multiple files**

A: Use File → Automate → Batch or execute manually per file.

**Q: Performance optimization**

A: Standard for batch operations. Optimize image dimensions. Close unnecessary applications.

---

## Resources

- Adobe ExtendScript: https://github.com/Adobe-CEP/CEP-Resources
- Photoshop Scripting: https://www.adobe.io/apis/creativecloud/photoshop.html
- ExtendScript Toolkit: https://www.adobe.com/products/extendscript.html
- Adobe Community: https://forums.adobe.com/community/en/groups/adobe-dev

---

## License

MIT License. Free for personal and commercial use.

See LICENSE file for full details.

---

## Support

Email: gssdarm@gmail.com
Telegram: [@ohnedan](https://t.me/ohnedan)
GitHub: [@TheMaestr-o](https://github.com/TheMaestr-o)

---

Last updated: June 2026
