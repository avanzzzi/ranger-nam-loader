# Ranger NAM Loader

A simple, fast NAM loader plugin. Inspired by [ranger](https://github.com/ranger/ranger) and vim. Keyboard-driven, optimized for performance.

Built with [JUCE](https://juce.com/), [NeuralAmpModelerCore](https://github.com/sdatkinson/NeuralAmpModelerCore), [FFTConvolver](https://github.com/HiFi-LoFi/FFTConvolver), and CMake. Available as VST3 (Windows, Linux) and LV2 (Linux).

https://github.com/user-attachments/assets/146d01d8-ede9-408f-83ae-f58c652ecf14

## Features

- Ranger-style keyboard-driven file browser for fast NAM and IR browsing
- Two serial NAM slots (A → B) for stacking amp models
- Two parallel IR slots (A + B) with crossfade mix for cabinet blending
- Per-slot input/output gain controls
- NAM and IR output normalization

## Downloads

Check the [Releases](../../releases) page for pre-built VST3 binaries for Windows, Linux and MacOS.

## Controls

| Key       | Action                            |
|-----------|-----------------------------------|
| ↑ / ↓     | Navigate file list                |
| → / Enter | Enter directory / Load file       |
| ←         | Go to parent directory            |
| Enter     | Load selected NAM or IR           |
| Tab       | Cycle panel: NAM A → B → IR A → B |
| Space     | Toggle active slot on/off         |

## Advanced Shortcuts

| Key | Action |
|-----|--------|
| 1 2 3 4 | Switch to NAM A, NAM B, IR A, IR B |
| h | Toggle IR mix between A and B |
| n | Load next file in browser |
| p | Load previous file in browser |
| pgup | Go to the first file in browser |
| pgdn | Go to the last file in browser |