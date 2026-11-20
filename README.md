# 🐾 Dieren sorteren – mapjes benoemen en slepen

Een interactieve leeroefening voor kinderen in de browser. Ze **benoemen eerst vijf mapjes** (leefgebieden) en **slepen daarna dierenkaartjes** naar het juiste leefgebied. De oefening is één HTML-bestand en heeft geen installatie of internetverbinding nodig.

## ✨ Functies

- **Vijf leefgebieden**: Oceaan 🌊, Jungle 🌴, Savanne 🌾, Woestijn 🏜️ en Poolgebied ❄️. Elk mapje heeft een eigen kleur en een korte hint.
- **25 dieren** (5 per leefgebied) met emoji. Bij elke start of reset worden ze willekeurig geschud.
- **Twee stappen**:
  1. Geef elk mapje de juiste naam. Synoniemen worden ook goedgekeurd, bijvoorbeeld *zee*, *regenwoud*, *steppe* of *noordpool*.
  2. Als alle mapjes goed benoemd zijn, worden de dierenkaartjes actief en kunnen ze versleept worden.
- **Schermtoetsenbord**: handig op een touchscreen of digibord.
- **Nakijken**: mapjes kleuren kort groen (alles goed) of rood (er zit een fout in).
- **Eindresultaat**: een overzicht met de score en een lijst van foute en niet-geplaatste dieren, met daarbij de map waar ze wel horen.
- **Reset / Opnieuw**: start de oefening opnieuw.

## 🚀 Gebruik

1. Download of clone deze repository.
2. Open `dieren_sorteren_mappen.html` in een moderne browser (Chrome, Edge, Firefox of Safari).
3. Speel de oefening:
   - Typ in elk mapje de naam van het leefgebied, met het gewone toetsenbord of met het schermtoetsenbord. Met het gewone toetsenbord wordt het antwoord direct gecontroleerd. Met het schermtoetsenbord druk je op **OK ↵** om te controleren.
   - Sleep alle dieren uit de **Dierenbank** naar het juiste mapje.
   - Klik op **Nakijken** voor tussentijdse feedback, of op **Eindresultaat** voor het overzicht.

> ℹ️ Slepen gebruikt HTML5 drag-and-drop. Dat werkt het best met een muis of op een digibord. Op sommige tablets en telefoons werkt slepen mogelijk niet.

## 📁 Bestanden

| Bestand | Beschrijving |
|---|---|
| `dieren_sorteren_mappen.html` | De oefening zelf (HTML, CSS en JavaScript in één bestand). |
| `Dierenmapjes.txt` | Python-script dat dezelfde HTML (v2.9) als string bevat en naar een `.html`-bestand wegschrijft. |
| `README.md` | Deze uitleg. |

## 🛠️ Aanpassen

Alle inhoud staat bovenaan het `<script>`-blok in `dieren_sorteren_mappen.html`:

- **`FOLDERS`**: de mapjes. Per mapje: `id`, `name`, `icon`, `colorClass`, `answers` (goedgekeurde namen, niet hoofdlettergevoelig) en `desc` (hint).
- **`ANIMALS`**: de dieren. Per dier: `id`, `name`, `emoji` en `folder` (het `id` van het juiste mapje).

Voorbeeld: een dier toevoegen

```js
{id:'zeehond', name:'Zeehond', emoji:'🦭', folder:'pool'},
```

Voeg je een nieuw mapje toe, maak dan ook een kleurklasse (`.c-...`) en een kleurvariabele in het `<style>`-blok.

## 📜 Licentie

Er is nog geen licentie toegevoegd. Neem contact op met de eigenaar van de repository als je de oefening wilt hergebruiken.
