# Bing (incl. Copilot / AI answers)

Share: 9.76% US (StatCounter, Oct 2026). Also powers Yahoo results (see `yahoo.md`).

## Current rules
- Bing Webmaster Tools + IndexNow for fast indexing.
- Ranking rests on the 6 parameters in Microsoft Support's Bing ranking explainer, in general order: 1 Relevance (terms on page, link phrases, synonyms), 2 Quality and Credibility (purpose clarity, usability, reputation, fact vs opinion, first-hand/attributed content), 3 User Engagement (clicks, dwell vs quick return, reformulation), 4 Freshness, 5 Location and Language, 6 Page Load Time.
- GEO format (answer-first, structured, citable) for AI answers. Priority for US Notary Journal.
- Discovery: IndexNow (stream changes, do not batch), XML sitemaps with canonical URLs only and accurate lastmod, crawlable <a href> internal links, allow Bingbot, no critical content behind client-side-only rendering.
- Copilot/grounding limits: noindex removes a URL from Bing + Copilot; noarchive blocks Copilot use; nocache limits Copilot to URL/title/snippet; nosnippet/data-nosnippet limit citation quality. Do not put these on promotable pages.
- Penalties: cloaking, link schemes, keyword stuffing / artificially engineered language (including language engineered to trigger AI citations), prompt injection, scraped/duplicate content, unreviewed large-scale generated content, thin affiliate, misleading structured data.

## Recent changes
- **Announced 2026-10-30, effective 2027-02-01:** AI-preference change. Our migration deadline: 2027-03-01.
- **2026-11-11:** Searcher control to turn AI answers on/off. Not a ranking change.
- No November 2026 ranking/guideline update found as of 2026-11-24.

## Sources
- Webmaster Guidelines: https://www.bing.com/webmaster/help/webmaster-guidelines-30fba23a
- How Bing delivers search results (Microsoft Support): https://support.microsoft.com/en-us/bing/how-bing-delivers-search-results
- AI preferences (Bing Blog, 2026-10-30): https://blogs.bing.com/search/2026/10/your-content-your-choice-clearer-preferences-for-training-and-grounding/
- AI answers on/off (Bing Blog, 2026-11-11): https://blogs.bing.com/search/2026/11/your-choice-turn-ai-answers-on-or-off-in-bing/
- IndexNow: https://www.indexnow.org/en_gb/documentation

Verified: 2026-11-24 by Muse, via Microsoft Support plus Muse's 2026-11-19 reading of the Guidelines.
Note: bing.com is blocked for direct fetch in Muse's environment, so Bing's own pages were not re-fetched today.
