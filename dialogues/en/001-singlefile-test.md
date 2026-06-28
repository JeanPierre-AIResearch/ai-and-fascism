---
dialogue: 001
title: Single-file test
date: 2026-06-28
lang: en
participants: Jean-Pierre, Claude
---

# Single-file test

We are testing the new combined-file workflow, where one bilingual Markdown file is split by the push tool into two language pages. This file carries an English block and a German block separated by HTML-comment markers, and the tool should commit the English half to `dialogues/en/` and the German half to `dialogues/de/` under the same name. A successful push confirms that the split, the markers, and the two-file repository structure all work end to end.