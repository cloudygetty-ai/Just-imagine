# Just Imagine

**All-in-one AI app designer, architect, and deployment platform.**

Just Imagine is a multi-agent creative orchestration system that turns a single description into complete, production-ready deliverables — slides, video, documents, audio — in seconds.

## Features

- **Multi-agent orchestration**: Researcher, Writer, Designer, and Producer agents working in parallel
- **Any output format**: `.pptx`, `.pdf`, `.mp4`, `.mp3`, `.docx`, and more
- **Autonomy Mode**: Set it and walk away — the system builds while you sleep
- **Real-time director log**: Watch every agent's progress live

## Quick Start

Open `app.html` directly in a browser for the full interactive prototype.

For the full production deployment:

```bash
npm install
npm run dev
```

## Architecture

```
just-imagine/
├── app.html          # Standalone interactive prototype
├── src/
│   ├── agents/       # Individual agent modules
│   ├── orchestrator/ # Multi-agent coordinator
│   ├── renderers/    # Output format renderers
│   └── ui/           # React frontend
├── server/           # Node.js API + WebSocket server
└── docker-compose.yml
```

## Deployment

- **Frontend**: Deploy to Vercel (`npm run build`)
- **Backend**: Deploy to Railway or Render
- **Environment variables**: Copy `.env.example` to `.env`

## Stack

- Frontend: React 18, Vite, TailwindCSS
- Backend: Node.js, Express, Socket.IO
- Agents: Claude API (Anthropic)
- Output: LibreOffice, FFmpeg, pdf-lib
