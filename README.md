# AI Apocalypse companion page

This folder contains the live companion page for the AI Apocalypse Short.

## Files
- `index.html` — the companion page itself

## Free GitHub Pages publish steps
1. Keep `index.html` at the repository root.
2. Commit and push the page assets.
3. In repo settings, open Pages.
4. Choose the branch you pushed to, usually `main` and `/ (root)`.
5. Wait for GitHub Pages to generate the site.
6. Visit the published URL shown by GitHub.

## Recommended repo structure
```text
ai-apocalypse/
├── index.html
└── README.md
```

## Why this helps indexing
- It gives crawlers a public text page.
- It includes the transcript, title, summary, and key terms.
- It exposes VideoObject schema.
- It creates a stable page that search engines and LLMs can read.

## Next automation idea: companion page patch for MMPT
When a new MMPT run finishes, patch the archive and episode pages from the run outputs instead of hand-editing a fresh page.

Use the run artifacts in this order:
1. `aligned.srt` for the transcript
2. `prompts.json` for the visual direction, keywords, and scene language
3. `run.log` for run context and timing
4. the public YouTube Short URL once the video is live
5. TikTok and Bilibili links once they exist

Update these surfaces together:
- `archive.html`
- `archive.json`
- `feed.xml`
- `llms.txt`
- `sitemap.xml`
- the episode page HTML

Keep the page text-first, transcript-heavy, and schema-backed. Leave private or not-yet-public video links out of the public site until the upload is live.
