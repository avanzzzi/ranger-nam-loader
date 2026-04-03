# Ranger NAM Loader

A dual Neural Amp Model (NAM) loader with dual IR cabinet simulation. Inspired by [ranger](https://github.com/ranger/ranger) and vim — keyboard-driven, optimized for performance.

Built with [JUCE](https://juce.com/), [NeuralAmpModelerCore](https://github.com/sdatkinson/NeuralAmpModelerCore), [FFTConvolver](https://github.com/HiFi-LoFi/FFTConvolver), and CMake. Available as VST3 (Windows, Linux) and LV2 (Linux).

## Features

- Two serial NAM slots (A → B) for stacking amp models
- Two parallel IR slots (A + B) with crossfade mix for cabinet blending
- Per-slot input/output gain controls
- IR mix and IR output controls
- Ranger-style keyboard-driven file browser with independent cursor memory per panel
- NAM file preview with model name, architecture, and output normalization metadata
- IR preview with sample rate, duration, and bit depth
- On/off toggle per slot
- State serialization — full session recall including file paths and browser positions
- .nam and .wav file type filtering per panel

## Signal Chain

```
Input → NAM A → NAM B → (IR A + IR B mixed) → Output
```

Each stage can be independently bypassed. NAM slots process in series, IR slots in parallel with adjustable mix.

## Downloads

Check the [Releases](../../releases) page for pre-built VST3 binaries for Windows and Linux.

## Controls

| Key       | Action                          |
|-----------|---------------------------------|
| ↑ / ↓     | Navigate file list              |
| → / Enter | Enter directory / Load file     |
| ←         | Go to parent directory          |
| Enter     | Load selected NAM or IR         |
| Tab       | Cycle panel: NAM A → B → IR A → B |

## Parameters

| Parameter  | Range          | Description                     |
|------------|----------------|---------------------------------|
| Input A    | -60 to +12 dB  | Gain before NAM A processing    |
| Output A   | -60 to +12 dB  | Gain after NAM A processing     |
| Input B    | -60 to +12 dB  | Gain before NAM B processing    |
| Output B   | -60 to +12 dB  | Gain after NAM B processing     |
| IR Mix     | -1.0 to +1.0   | IR A/B blend (left=A, right=B)  |
| IR Output  | -60 to +12 dB  | Gain after IR mixing            |

## License

MIT
