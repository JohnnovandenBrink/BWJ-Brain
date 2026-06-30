---
titel: Schrijfrichtlijnen
domein: meta
type: naslag
status: actueel
eigenaar: Johnno van den Brink
laatst_bijgewerkt: 2026-06-30
tags: [meta, richtlijnen, kwaliteit]
aliases: [conventies, stijlgids]
gerelateerd: ["[[Hoe-werkt-dit-brain]]", "[[Taxonomie-en-Tags]]", "[[Tone-of-Voice]]"]
---

# Schrijfrichtlijnen

Deze richtlijnen zorgen dat het brain consistent, leesbaar en bruikbaar blijft voor de
AI. Een document dat hieraan voldoet, geeft betere antwoorden.

## 1. Eén onderwerp per bestand (atomair)

Splits brede onderwerpen op. Liever 3 korte documenten dan 1 lang document.
Dit verbetert hoe de AI relevante stukken (chunks) terugvindt.

## 2. Altijd volledige frontmatter

Elk bestand begint met frontmatter tussen `---`. Verplichte velden:

| Veld | Uitleg | Voorbeeld |
|------|--------|-----------|
| `titel` | Mensvriendelijke titel | `Retourbeleid` |
| `domein` | Hoofddomein (zie [[Taxonomie-en-Tags]]) | `klantenservice` |
| `type` | `kennisartikel` / `faq` / `proces` / `beleid` / `naslag` | `beleid` |
| `status` | `concept` / `in-review` / `actueel` / `verouderd` | `actueel` |
| `eigenaar` | Wie verantwoordelijk is | `Johnno van den Brink` |
| `laatst_bijgewerkt` | Datum `JJJJ-MM-DD` | `2026-06-30` |
| `tags` | Lijst trefwoorden | `[retour, garantie]` |

Optioneel: `aliases` (synoniemen waarop gezocht/gelinkt wordt — Obsidian herkent deze
Engelse sleutel), `gerelateerd` (wikilinks).

## 3. Schrijf voor mens én machine

- **Begin met het antwoord.** Zet de kern bovenaan, details eronder.
- **Eén H1 (`#`) per document** = de titel.
- **Gebruik beschrijvende koppen** (`##`). De AI gebruikt koppen als context.
- **Korte alinea's en lijstjes.** Vermijd lange lappen tekst.
- **Wees expliciet.** Schrijf "binnen 14 dagen", niet "op tijd". Vermijd "zie boven".

## 4. Taal en toon

- Schrijf in het **Nederlands**.
- Volg de [[Tone-of-Voice]] van BWJ.
- Leg jargon uit of link naar het [[Begrippenlijst|begrippenlijst]].

## 5. Concrete feiten en bronnen

- Noem getallen, termijnen, bedragen en voorwaarden expliciet.
- Verwijst een document naar een extern systeem (bijv. Shopify)? Link of benoem het in
  [07-IT-en-Tools/](../07-IT-en-Tools/).
- Twijfel je over een feit? Zet status op `concept` en markeer met `> ⚠️ TE VERIFIËREN`.

## 6. Onderhoud

- Werk `laatst_bijgewerkt` bij na elke wijziging.
- Verouderd? Status op `verouderd` en verplaats naar [99-Archief/](../99-Archief/).
- Vermijd dubbele informatie: link liever naar het bronbestand.
