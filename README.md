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

## What It Does

- Loads an audio file locally in the browser
- Shows basic safety checks such as peak, loudness, clipping risk, muddiness, harshness, stereo balance, mono risk, and silence
- Marks sections that should be listened to again
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

## Browser Support

Use a current version of Chrome or Edge. Other modern browsers may work, but audio format support can vary.

WAV and common MP3 files are the safest input formats.

## GitHub Pages

This project can be served directly with GitHub Pages because it is a static HTML app.

After enabling Pages, open the published URL and use the app in the browser.

