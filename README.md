# Alloy Code — Releases

Signed release binaries for **Alloy Code** (closed-source). This repository hosts artifacts only — no source code.

## Install

**Windows (PowerShell):**

    irm https://atlasbrain.cloud/install.ps1 | iex

**macOS / Linux:**

    curl -fsSL https://atlasbrain.cloud/install | sh

Then sign in:

    alloy login

## Verifying a release

Every release ships a `SHA256SUMS` manifest signed with an offline ed25519 key (`SHA256SUMS.sig`). The install scripts verify SHA-256 automatically. To verify the signature end-to-end, check `SHA256SUMS.sig` against the published `release-signing.pub`.
