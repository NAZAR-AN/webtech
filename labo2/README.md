# Labo 2 - reflecties

Naam: (Nazar Andrushchenko)

## 2. Selectors lezen

Welke elementen raakt elke selector? Eén zin per selector.

- a. `header nav ul li a`:Raakt elke link binnen een lijstitem van de navigatie in de header
- b. `article > p`: Raakt elke paragraaf die een direct kind is van een artikel
- c. `.uren li:nth-child(3)`: Raakt het derde lijstitem binnen de class uren
- d. `h2 ~ p`: Raakt elke paragraaf die volgt op een h2 binnen dezelfde ouder
- e. `.rassen li:first-child`: Raakt het eerste lijstitem binnen de class rassen

## 3. Voorspel, dan kijk

Vul de eerste twee kolommen in vóór je de pagina opent. Trede: herkomst, specificiteit, volgorde of overerving (of iets anders, benoem het).

| vraag | mijn voorspelling (kleur) | beslissende trede | uitkomst in de browser | juist? |
|---|------|--------------|------|-----|
| 1 |green |herkomst      |green |juist|
| 2 |blue  |volgorde      |blauw |juist|
| 3 |red   |specificiteit |red   |juist|
| 4 |red   |volgorde      |red   |juist|
| 5 |blue  |specificiteit |blue  |juist|
| 6 |blue  |specificiteit |blue  |juist|
| 7 |red   |              |red   |juist|
| 8 |blue  |specificiteit |blue  |juist|
| 9 |red   |specificiteit |red   |juist|
| 10|green |volgorde      |green |juist|

Bij welke vraag zat je fout, en wat was de reden? (Alles juist? Welke vraag duurde het langst, en waarom?)
Vraag 3 kostte de meeste tijd, omdat ik op zoek was naar de specificiteit.

## 4. De nabouw

- Welke selector koos je voor de links in de navigatie, en waarom geen class? De selector "nav a". Er is geen class gekozen omdat de HTML niet gewijzigd mocht worden en structuurselectie de voorkeur heeft.
- Welke regel kostte je het meeste tijd, en wat was uiteindelijk de oorzaak?

## 6. Je site

- Welke drie waarden staan in je tokenblok, en waarom die? "--papier", "--inkt" en "--accent". Deze vormen de basiskleuren van het visuele ontwerp uit de opgave
- Wat verandert er in je site als je één token wijzigt? Alle elementen die gelinkt zijn aan dat specifieke token nemen direct de nieuwe kleur over

## Thuis: R2.3 (met AI)

Prompt en onbewerkte output staan in `review/`. Minstens vijf bevindingen, elk met een verwijzing naar de sectie of het foutnummer:
1. **Gebruik van pixels in plaats van rem (Sectie 2.8):** In de initiële code stond `font-size: 16px;` op de `body`. Dit moet volgens de regels in `rem` worden uitgedrukt (bijv. `1rem`), zodat de basismaat netjes schaalt.
2. **Onjuiste lettertype-toewijzing (Sectie 2.6 & Opgave):** De opgave stelt dat de hoofdtekst in Verdana en de koppen in Georgia moeten staan. In de eerste versie stonden deze door elkaar in `--font-body`, wat is opgesplitst per elementtype.
3. **Ontbrekende interactieve states (Sectie 2.2):** Niet alle links hadden direct de vereiste `:hover`- en `:focus`-stijlen (zoals de specifieke achtergrondkleurwissel bij `main a`), wat in het stylesheet is aangevuld.
4. **Validatie van structuurselectoren (Sectie 2.7):** Er is gecontroleerd of er geen verboden ID-selectors of `!important`-regels zijn gebruikt, en of er optimaal gebruik is gemaakt van overerving en elementselectoren.
5. **Beheer van lijsten en opmaak (Sectie 2.9):** Het zebrapatroon via `.kaart li:nth-child(odd)` en de bijbehorende list-styling vereisten een correcte toepassing van de `:root`-tokens om de kleuren consistent te houden met de ontwerpspecificaties.