---
title: AI and Fascism — A Public Dialogic Research Project
---

# AI and Fascism

**A Public Dialogic Research Project**

This site documents an ongoing public research project exploring the relationship between artificial intelligence and fascism. The research takes the form of a structured dialogue between **Jean-Pierre** (human researcher) and **Claude** (an Anthropic AI). Both the questions and the answers are the research material, published in full — without editing or curation — in **English and German**.

The dialogic format reflects a conviction: the way we ask questions about AI and fascism is itself part of the research.

## Dialogues

{% assign en_dialogues = site.pages | where_exp: "p", "p.path contains 'dialogues/en/'" | sort: "path" %}
{% if en_dialogues.size > 0 %}
{% for d in en_dialogues %}{% assign base = d.path | split: "/" | last %}{% assign de_path = "dialogues/de/" | append: base %}{% assign de = site.pages | where_exp: "p", "p.path == de_path" | first %}
- **{{ d.title | default: base }}** — [English]({{ d.url | relative_url }}){% if de %} · [Deutsch]({{ de.url | relative_url }}){% endif %}
{% endfor %}
{% else %}
*No dialogues are published yet.*
{% endif %}

---

*Maintained by Jean-Pierre · ai-and-facism@mailbox.org*
