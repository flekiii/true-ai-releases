# TRUE AI — Official Releases

This **public repository contains only official TRUE AI release files**. The application's source code is maintained separately in a private development repository.

## Downloads

Use [GitHub Releases](https://github.com/flekiii/true-ai-releases/releases) for official versions.

Each Linux x86_64 release includes:

- `TRUE-AI-<version>-linux-x64.tar.gz` — portable Linux build and optional installer
- `SHA256SUMS` — integrity checksums
- Release notes (improvements, limitations, and supported platforms)

No release has been published until the Releases page contains a dated version and downloadable assets.

## Verify and use a Linux release

Download the archive and `SHA256SUMS` from the same official release. Then:

```bash
sha256sum -c SHA256SUMS
tar -xzf TRUE-AI-<version>-linux-x64.tar.gz
cd TRUE-AI-<version>-linux-x64
./run.sh
```

Replace `<version>` with the actual version number.

Optional user-local installation:

```bash
bash install.sh
```

The installer keeps old releases for rollback and does **not** delete your chats or settings. No `sudo` is needed. It does not install Ollama or AI models.

## Privacy and updates

- TRUE AI checks this repository only when you request an update check.
- Updates are **not mandatory** and are **never installed automatically**.
- Chat history and local settings stay on the user's computer.
- The checksum detects corruption, but it is not a cryptographic code signature.
- Linux builds require compatible GTK runtime libraries; portability across distributions varies.

This release repository is not intended to host API keys, user data, local models, or the private development source.
