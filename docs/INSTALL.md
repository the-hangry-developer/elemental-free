# Installation Guide

## Windows

1. Download the `.msi` installer
2. Run it. Windows SmartScreen may block it — click "More info" then "Run anyway"

## macOS

1. Download the `.pkg`
2. **First launch**: Right-click the app → "Open". Gatekeeper will warn you. Click "Open" again.
3. If that fails: `System Settings → Privacy & Security → Security → Allow anyway`

## Linux (Wayland)

1. Download the `.deb`
2. Run:

```bash
sudo apt update
sudo apt install libwayland-cursor0 libwayland-client0 libvulkan1 libxkbcommon0
sudo apt install elemental-free-Linux.deb
```

### Dependencies
- `libwayland-cursor` `libwayland-client` `libvulkan1` `libxkbcommon` `libvulkan1`
- Wayland compositor
