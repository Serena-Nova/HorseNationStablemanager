# Horse Nation Stalmanagement

Eén bestand (`index.html`) — geen build nodig, werkt direct via GitHub Pages.
Alles zit in één app, met zeven tabbladen: **Kladblok**, **Stamboom**, **Predicaten**, **Dracht**, **Namen**, **Waarde** en **Trainingscentrum**.

## Zetten op GitHub Pages
1. Vervang in je bestaande repository `index.html` (en `README.md`) door deze versie. Laat `.nojekyll` staan.
2. Je gegevens blijven gewoon staan: ze zitten in je browser en in Dropbox, niet in het bestand.
3. Na een minuutje staat de nieuwe versie online op hetzelfde adres. Dropbox blijft gekoppeld, want het adres verandert niet.

## De tabbladen
- **Kladblok** — groepen, kleuren, status-iconen, vader/moeder, S/D/G (Stap, Draf en Galop los; de SDG wordt dan vanzelf het totaal). Subgroepen verplaats je met ▲ ▼ binnen een groep, of met "⇄ naar…" naar een andere groep. Nieuw per paard, onder "Predicaat & wedstrijden":
  - het **predicaat** (Ster, Keur, Elite, Preferent), met een badge achter de naam, en de **premie** (1e, 2e, 3e);
  - de **geboortedatum** (of de leeftijd zoals het spel die nu toont); de app rekent de leeftijd zelf uit: na het opgroeien 3 jaar, daarna 1 jaar per week;
  - het **niveau per discipline** (Dressuur, Springen, Reining, Trail, Western Pleasure);
  - welke eisen het paard al haalt voor het **volgende predicaat**;
  - de lijst met **nakomelingen**, automatisch gevonden via vader en moeder. Met **+ Veulen toevoegen** voer je een veulen direct in (naam, geslacht, SDG, predicaat, geboortedatum); het komt als extern paard in de database met dit paard als vader of moeder. Naam, SDG en predicaat van een veulen pas je in de lijst meteen aan (een nieuwe naam wordt overal meegenomen: stamboom, vader/moeder van eigen veulens en 'gedekt met'), met × koppel je een veulen los.
  Een 🔔 achter de naam betekent: klaar voor keuring.
  Verwijder je een paard, subgroep of groep uit het Kladblok, dan blijven de paarden bewaard in de Stamboom (als externe paarden). Zo hoef je ze daar niet opnieuw in te voeren. Met **↩ paard uit database terugzetten** (onder elke subgroep) zet je zo'n paard, met al zijn gegevens, weer terug in het Kladblok.
  Vink je **Fokbonus getraind** aan, dan kies je Western, Engels of Beide en worden de niveaus van die disciplines meteen op het hoogste niveau gezet. **Allround volledig getraind** zet alle disciplines op het hoogste niveau.
- **Stamboom** — stamboom en inteelt-check. Ook externe paarden (bijv. verkochte veulens) kunnen hier een predicaat krijgen, zodat ze meetellen voor hun ouders.
- **Predicaten** — onderaan staat **Dekgeld**: een adviesprijs per hengst. Je vult in wat een hengst met een bepaalde SDG waard is en hoeveel procent de prijs per hele SDG verschilt; de app rekent alle prijzen van 10 tot 40 SDG uit. Per ras kun je eigen prijzen instellen, rassen zonder eigen prijzen gebruiken 'Standaard'. Toeslagen voor fokbonus en predicaat gelden voor alle rassen. Deze instellingen worden per browser bewaard. Bij elke hengst in het Kladblok zie je het advies en kun je je eigen dekgeld invullen.
- **Predicaten** (verder) — overzicht van je stal: wie klaar is voor keuring (met een knop om het predicaat meteen toe te kennen), wie nog één eis mist (paarden met SALE niet), het Preferent-traject per paard met de stand van elk veulen, en een lijst van alle paarden.
- **Dracht** — drie delen:
  - **💞 Dekplanner**: kies een merrie en zie per hengst of je hem al eerder bij je merries hebt gebruikt (via hun veulens en huidige drachten, met een duidelijke waarschuwing als het bij dezelfde merrie was), de minimale SDG van het veulen per letter en het inteeltpercentage. Sorteren kan op hoogste SDG of 'nog niet gebruikt eerst'. Met 'Alleen hengsten van hetzelfde ras' (standaard aan) zie je alleen hengsten van het ras van de merrie. In de lijst staan alleen hengsten die als dekhengst beschikbaar zijn: je eigen hengsten (uit te zetten bij 'Beschikbaar als dekhengst') en hengsten die je in de Stamboom of bij Dekhengsten als dekhengst aanvinkt. Hengsten uit dezelfde lijn als de merrie (vader, zoon, (half)broer, grootvader, kleinzoon of andere familie via gedeelde voorouders) worden standaard verborgen.
  - **Drachtig**: alle merries met Gedekt of Echo positief (uit het Kladblok; met **+ Drachtige merrie toevoegen** voeg je er hier een toe — staat ze nog niet in je Kladblok, dan wordt ze daar in de gekozen groep bij gezet). Hengst en bevallingsdatum pas je in de tabel direct aan, met **uit overzicht** haal je een dracht weg. Verder: met bevallingsdatum (en hoeveel dagen nog), door wie ze gedekt zijn, de minimale SDG van het veulen (het gemiddelde van beide ouders, per letter als S, D en G bekend zijn), of moeder en vader fokbonus hebben, en het geslacht van het veulen als je dat weet. Sorteren kan op bevallingsdatum of SDG.
  - **Dekhengsten**: een lijst met hengsten van andere spelers (naam, stal, ras, S/D/G, fokbonus, predicaat, dekgeld, notitie). Ze staan ook in de Stamboom en in de keuzelijst bij 'Gedekt met'. Kies een merrie en de app rekent per hengst de minimale SDG van het veulen uit.
- **Namen** — een namengenerator. Per ras maak je een of meer thema's (bijvoorbeeld één per lijn, voor gescheiden lijnen). Elk thema heeft een eigen naam en namenlijst (zelf typen, of beginnen met voorbeeldnamen: sterrenkunde, bomen in het Latijn, Iers/Gaelisch, chemische elementen, kruiden, bloemen, eten en snoep, edelstenen, Griekse, Noorse of Egyptische mythologie, weer en natuur, muziek en dans, popcultuur) en welke beginletter-regel geldt: zelfde letter als de moeder of vader, de volgende letter in het alfabet (na de moeder of vader), een vaste letter, of willekeurig. De app herkent de lijn aan de naam van de moeder of vader en kiest dan het bijbehorende thema. Kies een moeder (en vader) en je krijgt vrije namen met de juiste beginletter, zodat de lijn herkenbaar blijft; ook de moederlijn wordt getoond. Namen in je database en in je lijst met gebruikte namen worden overgeslagen. Namensuggesties staan ook bij '+ Veulen toevoegen' en in de bevallings-pop-up. Thema's en gebruikte namen gaan mee met Dropbox en de back-up.
- **Waarde** — een inschatting van wat een paard waard is, afgestemd op de Handelaar: SDG ten opzichte van de start-SDG van het ras, veulen of volwassen, wedstrijdniveau, fokbonus/allround, predicaat, leeftijd (20+), inteelt en marktstand. Je krijgt een Handelaar-indicatie (ondergrens) en een vraagprijs voor de markt. De schatting start met een ingebouwde basis (24 verkopen aan de Handelaar met alle details en de rassenlijst van 29-09-2026) en wordt beter als je in het logboek biedingen en verkopen invult. Heeft een paard een echt bod in het logboek, dan toont de app dat bedrag (met de schatting ernaast). Je eigen bedragen tellen zwaarder mee dan de basis, vooral voor hetzelfde ras. Bedragen worden precies bewaard zoals je ze invult. Rassenlijst en alle factoren zijn aan te passen. Let op: dit is een schatting van deze app, niet van Horse Nation; de bedragen in het spel kunnen afwijken. Logboek en instellingen gaan mee met Dropbox en de back-up.
- **Trainingscentrum** — kosten, klikjes, planning, stalgroepen en fokken. Bij "Mijn paard" kun je een paard uit je stal kiezen; de niveaus komen dan uit het Kladblok.

## Werking
- Alles wordt automatisch bewaard in de browser (localStorage) en, als je die gekoppeld hebt, in Dropbox.
- **Exporteer back-up (JSON)** en **Importeer back-up** nemen ook de nieuwe velden mee.
- De instellingen van het Trainingscentrum (methode, trainers, combo) worden alleen in de browser bewaard, niet in Dropbox.

## Bevallingen
Is de bevallingsdatum van een gedekte merrie voorbij (vanaf de dag erna), dan verschijnt bij het openen van de app een pop-up "Bevallen!". Per merrie kies je **Veulen invoeren** (naam, geslacht, SDG, vader en geboortedatum staan al klaar) of **Geen veulen invoeren**. In beide gevallen worden bij de merrie gedekt, echo en bevallingsdatum uitgezet. Met **Later** verdwijnt de pop-up tot je de app opnieuw opent.

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
