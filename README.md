# Deepgram MP3 Transcriber 🎙️

A sleek, serverless MP3 transcription suite powered by **Next.js**, **React**, and the **Deepgram API**. 

This application runs **100% in your browser** as a static HTML export. No backend is required, meaning your API Key and audio files are communicated directly from your browser to Deepgram's API securely without any middleman servers.

## Features ✨

*   **Serverless Architecture**: Pure client-side interactions via `fetch` to `api.deepgram.com`. Ready for GitHub Pages hosting out-of-the-box.
*   **Minimalist Brutalist UI**: A beautiful, distraction-free environment allowing easy text review.
*   **Advanced Audio Intelligence Settings**: Get full access to Deepgram's proprietary intelligence tooling natively via a custom UI accordion, avoiding complicated API requests. Included are **Summarization, Topics, Intents, Entities, and Sentiment Analysis**.
*   **Deep Transcription Options**: Select Base and Fine-tuned models, configure **Speaker Diarization**, find and replace keywords, filter profanity, apply redactions, use Smart Formatting, and more.
*   **Batch Markdown Export (.md)**: Transcribe multiple files, view their intelligent metadata, and save perfectly aligned Markdown outputs with a single click.

## Technology Stack 💻

- **Framework**: Next.js 15 (App Router enabled with `output: 'export'`)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Icons**: lucide-react

---

## Getting Started 🚀

### Local Development

1. Clone the repository and install dependencies using `bun` (or `npm`/`yarn`):

```bash
bun install
```

2. Start the development server:

```bash
bun run dev
```

3. Open your browser and navigate to [http://localhost:3000](http://localhost:3000).

*Note: No `.env` variables are required! You will supply your API Key securely in the UI, which will be safely saved into your browser's local storage.*

### Deploying to GitHub Pages 🌍

This project is already pre-configured for **GitHub Pages generation**. Simply use the included deployment scripts:

1. Clone the repository and install dependencies.
2. Run the deployment script to push the static `/out` directory to your `gh-pages` branch seamlessly:

```bash
bun run deploy
```

3. Head over to **Settings -> Pages** in your GitHub repository and ensure the source branch is set to `gh-pages`. In a few minutes, your site will be live!

---

## How It Works ⚙️
1. Input your Deepgram API Key (It is saved using local storage).
2. Configure **Advanced Settings** based on what metadata you require.
3. Drag & Drop an MP3 file (or click the dashed box). 
4. Deepgram's Nova-3 (or whichever model you select) will transcribe the file via direct post requests.
5. Export your summary, topics, and transcribed results to Markdown.
