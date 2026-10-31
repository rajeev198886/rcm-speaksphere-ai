# RCM SpeakSphere AI

A React, TypeScript, and Vite demo for the RCM personalized communication practice platform. It includes a syllabus workspace and a read-first, topic-linked voice-coaching module.

## Requirements

- Node.js 20.19+ or 22.12+
- npm

## Run in Windows PowerShell

```powershell
npm install
npm run dev
```

Open the local URL printed by Vite. Create a production build with `npm run build`.

## Demo mode

Dashboard activity and streak values are illustrative sample content, not RCM student or college analytics. Voice practice uses browser speech recognition only after consent, or a typed response; session text stays in page memory and clears on refresh or when you leave. No account, audio recording, backend, live AI feedback, or persistence is connected.

## Current milestone

Current demo: responsive learning space, curriculum source catalog, and a sequenced voice practice module. Student progress and dashboard figures remain illustrative.

## Syllabus workspace

The Curriculum page is a source-traceable demo for the syllabus PDFs in `Assets/Syllabus latest`. It distinguishes readable course catalogs from course-list-only and OCR-required sources and provides syllabus-informed communication task templates. It does not fine-tune an AI model, provide live AI feedback, or claim complete topic coverage. Several supplied PDFs contain only course tables, and scanned/image-encoded PDFs still require OCR and faculty review before every topic can be marked complete.

## Voice coach and discussion practice

The Voice Coach runs a read-first 18-minute daily module: syllabus-linked passage (3 minutes), student-reported reading/confidence check (2 minutes), ten-minute speaking exercise, and a short coach review/follow-up. Prompts can be read aloud with browser text-to-speech. Browser speech recognition is optional and requires consent; typed answers are available. The correction panel uses a small set of visible transcript rules and formatting cues, not a live AI grammar, pronunciation, anxiety, or fluency model. Timer duration does not verify continuous speaking. Camera preview is opt-in and local; video is not analyzed, recorded, or uploaded. Anxiety and reading concerns come only from the student check-in. Group discussion roles are spoken prompts in a solo demo, not live peer connections. Browser speech support/processing varies. No server-side AI, remote peer room, or persistent session storage is connected.

## Feedback and progress history

Typed syllabus reflections return an immediate local coaching report based on response structure, examples, development, and common transcript language cues. Presentation and voice sessions can be saved to the same browser-local progress history. Dashboard summary and recent session rows read from that saved history. These records use localStorage on this browser/device; they are not synced across devices or backed by a student account and can be cleared from the dashboard. The feedback is rule-based coaching, not a connected generative AI model, pronunciation evaluator, or academic grading service. Speech feedback depends on optional browser speech recognition and its transcript quality.

## Login and student registration prototype

The `/login` and `/signup` routes use the supplied SpeakSphere logo. Authentication is explicitly a frontend demo: sign-in accepts a non-empty roll number and an eight-digit DDMMYYYY value to enter the existing dashboard; there is no student registry, backend, password verification, or real account creation. Signup validates required fields and displays a pending verification notice without storing submitted personal data. Optional roll-number remembrance saves only that identifier in localStorage; the date-of-birth password is never saved. Do not use real student credentials until a secure, authorized backend is implemented.
