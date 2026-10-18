# Data Engineer Drill

A mobile-first, offline-capable practice app for the Databricks Data Engineer
Associate certification.

## Product features

- Five-question drills that prioritize unseen questions.
- Module practice aligned to the seven current official exam sections.
- Immediate answer feedback and detailed explanations.
- A mistake list that clears a question after two correct review attempts.
- On-device progress, current-round recovery, and explanation issue reports.
- “Ask ChatGPT” copies a complete English study prompt and opens ChatGPT.
- Knowledge review highlights weak modules using local attempt history.
- Installable web-app behavior and offline caching after the first visit.

The app contains no API key, backend, account, tracking, or cloud persistence.
All progress remains in the browser’s local storage.

## Files

- `index.html` contains the complete product interface and behavior.
- `questions.json` contains the normalized 1,008-question bank.
- `manifest.webmanifest` provides installable app metadata.
- `service-worker.js` caches the app for offline study.
- `og.png` is the English social-preview card.
- `outputs/` contains the canonical question-bank deliverables and audit report.

## Commands

```bash
npm run dev
npm test
npm run build
```

The project has no runtime or build dependencies beyond Node.js.

## Content status

The practice questions and explanations come from a community repository and
remain marked as unverified. Fifteen lineage questions that cannot be reliably
mapped to the current official exam outline remain in the `unknown` module.
