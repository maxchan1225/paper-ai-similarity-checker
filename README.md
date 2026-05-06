# AI Writing Risk Screener

A Firebase Hosting single-page app for uploading or pasting a paper and producing an AI-writing risk report.

## Scope

This version intentionally does not provide plagiarism or public-index similarity scores. Earlier public-index matching depended on unstable third-party availability and could be misunderstood as a formal originality score.

The app does not connect to Turnitin, iThenticate, commercial databases, or proprietary AI detector models. It estimates AI-writing risk from explainable text features and is intended for screening, revision guidance, and manual review prioritization.

## Features

- Upload `.txt`, `.pdf`, and `.docx` files.
- Estimate AI writing rate from sentence rhythm, lexical diversity, transition patterns, hedging, citation support, data density, method traces, paragraph rhythm, author-process traces, and punctuation rhythm.
- Show confidence level based on text length, sentence count, paragraph count, and citation evidence.
- Rank high-risk paragraphs.
- Provide practical recommendations for lowering AI-risk signals.
- Download a structured AI writing risk report.

## Deploy

```powershell
npx.cmd -y firebase-tools@latest deploy --only hosting --project teacherstudy-ac70b
```
