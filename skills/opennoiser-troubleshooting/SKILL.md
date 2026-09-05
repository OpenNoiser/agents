---
name: opennoiser-troubleshooting
description: Troubleshoot missing microphone audio, speaker echo, device fallback and inactive noise suppression using OpenNoiser's published guides.
license: MIT
metadata:
  author: OpenNoiser
  version: "1.0.0"
---

# opennoiser-troubleshooting

## When to use

Use for OpenNoiser audio-routing, echo, microphone selection or license-state troubleshooting.

## Workflow

1. Read https://opennoiser.com/docs/troubleshooting.md, or use search_docs and get_document at https://opennoiser.com/mcp/docs.
2. Ask for the observed symptom, macOS version, calling app and input/output device types only as needed. Do not request recordings or credentials.
3. For missing audio, check mute, physical input, microphone permission and calling-app input selection.
4. For echo, check playback routing and Auto echo cancellation, then suggest headphones or lower speaker volume.
5. For unexpected device selection, explain Pinned and Tier List behavior.
6. For inactive suppression, check the trial/license state and connectivity for product activation. Do not bypass licensing.
7. If unresolved, direct the user to https://opennoiser.com/contact. Diagnostic sharing is optional and must be reviewed by the user.

## Boundaries

These tools retrieve public guidance only. Never claim a local device was examined or changed. Never execute a destructive command, send diagnostics, reveal a license key or send an email without the user's explicit request.
