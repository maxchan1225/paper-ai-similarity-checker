# Paper AI Similarity Checker

A Firebase Hosting single-page app for uploading or pasting a paper and producing an estimated similarity score and AI-writing likelihood.

## Important Scope

This app runs in the browser and does not connect to a commercial plagiarism database or a proprietary AI detector. It is intended as a first-pass screening tool for teaching and review workflows.

## Features

- Upload `.txt`, `.pdf`, and `.docx` files.
- Paste manuscript text and optional reference text for local comparison.
- Estimate similarity risk from internal repetition, reference overlap, citation density, and phrase reuse.
- Estimate AI-writing likelihood from sentence uniformity, transition patterns, lexical variety, hedging, and punctuation rhythm.
- Show highlighted repeated phrases, risk explanations, and a downloadable text report.

## Deploy

```powershell
npx.cmd -y firebase-tools@latest deploy --only hosting --project teacherstudy-ac70b
```
