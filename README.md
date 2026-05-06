# Paper Originality and AI Screening Report

A Firebase Hosting single-page app for uploading a main paper plus a local comparison database, then producing an originality report and AI-writing likelihood report.

## Important Scope

This app runs in the browser and does not connect to Turnitin, iThenticate, commercial journal databases, student-paper repositories, or proprietary AI detectors. It is intended as a stronger first-pass screening tool for teaching and review workflows.

To get meaningful similarity results, upload one file as the main paper and upload known sources, peer papers, course materials, or copied web text into the comparison database. A single paper with no comparison sources can only produce internal repetition and writing-pattern signals.

## Features

- Upload `.txt`, `.pdf`, and `.docx` files for the main paper.
- Upload multiple `.txt`, `.pdf`, and `.docx` files as a local comparison database.
- Paste additional source text separated by `---`.
- Estimate overall similarity from document fingerprints and paragraph-level source coverage.
- Show source ranking, highest single-source similarity, matched paragraphs, repeated internal phrases, citation signals, and long-quote risk.
- Estimate AI-writing likelihood from sentence uniformity, lexical variety, transition patterns, hedging, citation support, and punctuation rhythm.
- Download a structured text report similar to an originality and AI screening summary.

## Deploy

```powershell
npx.cmd -y firebase-tools@latest deploy --only hosting --project teacherstudy-ac70b
```
