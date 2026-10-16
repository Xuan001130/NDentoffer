FLIPBOOK — quick guide
======================

SWAP THE PDF
  1. Replace document.pdf with your new PDF (keep the name "document.pdf").
  2. Redeploy. That's it. Page count, page shape and title are picked up automatically.

  Optional settings (top of the <script> in index.html, the CONFIG block):
    title   — custom title ("" = use the PDF's own title)
    layout  — "single" (one page at a time, best for landscape slides)
              "spread" (two pages side by side on wide screens, best for portrait docs)
    flipTime — page-turn speed in ms
  Colours are in the SETTINGS block at the top of the <style>.

DEPLOY TO VERCEL
  Option A (no terminal): vercel.com > Add New > Project > drag this folder in.
  Option B (CLI):         cd into this folder, run `vercel`, then `vercel --prod`.
  Option C (GitHub):      push this folder to a repo and import it in Vercel.
  Framework preset: "Other". No build command, no output directory.

TEST LOCALLY
  Opening index.html by double-click won't load the PDF (browser security).
  Run a tiny server in this folder instead, e.g.  npx serve  or  python -m http.server
