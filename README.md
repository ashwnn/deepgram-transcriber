# Deepgram MP3 Transcriber

A serverless MP3 transcription tool powered by Next.js and the Deepgram API. Runs entirely in your browser with no backend required.

## Features

- Serverless architecture: direct browser fetch to Deepgram API, no middleman server
- Minimalist UI
- Audio Intelligence: Summarization, Topics, Intents, Entity Detection, Sentiment Analysis
- Transcription options: Diarization, Smart Format, Punctuation, Utterances, Redaction, and more
- Export transcription results as Markdown
- Supports files up to 100MB via chunked streaming

## Tech Stack

- Next.js 15 (static export)
- TypeScript
- Tailwind CSS

## Getting Started

Install dependencies:

```bash
bun install
```

Run locally:

```bash
bun run dev
```

Open [http://localhost:3000](http://localhost:3000). No `.env` file needed. Enter your Deepgram API key directly in the UI.

## GitHub Pages Deployment

Build and deploy to the `gh-pages` branch:

```bash
bun run deploy
```

Then go to your repo's Settings > Pages and set the source branch to `gh-pages`.

## License

[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/)

> NOTE: AI tools (Kimi 2.5 and GPT-5.3 Codex) were used to assist with implementation.
