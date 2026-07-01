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
5. Create a processed version from the Main tab.
6. Open the Result tab, read the save decision flow, and start the final listening check.
7. In the final check, choose one result for each segment: processed is OK, uncomfortable, or original is better.
8. Save only when the app shows a save candidate or final pass.

## Optional Genre Workflow

If you want a style-specific pass, open the Genre tab after loading a file.

1. Choose a genre such as vocal ballad, rock/band, acoustic, dance/EDM, or hip-hop/R&B.
2. Keep `pre-clean first` enabled for a first pass from the original file.
3. Start with the normal strength, then try genre emphasis only when the result still feels too dull or buried.
4. Avoid repeatedly processing an already processed export.

## Save Decision Flow

The difference may sound subtle on ordinary headphones or speakers. This tool is meant to reduce risk, not make a dramatic mastering change.

1. First check the waveform and numbers for peak safety, clipping risk, muddiness, tiring highs, and obvious regressions.
2. Then listen to the same short section in original and processed form.
3. Judge whether the processed version is uncomfortable, not whether it sounds dramatically better.
4. If the final check marks discomfort or original-is-better, do not save. Try a lighter pass or keep the original.

## Usage Guidelines

- Keep the first pass conservative. This tool is meant to reduce obvious risks, not to radically remake a mix.
- Check the marked risky sections visually first, then listen on the equipment you have.
- The difference between original and processed audio may be subtle on ordinary playback gear. Use the waveform and save decision flow together.
- If the processed version sounds smaller, duller, distorted, or tiring, keep the original or try a lighter goal.
- Do not stack many exports on top of each other. Re-processing an already processed file can make artifacts worse.
- Keep a copy of the original file. The exported WAV is a new file, but it should not become your only source.
- For important releases, treat this as a quick helper and still check the result in your normal listening environment.

## What It Does

- Loads an audio file locally in the browser
- Splits the app into Main, Settings, Section Check, Result, Compare, Genre, Sound Character, and Explanation tabs
- Shows basic safety checks such as peak, loudness, clipping risk, muddiness, tiring highs, high-frequency note tails, stereo balance, mono risk, and silence
- Checks small-speaker risk from stereo/phase behavior
- Marks sections to review directly on the waveform
- Starts with broad regions, with detailed sections expandable only when needed
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
- Offers a separate genre-processing path with an optional pre-clean pass
- Offers beginner-friendly goals:
  - Auto
  - Vocal clarity
  - Reduce muddiness
  - Softer highs
  - Reduce smeared reverb
  - Safer separation
- Compares original and processed audio
- Shows beginner-readable sound-character hints such as space, center, low-end weight, muddiness, high fatigue, and energy movement
- Provides a final listening check before saving
- Prevents accidental saving after a final-check hold result
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
