# Edgar Licea — Portfolio Site

A personal portfolio of Edgar's AI/Claude work, built July 17, 2026. Static HTML/CSS, no build step, no dependencies. This README is the complete handoff: a fresh Claude session (or human) can continue the project from this file alone.

## Purpose

1. **Primary:** application for the onX Maps **Senior Web Platform Manager** role (Marketing dept, Greenhouse job ID 4682133006, $150k–185k). The role wants: a website run as a measurable growth engine, SEO plus "emerging AI-driven discovery channels" (GEO), GA4/GSC fluency, CMS architecture, scalable web production processes, AI-driven workflows, program management. Every page is framed against those requirements.
2. **Secondary:** a lasting thought-leadership home for Edgar's GEO and AI-operations work.

Positioning line: **"I run websites as growth engines. I build the AI workflows that scale them."**

## Files

```
index.html                          Home: hero, resume-backed stats, 5 work cards
geo.html                            Flagship GEO page ("Why it matters and how I do it")
toolkit.html                        6 custom Claude skills + MCP integrations
about.html                          Bio ("How hard can it be?") + outdoors section
projects/publishing-pipeline.html   CTO Studio AI publishing pipeline case study
projects/content-intelligence.html  Quote bank + news-cut case study
projects/ai-reporting.html          Weekly SEO+GEO reporting automation case study
css/style.css                       All styling (bold editorial: Fraunces + Inter,
                                    cream/ink/vermilion). Linked as style.css?v=3 —
                                    bump the version whenever CSS changes.
source-materials/                   Files Edgar provided (resume PDF)
```

Preview locally: `python3 -m http.server 8741 --directory .` then open http://localhost:8741

## Editorial rules (Edgar's explicit directives — do not violate)

- **Zero em dashes** anywhere, ever. Use commas, colons, periods.
- **Never mention "Howdy" or howdy.com.** The employer is always "a Y Combinator-backed (talent) company" in prose, "YC-Backed Company" in card tags/kickers. CTO Studio and ctostudio.com stay by name (public brand). Moonshine Rods and Flylords stay by name.
- **No claims that Edgar manages a web development team.**
- Edgar's title is **Senior Program Manager, US Marketing** (never "product manager").
- **Present tense, active systems.** These tools run weekly; never frame the work as finished/past.
- Card titles are **one plain sentence describing what the tool does, with a stat baked in** ("A tool that lets the team update the live website from a spreadsheet: 481 deploys in 4 months"). Written for a hiring manager who should think "we need someone who can connect and automate tools."
- Every number on the site must be verifiable. Do not inflate. When a claim can't be verified, use the defensible framing (see stats below).

## Verified stats and their sources (as of July 17, 2026)

From the ctostudio GitHub repo (`git` counts, howdycom/ctostudio):
- **51** guest bio pages live; **74** transcripts processed; launched **March 2026**
- **481** commits by github-actions bot = "481 automated deploys in 4 months" (Edgar personally: 144; Jorge Gonzalez: 35 — do NOT credit all 661 commits to Edgar)
- 7 interviews shipped in one two-week span; new interviews record weekly in San Francisco and Austin (Volume 002 in production)

From Gauge (withgauge.com, live tracking):
- Brand visibility on non-branded tracked prompts: **21.6% (March) → 25.0% (July)** = "1 in 4, up from 1 in 5"
- Citation rate: **39.5%** ("approaching 40%")
- **#1 most-cited brand in category**: 36.5% vs linkedin.com 15.3% (30-day window) = "more than 2 to 1"
- Prompt library: **841 total, 735 non-branded** → site says "700+ tracked prompts" (Edgar suggested "1,000+" but data says 841; we kept it honest)

From Search Console (via Gauge):
- Branded "howdy" query clicks: 332 (Jan window) → 517 (Jun 15–Jul 15) = **+56% branded search growth**

From GA4 (via Gauge) — IMPORTANT caveat:
- AI-referral sessions are roughly FLAT (~41/mo Jan → ~50/mo Jun–Jul). Do NOT claim AI referral traffic growth. The site's honest framing: AI answers send demand, not clicks; the downstream signal is branded search (+56%), and referrals now come from 4 platforms (ChatGPT, Gemini, Claude, +1) vs effectively 1 in January.

From Edgar's resume (his own public claims, safe to cite):
- 14 years in marketing/product/program management
- 700%+ website traffic growth in under 2 years (~26K monthly visitors at peak)
- 4,000+ developer leads captured for a YC-backed client (LATAM)
- Moonshine Rods: 400% organic blog traffic growth in one year
- Stack: WordPress, WP Engine, Shopify, Webflow, Buffer, ClickUp, Asana, Klaviyo, HubSpot, SEMrush, Gauge, SimpleAnalytics, GA4, Google Ads, Meta Ads
- B.S. Marketing/Communications, University of North Texas

## Contact details used on the site

- Email: edgar@licea.email
- LinkedIn: https://www.linkedin.com/in/edgar-licea-8003b765/
- Instagram: https://www.instagram.com/e.dgr (About page + footer)
- Personal facts on About: certified Orvis-Endorsed fly fishing guide based in Colorado; avid off-roader and overlander. (Deliberate onX culture-fit signal — onX makes offroad/backcountry/fishing navigation apps.)

## The six custom Claude skills on the Toolkit page

All real, all in production. publish-bio (orchestrator: transcript → live page, delegates to the others), guest-bio (transcript → full profile fields), transcript-clean (raw transcript → crawlable HTML), build-bio-pages (scoped on-demand deploys to GitHub), quote-bank (timecoded quote index), news-cut (news → montage video script package). Framed as one multi-agent publishing system, humans only approve.

## Open items (in priority order)

1. **Headshot**: drop into `img/edgar.jpg`. About page has a commented placeholder slot. Ideally an outdoors shot (river or rig) — it reinforces the closing section.
2. **Deploy**: create a GitHub repo on Edgar's PERSONAL GitHub account, push, enable GitHub Pages. Free `<username>.github.io/<repo>` URL first; custom domain later with zero rework. (This export was made because the original session ran on Edgar's work accounts.)
3. **Flylords case study**: currently a "coming soon" card on the home page + a paragraph on geo.html (4-week engagement, onboarded founder + chief editor: create new content AND update existing content for maximum ROI). Edgar will supply details; needs founder's OK before citing specific results.
4. **Final confidentiality read-through** before the URL is shared anywhere: Edgar approved the anonymized GEO figures for drafting, but give him one last explicit yes/no on geo.html once live.

## Design system

Cream paper (#faf4ea), ink (#171310), vermilion accent (#e8430f). Fraunces (display) + Inter (body) via Google Fonts. Bordered cards with offset hover shadow, black TL;DR blocks, numbered "flow" lists (title on its own line, description below), stat tiles, responsive at 860px and 560px breakpoints. Cache-bust CSS via the `?v=N` query on every stylesheet link.
