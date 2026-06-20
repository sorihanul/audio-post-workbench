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
3. Check the analysis cards and the marked timeline sections.
4. Pick a goal such as `Auto`, `Vocal clarity`, or `Clean low end`.
5. Click the processing button.
6. Compare the original and processed audio before saving.
7. Export WAV only if the processed version is actually better.

## Usage Guidelines

- Keep the first pass conservative. This tool is meant to reduce obvious risks, not to radically remake a mix.
- Listen to the marked risky sections with headphones or reliable speakers before trusting the result.
- If the processed version sounds smaller, duller, distorted, or tiring, keep the original or try a lighter goal.
- Do not stack many exports on top of each other. Re-processing an already processed file can make artifacts worse.
- Keep a copy of the original file. The exported WAV is a new file, but it should not become your only source.
- For important releases, treat this as a quick helper and still check the result in your normal listening environment.

## What It Does

- Loads an audio file locally in the browser
- Shows basic safety checks such as peak, loudness, clipping risk, muddiness, harshness, high-frequency note tails, stereo balance, mono risk, and silence
- Checks small-speaker risk from stereo/phase behavior
- Marks sections that should be listened to again
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
