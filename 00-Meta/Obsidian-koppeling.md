---
titel: Obsidian-koppeling
domein: meta
type: proces
status: concept
eigenaar: Johnno van den Brink
laatst_bijgewerkt: 2026-06-30
tags: [meta, obsidian, git]
aliassen: [obsidian, vault, sync]
gerelateerd: ["[[Hoe-werkt-dit-brain]]"]
---

# Obsidian-koppeling

Deze GitHub-repo dient als **Obsidian vault**. Zo werk je lokaal in Obsidian en synchroniseer
je via Git.

## Eenmalige setup

1. Clone deze repo lokaal: `git clone <repo-url>`.
2. Open in Obsidian via **Open folder as vault** en kies de gekloonde map.
3. Installeer de community plugin **Obsidian Git** voor automatische sync (commit & push).
4. Stel in Obsidian in: **Settings → Files & Links → New link format = Relative path**
   (zodat wikilinks ook op GitHub blijven werken waar mogelijk).

## Werkwijze

- Schrijven en linken doe je in Obsidian.
- Obsidian Git commit en pusht je wijzigingen (handmatig of op interval).
- Wijzigingen van collega's haal je op met **pull**.

## Aandachtspunten

- De map `.obsidian/` bevat je persoonlijke instellingen. Spreek af of die wel/niet in
  Git komt (kan conflicten geven bij meerdere gebruikers).
- Wikilinks `[[Bestandsnaam]]` werken perfect in Obsidian; op GitHub renderen ze als
  platte tekst. Voor belangrijke navigatie (zoals README) gebruiken we daarom gewone
  Markdown-links `[tekst](pad)`.

> ⚠️ TE VERIFIËREN: definitieve afspraken over `.obsidian/` in Git en sync-frequentie.
