---
dialogue: 004
title: Reading Blocked Pages — Press Links, Le Monde diplomatique, and Bot Blocking
date: 2026-06-29
lang: en
participants: Jean-Pierre, Claude
---

# Reading Blocked Pages — Press Links, Le Monde diplomatique, and Bot Blocking

> *Note: in this dialogue the prompts were originally written in English and Claude's answers originally in German. On this English page, the answers are Claude's English translations of the German originals; the [German page](https://jeanpierre-airesearch.github.io/ai-and-fascism/dialogues/de/004-fetching-blocked-pages.html) carries the original answers and translated prompts.*

**Prompt 1 — Jean-Pierre:**

Are you able to extract the article URLs from: https://www.authoritarian-stack.info/press and read the articles?

**Response 1 — Claude:**

No, not reliably — for the same reasons dialogue 003 already shows. I tried fetching …/press directly twice; both times it was blocked by bot detection (once with, once without special extraction). The page actively refuses automated access. Going through the search index returned only the page's licence and methodology text (Creative Commons licence, data current as of October 2025) — not a list of the press articles with URLs. That matches the finding from 003: the actual content is rendered client-side via JavaScript, so the crawler only receives static footer text. On third-party pages I did find related links (to The Nerd Reich, CBS News, BBC, FAS, and Politico Pro, among others), but they were not verifiably the site's own …/press links and were truncated in the snippet — and I won't present incomplete, unverified URLs as checked. The reliable path: open …/press in your browser and paste the article URLs into the chat; then I'll fetch each one, read the accessible articles in full, and create a verified source for each one I recommend.

**Prompt 2 — Jean-Pierre:**

Can you read: https://mondediplo.com/2025/11/02tech — also the sources provided in this article?

**Response 2 — Claude:**

I could not open the Le Monde diplomatique article itself — it is blocked. But I read in full a freely accessible English version of the same essay by Francesca Bria, published by the Rosa-Luxemburg-Stiftung (which co-funded the project). It is very probably the same text as, or a sibling of, the LMd version — but it is a different publication, so the links below are the sources of *this* RLS article, not a verified copy of the LMd sources. What it argues: under Trump's second term, a bloc of tech billionaires, venture capital, and ideologues is assembling a vertically integrated, privatized apparatus of control — from cloud and AI to autonomous drones, military satellites, and monetary infrastructure. Bria names as the trigger the roughly $10 billion U.S. Army contract with Palantir of late July 2025, and points to "Detachment 201," a $30 million ICE contract for a platform called ImmigrationOS, and the spread into Europe (Palantir at the NHS and with German police, Anduril/Rheinmetall drones, Starlink in Italy). The source links embedded in the RLS article: authoritarian-stack.info and euro-stack.info; the U.S. Army "Detachment 201" page; the NHS Federated Data Platform; Deutsche Welle (Palantir and German police); Euronews (Rheinmetall–Anduril); and Bloomberg (Italy–Starlink). How would you like to proceed? I can fetch these links one by one, read the accessible ones in full, and create a verified source entry for each solid one (Bloomberg is very likely paywalled). For the actual LMd sources, you would need to paste the article text or its link list from your browser.

**Prompt 3 — Jean-Pierre:**

As a human using Firefox, https://mondediplo.com/2025/11/02tech is available in full text without a paywall. Any idea why you can't fetch the page?

**Response 3 — Claude:**

Good question — and it isn't a paywall. In your browser the article is freely readable; the problem sits on the retrieval side. My fetch tool reported "SITE_BLOCKED" for mondediplo.com — which is different from the "bot detection" I hit on the Authoritarian Stack site, and usually means the request is refused before it ever reaches the page. The likely causes, in order: most often a server-side bot defence — many news sites block automated access using signals a real Firefox carries (a full user-agent, JavaScript execution, cookies, plausible behaviour) and a fetcher does not; my request looks like a bot to the protection layer and is turned away regardless of whether the content is free. It could also be a block on my tool's side: Anthropic's fetcher respects robots.txt and its own access rules, and some domains are simply not retrieved. Which of the two applies here I cannot tell for certain from where I sit — the message only says "blocked," not "why." The key distinction: "free, no paywall" and "machine-retrievable" are two different things; a page can be open to humans yet closed to automated clients. The practical workaround: paste the full text (or the relevant paragraphs) from Firefox into the chat — then I'll read it from there and create a verified source entry; I'll fetch the embedded source links one by one, as far as they are not also blocked.