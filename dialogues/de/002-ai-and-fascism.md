---
dialogue: 004
title: Gesperrte Seiten lesen — Presselinks, Le Monde diplomatique und Bot-Blockaden
date: 2026-06-29
lang: de
participants: Jean-Pierre, Claude
---

# Gesperrte Seiten lesen — Presselinks, Le Monde diplomatique und Bot-Blockaden

> *Hinweis: In diesem Dialog waren die Prompts ursprünglich auf Englisch und Claudes Antworten ursprünglich auf Deutsch. Auf dieser deutschen Seite sind die Prompts Claudes Übersetzungen der englischen Originale; die Antworten sind die deutschen Originale. Siehe die [englische Seite](https://jeanpierre-airesearch.github.io/ai-and-fascism/dialogues/en/004-fetching-blocked-pages.html).*

**Frage 1 — Jean-Pierre:**

Kannst du die Artikel-URLs von https://www.authoritarian-stack.info/press extrahieren und die Artikel lesen?

**Antwort 1 — Claude:**

Nein, zuverlässig nicht — aus denselben Gründen, die schon Dialog 003 zeigt. Ich habe den direkten Abruf von …/press zweimal versucht; beide Male wurde er durch Bot-Erkennung blockiert (einmal mit, einmal ohne spezielle Extraktion). Die Seite lässt automatisierten Zugriff also aktiv nicht zu. Der Umweg über den Suchindex lieferte nur den Lizenz- und Methodik-Text der Seite (Creative-Commons-Lizenz, Datenstand Oktober 2025) — keine Liste der Presseartikel mit URLs. Das passt zum Befund von 003: Der eigentliche Inhalt wird clientseitig per JavaScript gerendert, der Crawler bekommt nur statische Fußzeilen. Auf Drittseiten fand ich zwar verwandte Links (u. a. zu The Nerd Reich, CBS News, BBC, FAS und Politico Pro), aber sie waren nicht nachweislich die …/press-Links der Website selbst und im Snippet abgeschnitten — solche unvollständigen, ungeprüften URLs gebe ich nicht als geprüft aus. Verlässlicher Weg: Öffne …/press im Browser und füge mir die Artikel-URLs direkt in den Chat ein; dann rufe ich jede einzeln ab, lese die zugänglichen Artikel vollständig und lege für die empfohlenen je eine geprüfte Quelle an.

**Frage 2 — Jean-Pierre:**

Kannst du https://mondediplo.com/2025/11/02tech lesen — und auch die in diesem Artikel angegebenen Quellen?

**Antwort 2 — Claude:**

Den Monde-diplomatique-Artikel selbst konnte ich nicht öffnen — er ist gesperrt. Aber ich habe eine frei zugängliche englische Fassung desselben Essays von Francesca Bria bei der Rosa-Luxemburg-Stiftung vollständig gelesen (die RLS hat das Projekt mitfinanziert). Inhaltlich ist das mit hoher Wahrscheinlichkeit derselbe bzw. ein Schwester-Text zur LMd-Version — aber eine andere Publikation; die unten genannten Links sind also die Quellen *dieses* RLS-Artikels, nicht eine verifizierte Kopie der LMd-Quellen. Worum es geht: Der Essay beschreibt, wie sich unter Trumps zweiter Amtszeit ein Block aus Tech-Milliardären, Wagniskapital und Ideologen formiert, der einen vertikal integrierten, privatisierten Kontrollapparat baue — von Cloud und KI über autonome Drohnen und Militärsatelliten bis zur Geldinfrastruktur. Als Auslöser nennt Bria den rund 10-Milliarden-Dollar-Vertrag der US-Armee mit Palantir von Ende Juli 2025 und verweist u. a. auf „Detachment 201", einen 30-Mio.-Dollar-ICE-Vertrag für eine Plattform namens ImmigrationOS und die Ausbreitung nach Europa (Palantir bei NHS und deutscher Polizei, Anduril/Rheinmetall-Drohnen, Starlink in Italien). Die im RLS-Artikel eingebetteten Quell-Links: authoritarian-stack.info und euro-stack.info; die US-Army-Seite zu „Detachment 201"; die NHS Federated Data Platform; Deutsche Welle (Palantir bei deutscher Polizei); Euronews (Rheinmetall–Anduril); und Bloomberg (Italien–Starlink). Wie möchtest du weiter vorgehen? Ich kann diese Links einzeln abrufen, die zugänglichen vollständig lesen und für die belastbaren je einen geprüften sources/-Eintrag anlegen (Bloomberg ist sehr wahrscheinlich durch Paywall gesperrt). Für die echten LMd-Quellen müsstest du mir den Artikeltext oder die Linkliste aus deinem Browser einfügen.

**Frage 3 — Jean-Pierre:**

Als Mensch mit Firefox ist https://mondediplo.com/2025/11/02tech im Volltext ohne Paywall verfügbar. Hast du eine Idee, warum du die Seite nicht abrufen kannst?

**Antwort 3 — Claude:**

Gute Frage — und es liegt nicht an einer Paywall. Für dich im Browser ist der Artikel frei lesbar; das Problem sitzt auf der Abrufseite. Mein Fetch-Tool meldete bei mondediplo.com „SITE_BLOCKED" — das ist etwas anderes als die „Bot-Erkennung" bei der Authoritarian-Stack-Seite und heißt meist, dass der Abruf gar nicht erst durchgelassen, sondern vorab abgewiesen wird. Wahrscheinliche Ursachen, der Reihe nach: Am häufigsten eine serverseitige Bot-Abwehr — viele Redaktionsseiten blocken automatisierte Zugriffe anhand von Signalen, die ein echter Firefox mitbringt (voller User-Agent, JavaScript, Cookies, plausibles Verhalten) und ein Fetcher nicht; mein Abruf sieht für die Schutzschicht wie ein Bot aus und wird abgewiesen, unabhängig davon, ob der Inhalt frei wäre. Möglich ist auch eine Sperrung auf meiner Tool-Seite: Anthropics Abruf respektiert u. a. robots.txt und eigene Zugriffsregeln; manche Domains werden grundsätzlich nicht abgerufen. Welche der beiden Ursachen genau greift, kann ich von hier aus nicht sicher unterscheiden — die Meldung sagt nur „blockiert", nicht „warum". Wichtig: „Frei ohne Paywall" und „maschinell abrufbar" sind zwei verschiedene Dinge; eine Seite kann für Menschen offen und zugleich für automatisierte Clients gesperrt sein. Praktischer Ausweg: Kopier mir den Volltext (oder die relevanten Absätze) aus Firefox in den Chat — dann lese ich ihn daraus und lege einen geprüften sources/-Eintrag an; die enthaltenen Quell-Links rufe ich einzeln ab, soweit sie nicht ebenfalls blockiert sind.