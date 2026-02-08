# ai.milady.Milaidy

Flatpak manifest for **Milaidy** — a personal AI assistant built on [ElizaOS](https://github.com/elizaos).

## Build locally

```bash
# Install Flatpak build tools
sudo apt install flatpak flatpak-builder

# Install the SDK
flatpak install flathub org.freedesktop.Platform//23.08
flatpak install flathub org.freedesktop.Sdk//23.08

# Build
flatpak-builder --repo=repo --force-clean build-dir ai.milady.Milaidy.yml

# Create a bundle
flatpak build-bundle repo milaidy.flatpak ai.milady.Milaidy

# Install and test
flatpak --user install milaidy.flatpak
flatpak run ai.milady.Milaidy start
```

## Flathub submission

This repo is structured for submission to [Flathub](https://flathub.org).
See the [Flathub submission guide](https://github.com/flathub/flathub/wiki/App-Submission).

## Files

- `ai.milady.Milaidy.yml` — Flatpak build manifest
- `ai.milady.Milaidy.desktop` — Desktop entry for app launchers
- `ai.milady.Milaidy.metainfo.xml` — AppStream metadata

## Links

- [Milaidy](https://github.com/milady-ai/milaidy)
- [milady.ai](https://milady.ai)
