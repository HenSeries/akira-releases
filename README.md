# Akira — releases

Downloads for **Akira**, a local-first software architect that runs on your own machine with
[Ollama](https://ollama.com) models.

This repository holds only release notes and built desktop bundles. The source code is
private, so there is no code, issue tracker or pull requests here.

## Download

Open the [latest release](../../releases/latest) and pick a bundle:

| File | For |
| --- | --- |
| `Akira_<version>_amd64.AppImage` | Any x86-64 Linux distribution (`chmod +x`, then run it) |
| `Akira_<version>_amd64.deb` | Debian, Ubuntu and derivatives (`sudo apt install ./Akira_*.deb`) |
| `Akira-<version>-1.x86_64.rpm` | Fedora, openSUSE and derivatives (`sudo dnf install ./Akira-*.rpm`) |
| `SHA256SUMS` | Checksums of every file in the release |

Check a download before installing it:

```bash
sha256sum -c SHA256SUMS --ignore-missing
```

## Requirements

- x86-64 Linux with WebKitGTK 4.1 (the AppImage bundles it).
- Ollama running locally.
- The Akira backend (a Python venv). The desktop app starts it from the folder named by
  `AKIRA_HOME`. The backend is not distributed here yet.

## Versions

Releases follow [semantic versioning](https://semver.org); tags are `vMAJOR.MINOR.PATCH`.
Pre-releases are marked as such on the releases page.
