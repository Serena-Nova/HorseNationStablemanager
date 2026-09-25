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
  - de **geboortedatum** (of de leeftijd zoals het spel die nu toont); de app rekent de leeftijd zelf uit: na het opgroeien 3 jaar, daarna 1 jaar per week;
  - het **niveau per discipline** (Dressuur, Springen, Reining, Trail, Western Pleasure);
  - welke eisen het paard al haalt voor het **volgende predicaat**;
  - de lijst met **nakomelingen**, automatisch gevonden via vader en moeder. Met **+ Veulen toevoegen** voer je een veulen direct in (naam, geslacht, SDG, predicaat, geboortedatum); het komt als extern paard in de database met dit paard als vader of moeder. SDG en predicaat van een veulen pas je in de lijst meteen aan, met × koppel je een veulen los.
  Een 🔔 achter de naam betekent: klaar voor keuring.
  Verwijder je een paard, subgroep of groep uit het Kladblok, dan blijven de paarden bewaard in de Stamboom (als externe paarden). Zo hoef je ze daar niet opnieuw in te voeren.
  Vink je **Fokbonus getraind** aan, dan kies je Western, Engels of Beide en worden de niveaus van die disciplines meteen op het hoogste niveau gezet. **Allround volledig getraind** zet alle disciplines op het hoogste niveau.
- **Stamboom** — stamboom en inteelt-check. Ook externe paarden (bijv. verkochte veulens) kunnen hier een predicaat krijgen, zodat ze meetellen voor hun ouders.
- **Predicaten** — overzicht van je stal: wie klaar is voor keuring (met een knop om het predicaat meteen toe te kennen), wie nog één eis mist (paarden met SALE niet), het Preferent-traject per paard met de stand van elk veulen, en een lijst van alle paarden.
- **Trainingscentrum** — kosten, klikjes, planning, stalgroepen en fokken. Bij "Mijn paard" kun je een paard uit je stal kiezen; de niveaus komen dan uit het Kladblok.

## Werking
- Alles wordt automatisch bewaard in de browser (localStorage) en, als je die gekoppeld hebt, in Dropbox.
- **Exporteer back-up (JSON)** en **Importeer back-up** nemen ook de nieuwe velden mee.
- De instellingen van het Trainingscentrum (methode, trainers, combo) worden alleen in de browser bewaard, niet in Dropbox.

## Delen met anderen
- Nieuwe gebruikers beginnen met een lege stal (groepen "Mijn stal" en "Veulens"). Jouw eigen paarden zien zij niet: die staan in jouw browser en jouw Dropbox.
- Iedereen die de link opent, heeft zijn eigen gegevens in zijn eigen browser.

## Dropbox-koppeling (sync tussen apparaten)
**Voor anderen makkelijk maken (eenmalig, door de eigenaar van de app):**
1. Open `index.html` (op GitHub: bestand openen, potloodje "Edit").
2. Zoek bovenin de regel `window.HN_DROPBOX_APP_KEY="";` en zet je App key tussen de aanhalingstekens, bijvoorbeeld `window.HN_DROPBOX_APP_KEY="abc123xyz";`. De App key is geen wachtwoord; dat is veilig.
3. Ga in de Dropbox App Console naar je app en klik op **Enable additional users**.
4. Controleer dat bij "Redirect URIs" precies het adres van de app staat.

Daarna hoeven anderen alleen op **Dropbox → Verbind met Dropbox** te klikken. Hun gegevens komen in een eigen mapje in hún Dropbox. Tot 500 gebruikers kunnen koppelen; zodra 50 gebruikers gekoppeld zijn, heb je twee weken om bij Dropbox productiestatus aan te vragen, anders kunnen er geen nieuwe gebruikers meer bij.

Wie liever een eigen Dropbox-app gebruikt, kan onder "Eigen Dropbox-app gebruiken (geavanceerd)" een eigen App key invullen.
