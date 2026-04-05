# Ranger NAM Loader

A simple, fast NAM loader plugin. Inspired by [ranger](https://github.com/ranger/ranger) and vim. Keyboard-driven, optimized for performance.

Built with [JUCE](https://juce.com/), [NeuralAmpModelerCore](https://github.com/sdatkinson/NeuralAmpModelerCore), [FFTConvolver](https://github.com/HiFi-LoFi/FFTConvolver), and CMake. Available as VST3 (Windows, Linux) and LV2 (Linux).

<img width="996" height="925" alt="Image" src="https://github.com/user-attachments/assets/3971e679-b242-4da0-9301-5f4ee19b7659" />

https://github.com/user-attachments/assets/ce79e359-73d3-4207-99d5-369920ee91d1

## Features

- Ranger-style keyboard-driven file browser for fast NAM and IR browsing
- Two serial NAM slots (A → B) for stacking amp models
- Two parallel IR slots (A + B) with crossfade mix for cabinet blending
- Per-slot input/output gain controls
- NAM and IR output normalization

## Downloads

Check the [Releases](../../releases) page for pre-built VST3 binaries for Windows and Linux.
MacOS builds coming soon.

## Controls

| Key       | Action                          |
|-----------|---------------------------------|
| ↑ / ↓     | Navigate file list              |
| → / Enter | Enter directory / Load file     |
| ←         | Go to parent directory          |
| Enter     | Load selected NAM or IR         |
| Tab       | Cycle panel: NAM A → B → IR A → B |
