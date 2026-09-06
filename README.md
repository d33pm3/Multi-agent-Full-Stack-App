# SEBI Compliance Command Centre

**Author:** DK Mendiratta

Unofficial frontend demo of a SEBI compliance command centre for listed-company filing tracking (LODR / PIT-style register items). Seeded dashboard, simulated register agent, and risk queue.

This is not SEBI software and not a live filing system.

The build plan (modules M1–M3) is in [plan.md](plan.md).

Neighbour repo: [SEBI-Compliance-Research](https://github.com/d33pm3/SEBI-Compliance-Research) researches live obligations into a 12-column workbook. This repo is the UI demo over seeded rows.

## This is / this is not

**This is** an unofficial frontend demo of a SEBI Compliance Command Centre (register simulation, dashboard, risk queue).
**This is** a local Vite/React app with ~80 seeded compliance rows in Zustand.
**This is** an evaluation UI — the “register agent” is a progress simulation, not a live extractor.
**This is not** SEBI, NSE, or BSE software.
**This is not** [SEBI-Compliance-Research](https://github.com/d33pm3/SEBI-Compliance-Research) (that repo researches live obligations into a 12-column workbook).
**This is not** a full-stack multi-agent platform or a live LLM pipeline.
**This is not** a filing, calendar submission, or compliance opinion.
**This is not** a complete `src/` tree on `main` — the runnable source is in `Codebase.zip`.

## Where the source is

The **complete application source** is in [`Codebase.zip`](Codebase.zip), under:

- `1_SEBI Full Stack App/src/`
- `1_SEBI Full Stack App/public/`

There is no runnable `src/` on `main`. Extract the zip before `npm run dev`.

## Run the eval build

Requires Node.js 18+ and npm.

```bash
git clone https://github.com/d33pm3/Multi-agent-Full-Stack-App.git
cd Multi-agent-Full-Stack-App
unzip -o Codebase.zip
cp -a "1_SEBI Full Stack App/src/." src/
cp -a "1_SEBI Full Stack App/public/." public/
npm i
npm run dev
```

After extract, `src/main.tsx` must exist. If it does not, the zip did not unpack.

```bash
npm test
npm run build
```

## What is not deployed

- There is no hosted URL, GitHub Pages site, or SEBI/exchange integration.
- Persistence is in-memory Zustand for the session only.
- The register-agent Run button is a timed log simulation, not a PDF extractor.
- Do not treat dashboard due dates, risk flags, or exports as a filing or a compliance conclusion.

## License

MIT. See `LICENSE`.

You may use this code; this is not a SEBI filing system and not a live compliance conclusion.
