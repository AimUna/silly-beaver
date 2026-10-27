# Silly Beaver V0.3

This diagnostic version separates:
1. microphone permission/input
2. browser speech-to-text support

## Update GitHub Pages
Replace your existing `index.html` with this one and commit the change.

## What the results mean
- Green audio bar moves, but transcription fails:
  microphone is fine; browser speech recognition is the problem.
- Green bar does not move:
  microphone permission/input issue.
- `not-allowed`:
  permission issue.
- `network` or `service-not-allowed`:
  browser speech service issue.

This file is intentionally diagnostic-only so we can isolate the problem cleanly.
