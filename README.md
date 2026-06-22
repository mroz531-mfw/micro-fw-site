# micro-fw.com

The website for **Micro Financial Wellness** — Mike Roselli's financial-coaching business. One page, no build step.

**👉 If you're Mike, open [`START-HERE.md`](START-HERE.md) first.** It walks you through everything in plain English: getting your web address working, editing the site, swapping photos, and undoing mistakes.

## What's in here
- `index.html` — the whole site (all the words live in this one file).
- `emblem.png` — the logo. `mike.jpg` — the headshot.
- `START-HERE.md` — the full, plain-English owner's guide.

## How it's hosted
A free static site on **GitHub Pages**. There's no build step — `index.html` is served as-is, and anything you save (commit) goes live within about a minute. The custom web address, micro-fw.com, is connected through your domain settings at Namecheap (walked through in START-HERE, Step 5).

## Connecting micro-fw.com — technical quick reference
START-HERE.md has the friendly, step-by-step version. The short of it:
1. In GitHub → **Settings → Pages**, set the custom domain to `micro-fw.com` (this creates a `CNAME` file automatically).
2. At **Namecheap → Advanced DNS**, delete the default parking records, then add:
   - four **A records** on host `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - one **CNAME** on host `www` → `YOUR-USERNAME.github.io`
3. Back in **Settings → Pages**, check **Enforce HTTPS** once it becomes available.

(GitHub's A-record IPs are current as of mid-2026; if the domain ever won't verify, re-check them in GitHub's "Managing a custom domain" docs.)
