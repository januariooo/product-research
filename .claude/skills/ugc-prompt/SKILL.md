---
name: ugc-prompt
description: Maak een nieuwe UGC-videoprompt voor een product in prompts/, in exact hetzelfde format als de bestaande prompts. Gebruik wanneer de gebruiker een UGC-video, video-prompt of avatar-script voor een product vraagt, of /ugc-prompt typt.
---

# UGC-videoprompt maken

Argumenten: `$ARGUMENTS` (productnaam, eventueel gevolgd door wensen zoals doelgroep,
avatar, hook, CTA of lengte).

## Stappen
1. Lees `template.md` (in deze map) en het voorbeeld `prompts/tart-cherry-extract-ugc.md`
   zodat toon, detailniveau en opmaak exact overeenkomen.
2. Bepaal uit de argumenten: product, doelgroep, avatar, hook en CTA. Ontbreekt iets,
   kies dan zelf een logische keuze die bij het product past en noem die aan het eind.
   Vraag alleen door als het product zelf onduidelijk is.
3. Schrijf `prompts/<product-slug>-ugc.md` door het template volledig in te vullen:
   - Alles in het Engels.
   - Script ~25 s, hook in 0–3 s, CTA in de laatste 5 s, plus een 15 s-variant.
   - Master prompt: één doorlopende alinea, concreet over persoon, licht, locatie,
     props en camerastijl. Negative prompt erbij.
   - Avatar-prompt matcht exact met de persoon uit de master prompt.
   - Compliance afgestemd op dit product (welke claims verboden zijn).
4. Controleer: alle 6 secties aanwezig, tijden in de shotlist sluiten aan, geen
   medische/genezende claims.
5. Commit `Add <Product> UGC video prompt` en push naar de huidige branch.
6. Geef een korte samenvatting in het Nederlands: bestand, gekozen hook/avatar/CTA.
