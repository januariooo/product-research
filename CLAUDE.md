# Product research – instructies voor Claude

Deze repo bevat productonderzoek en kant-en-klare prompts voor AI-gegenereerde UGC-video's.
Claude leest dit bestand automatisch aan het begin van elke sessie.

## Structuur
- `prompts/<product-slug>-ugc.md` – één bestand per product, altijd volgens
  `.claude/skills/ugc-prompt/template.md`.
- Voorbeeld van een af bestand: `prompts/tart-cherry-extract-ugc.md`.

## Vaste afspraken
- Prompts en scripts zijn in het **Engels**; uitleg aan mij mag in het Nederlands.
- Bestandsnamen: kleine letters, koppeltekens, eindigen op `-ugc.md`.
- Altijd dezelfde 6 secties in dezelfde volgorde (master prompt, script/shotlist,
  avatar, voice, captions, compliance).
- Compliance: alleen ervaringstaal ("I feel…"), nooit claims dat iets geneest,
  behandelt of voorkomt. Altijd "#ad"-regel opnemen.
- Na het maken van een nieuw bestand: committen met bericht
  `Add <Product> UGC video prompt` en pushen.

## Nieuwe prompt maken
Gebruik `/ugc-prompt <product> [extra wensen]` – zie `.claude/skills/ugc-prompt/SKILL.md`.
