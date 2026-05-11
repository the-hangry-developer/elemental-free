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

---

## Verifying Downloads

All releases include SHA256 checksums. Verify:

```bash
sha256sum -c checksums.txt
```

[VirusTotal results for the Windows .msi](https://www.virustotal.com/gui/file/0db93d2044e5b4ab08ec2f23b7505ca5832706f2ca8a2b9ebc045d8a0d7bc83a) are available here.
[VirusTotal results for the Linux .msi](https://www.virustotal.com/gui/file/e794265873b14340e51291ccd556b57e6362d6cfd2866e4bc09ce5c6056225d1) are available here.
