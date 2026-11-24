# LinkedIn

## Current rules: Page search ranking
Source: LinkedIn Help, answer a554382. Factors:
- How closely the Page name matches the search term
- Follower count
- Shared connections with the searcher
- Volume of discussion and comments
- Quality of posts, comments and reactions

Verified: 2026-11-24 by Muse, direct open of https://www.linkedin.com/help/linkedin/answer/a554382

## Recent changes
- **2026-11-09:** Profile Relevance uses semantic matching. Profiles and posts should state expertise in plain language.
  Verified: 2026-11-24 by Muse, direct open of LinkedIn Engineering, "Profile Relevance: Boosting Feed Relevance with LLMs at LinkedIn": https://www.linkedin.com/blog/engineering/feed/profile-relevance-boosting-feed-relevance-with-llms-at-linkedin
  - How it works: LinkedIn builds a "member prompt" from public profile fields (headline, summary, key skills, work history, education; name and gender excluded) and matches LLM embeddings of that prompt against post embeddings (post text, titles, transcripts, author location) for Unconnected Content in Feed.
  - Production threshold: a post needs at least 1 viral action (like, comment or share) from an unconnected member before Profile Relevance recommends it.
  - Reported results: +0.54% Feed Updates Viewed, +0.94% viral rate, -18.8% hide rate; cold-start members +17.7% viral engagement.
  - Action for us: Brian's profile headline, summary and skills must state notary operations / electronic notary journal expertise in plain language, or posts will not match the right audience.

Used by: US Notary Journal.

## Sources
- Page search: https://www.linkedin.com/help/linkedin/answer/a554382
- Profile Relevance: https://www.linkedin.com/blog/engineering/feed/profile-relevance-boosting-feed-relevance-with-llms-at-linkedin
- Pages best practices: https://business.linkedin.com/advertise/linkedin-pages/best-practices
