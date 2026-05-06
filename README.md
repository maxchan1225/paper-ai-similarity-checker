# Open Academic Index Originality and AI Screening

A Firebase Hosting single-page app for uploading a paper, searching free public academic indexes, and producing an originality and AI-writing likelihood screening report.

## Important Scope

This app runs in the browser and does not connect to Turnitin, iThenticate, commercial journal databases, student-paper repositories, or proprietary AI detectors. It queries public academic indexes such as Crossref, Semantic Scholar, and arXiv without requiring a commercial API key.

Because the app uses no paid credentials, public services may rate-limit requests. Similarity results are based on public titles, abstracts, metadata, and available descriptions rather than commercial full-text repositories.

Exact DOI or title matches are treated as bibliographic record matches, not as 100% full-text similarity. Scores are capped when only title or metadata evidence is available.

## Features

- Upload `.txt`, `.pdf`, and `.docx` files for the paper.
- Extract DOI, title, and keywords from the submitted paper.
- Search Crossref, Semantic Scholar, and arXiv public indexes.
- Estimate public-index similarity from title overlap, abstract overlap, and phrase overlap.
- Show public source ranking, highest suspicious source, likely matching sentences, index status, and report links.
- Estimate AI-writing likelihood from sentence uniformity, lexical variety, transition patterns, hedging, citation support, and punctuation rhythm.
- Download a structured public-index originality and AI screening report.

## Deploy

```powershell
npx.cmd -y firebase-tools@latest deploy --only hosting --project teacherstudy-ac70b
```
