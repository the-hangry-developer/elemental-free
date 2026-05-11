# Elemental

Fast, native, cross-platform 3D asset viewer. Local-only. No cloud. No upload.

Using GPU-accelerated UI, enables browsing and live-preview of glTF, FBX, OBJ files.

---

## Why This Exists

Previewing 3D files on desktop is broken:
- **Blender/Unity/Unreal**: Overkill for a quick look. Slow to launch, slow to import.
- **Web viewers**: Upload your files to someone else's server. Wait for network. Pray for privacy.
- **OS defaults**: Windows 3D Viewer is basic and Windows-only. macOS Preview doesn't do 3D. Linux? Good luck.

This is a native desktop app that opens your files locally, immediately, with GPU-accelerated rendering.

---

## Download

| Platform                  | Version | Download    | Size   |
|---------------------------|---------|-------------|--------|
| Windows 10+               | v0.1.0  | [msi](link) | ~46 MB |
| macOS 15+ (Apple Silicon) | v0.1.0  | [pkg](link) | ~18 MB |
| Linux (Wayland)           | v0.1.0  | [deb](link) | ~20 MB |

### ⚠️ Security Notice

Binaries are currently **unsigned**. Your OS will show a security warning on first launch. This is normal for independent software.

- **Windows**: Click "More info" → "Run anyway"  
- **macOS**: Right-click the app → "Open" (do this twice if needed)  
- **Linux**: deb files need root privilege to install. See [INSTALL.md](docs/INSTALL.md).

[Verify checksums](docs/CHECKSUMS.md) | [VirusTotal scan](link)

---

## Features

### Free Viewer
- **Live preview**: Click any imported glTF/glb, FBX, or OBJ model.
- **GPU-accelerated**: Smooth orbit, zoom & pan. Metal on macOS, D3D11/12 on Windows, Vulkan on Linux (Wayland).
- **Cross-platform**: Native Windows, macOS, and Linux (Wayland) builds
- **Local-only**: Your files never leave your machine. Nothing is uploaded.
- **Format inspection**: View mesh stats, material info, texture references.

### Pro ($15, one-time) - coming soon...

---

## System Requirements

- **OS**: Windows 10+, macOS 15+, or Linux with Wayland
- **GPU**: Vulkan 1.1+, Metal, or DirectX 11/12 compatible
- **RAM**: 4 GB minimum, 8 GB recommended
- **Storage**: 200 MB for the app

---

## Screenshots

[Main viewer interface](screenshots/viewer.png)  
[Project browser (Pro)](screenshots/project.png)  
[Material inspection panel](screenshots/inspect.png)

---

## Roadmap

- [x] glTF
- [x] FBX
- [x] OBJ/MTL
- [/] USD (in progress)
- [ ] Batch/mass operations
- [ ] Animation
- [ ] More file formats

---

## Support

- **Bug reports & feature requests**: [Open an issue](../../issues)
- **Pro support**: [the.hangry.developer@gmail.com](mailto:the.hangry.developer@gmail.com)
- **Refund policy**: 7-day no-questions refund via Gumroad

---

## License

Proprietary. All rights reserved.  
See [LICENSE](LICENSE) for details.

---

## Built With

- C++23
- Skia (GPU-accelerated UI)

**Not Electron. Not a web app. Native code.**
