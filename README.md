# Audio Post Workbench

No-install beginner audio post-processing workbench.

Audio Post Workbench runs in a modern browser, analyzes a local audio file, marks risky sections, applies conservative correction, lets you compare original vs processed audio, and exports a WAV file.

## Use

Open `index.html` in Chrome or Edge.

On Windows, you can also double-click:

```text
RUN_AUDIO_WORKBENCH.bat
```

No server, Python, Node.js, account, API key, or internet connection is required when using the downloaded files.

## Quick Guide

1. Open the app.
2. Choose an audio file.
3. Run the automatic check on the Main tab.
4. Use `Auto-select suspect section`.
5. Process and save from the same Main tab workflow.
6. Open Settings, Section Check, Result, Compare, or Explanation only when needed.

## Usage Guidelines

- Keep the first pass conservative. This tool is meant to reduce obvious risks, not to radically remake a mix.
- Listen to the marked risky sections with headphones or reliable speakers before trusting the result.
- If the processed version sounds smaller, duller, distorted, or tiring, keep the original or try a lighter goal.
- Do not stack many exports on top of each other. Re-processing an already processed file can make artifacts worse.
- Keep a copy of the original file. The exported WAV is a new file, but it should not become your only source.
- For important releases, treat this as a quick helper and still check the result in your normal listening environment.

## What It Does

- Loads an audio file locally in the browser
- Splits the app into Main, Settings, Section Check, Result, Compare, and Explanation tabs
- Shows basic safety checks such as peak, loudness, clipping risk, muddiness, harshness, high-frequency note tails, stereo balance, mono risk, and silence
- Checks small-speaker risk from stereo/phase behavior
- Marks sections that should be listened to again
- Can auto-stop playback at the end of a selected section
- Keeps suspect-section selection, processing, and saving in one quick workflow panel
- Shows precise timestamps for short high-frequency spike candidates
- Marks sections that may lose power on small speakers
- Lets you apply safe section-only fixes:
  - emergency fix for a loud section
  - soften a tiring section
  - soften a harsh high-frequency note tail
  - reset the section fix
  - automatic smoothing before and after the section
- Applies conservative correction presets
- Offers beginner-friendly goals:
  - Auto
  - Vocal clarity
  - Clean low end
  - Softer highs
  - Safer separation
- Compares original and processed audio
- Explains the original and processed sound in plain language from local analysis values
- Exports the processed result as WAV

## Privacy

Audio files are processed locally in your browser. They are not uploaded by this app.

## Boundary

This is not a professional mixing or mastering studio. It is a beginner helper for safer post-processing and quick A/B comparison.

It does not perform AI stem separation, vocal isolation, or professional mastering.

The analysis values are practical hints, not final truth. Your ears and the target platform still matter.

## Browser Support

Use a current version of Chrome or Edge. Other modern browsers may work, but audio format support can vary.

WAV and common MP3 files are the safest input formats.

## GitHub Pages

This project can be served directly with GitHub Pages because it is a static HTML app.

After enabling Pages, open the published URL and use the app in the browser.

Recommended Pages setting:

```text
Source: Deploy from a branch
Branch: main
Folder: / (root)
```
