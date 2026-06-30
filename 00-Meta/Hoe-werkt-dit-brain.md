---
titel: Hoe werkt dit brain
domein: meta
type: naslag
status: actueel
eigenaar: Johnno van den Brink
laatst_bijgewerkt: 2026-06-30
tags: [meta, handleiding, onboarding]
aliases: [start, handleiding, uitleg]
gerelateerd: ["[[Schrijfrichtlijnen]]", "[[Taxonomie-en-Tags]]"]
---

# Hoe werkt dit brain

Dit document legt uit hoe het BWJ AI Brain is opgebouwd en hoe je het gebruikt.

## Wat is het doel?

Dit brain is de **single source of truth** van BWJ Ecommerce. Het voedt:

1. **De AI-chatbot** — die antwoorden geeft aan klanten en/of medewerkers op basis van
   deze bestanden.
2. **Het team** — als kennisbank, doorzoekbaar in Obsidian of GitHub.

> 💡 Vuistregel: *als de chatbot het moet kunnen weten, moet het hier staan.*

## Hoe is het opgebouwd?

De kennis is verdeeld in **domeinen** (genummerde mappen). Binnen elk domein staan
**atomaire documenten**: één onderwerp per bestand. Zo vindt zowel de mens als de AI
snel het juiste antwoord.

Elk document heeft bovenaan **frontmatter** (metadata tussen `---`). De chatbot gebruikt
deze velden om te filteren (bijv. "geef alleen `actueel` beleid") en om bronnen te tonen.

## Documenttypes

| Type | Waarvoor | Template |
|------|----------|----------|
| `kennisartikel` | Algemene uitleg / naslag | [[Template-Kennisartikel]] |
| `faq` | Veelgestelde vragen (Q&A) | [[Template-FAQ]] |
| `proces` | Stap-voor-stap werkwijze | [[Template-Proces]] |
| `beleid` | Officiële regels (retour, garantie, ...) | [[Template-Beleid]] |
| `naslag` | Lijsten, definities, referentie | [[Template-Kennisartikel]] |

## Levenscyclus van een document

```
concept  →  in-review  →  actueel  →  verouderd  →  (naar 99-Archief)
```

- **concept**: nog in opbouw, niet betrouwbaar voor de chatbot.
- **in-review**: klaar, wacht op controle door eigenaar.
- **actueel**: goedgekeurd en betrouwbaar. *Alleen dit gebruikt de chatbot idealiter.*
- **verouderd**: niet meer geldig; verplaats naar [99-Archief/](../99-Archief/).

## Koppeling met Obsidian

Deze GitHub-repo is de vault. Zie [[Obsidian-koppeling]] voor de instelling.
Gebruik in Obsidian:
- **Wikilinks** `[[Bestandsnaam]]` om documenten te verbinden.
- **Tags** zoals `#klantenservice/retour` om dwarsverbanden te leggen.
- De **graph view** om gaten in de kennis te ontdekken.

## Hoe voeg ik iets toe?

1. Kies het juiste domein (map).
2. Kopieer een template uit [Templates/](Templates/).
3. Vul de frontmatter volledig in.
4. Schrijf het document volgens de [[Schrijfrichtlijnen]].
5. Zet de status op `in-review` als het klaar is.
