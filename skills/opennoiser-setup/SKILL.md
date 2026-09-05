---
name: opennoiser-setup
description: Check OpenNoiser compatibility and help configure its local virtual microphone for Zoom, Discord, Teams or recording on macOS.
license: MIT
metadata:
  author: OpenNoiser
  version: "1.0.0"
---

# opennoiser-setup

## When to use

Use when someone is setting up OpenNoiser or asks whether their Mac is compatible.

## Workflow

1. Read https://opennoiser.com/docs/setup.md. Require Apple Silicon and macOS 14 or later. Do not assume the operating system or processor.
2. Use the build_setup_checklist tool at https://opennoiser.com/mcp, or GET /api/agent/setup with the user-supplied os, architecture, macos_major and output. These are anonymous read-only interfaces.
3. Explain installation and microphone permission steps. Let the user perform installation and permission decisions.
4. Select the physical microphone in OpenNoiser and the OpenNoiser virtual microphone in the calling app; ordinary speakers or headphones remain the playback output.
5. Suggest the local voice test and Echo Cancellation on Auto.

## Boundaries

Do not claim to have inspected or configured the Mac. Do not collect audio, license keys or sign-in codes. No server tool installs software, grants permissions or starts a trial. The trial starts in the macOS app; website downloads require separate email verification.

Cite the setup guide and https://opennoiser.com/auth.md.
