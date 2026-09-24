# Horse Nation Stalmanagement

Eén bestand (`index.html`) — geen build nodig, werkt direct via GitHub Pages.
Alles zit in één app, met vier tabbladen: **Kladblok**, **Stamboom**, **Predicaten** en **Trainingscentrum**.

## Zetten op GitHub Pages
1. Vervang in je bestaande repository `index.html` (en `README.md`) door deze versie. Laat `.nojekyll` staan.
2. Je gegevens blijven gewoon staan: ze zitten in je browser en in Dropbox, niet in het bestand.
3. Na een minuutje staat de nieuwe versie online op hetzelfde adres. Dropbox blijft gekoppeld, want het adres verandert niet.

## De tabbladen
- **Kladblok** — groepen, kleuren, status-iconen, vader/moeder, S/D/G. Nieuw per paard, onder "Predicaat & wedstrijden":
  - het **predicaat** (Ster, Keur, Elite, Preferent), met een badge achter de naam;
  - de **leeftijd**: vul in wat het spel nu toont, de app telt daarna zelf door (1 jaar per week);
  - het **niveau per discipline** (Dressuur, Springen, Reining, Trail, Western Pleasure);
  - welke eisen het paard al haalt voor het **volgende predicaat**;
  - de lijst met **nakomelingen**, automatisch gevonden via vader en moeder. Met **+ Veulen toevoegen** voer je een veulen direct in (naam, geslacht, SDG, predicaat, geboortedatum); het komt als extern paard in de database met dit paard als vader of moeder. SDG en predicaat van een veulen pas je in de lijst meteen aan, met × koppel je een veulen los.
  Een 🔔 achter de naam betekent: klaar voor keuring.
- **Stamboom** — stamboom en inteelt-check. Ook externe paarden (bijv. verkochte veulens) kunnen hier een predicaat krijgen, zodat ze meetellen voor hun ouders.
- **Predicaten** — overzicht van je stal: wie klaar is voor keuring (met een knop om het predicaat meteen toe te kennen), wie nog één eis mist, het Preferent-traject per paard met de stand van elk veulen, en een lijst van alle paarden.
- **Trainingscentrum** — kosten, klikjes, planning, stalgroepen en fokken. Bij "Mijn paard" kun je een paard uit je stal kiezen; de niveaus komen dan uit het Kladblok.

## Werking
- Alles wordt automatisch bewaard in de browser (localStorage) en, als je die gekoppeld hebt, in Dropbox.
- **Exporteer back-up (JSON)** en **Importeer back-up** nemen ook de nieuwe velden mee.
- De instellingen van het Trainingscentrum (methode, trainers, combo) worden alleen in de browser bewaard, niet in Dropbox.

## Dropbox-koppeling (sync tussen apparaten)
Ongewijzigd: met de "Dropbox"-knop bovenin synchroniseer je je gegevens tussen apparaten.
Zie de uitleg in de app voor het eenmalig instellen (App key, Redirect URI, permissions).
