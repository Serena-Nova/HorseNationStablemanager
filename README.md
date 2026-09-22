# Horse Nation Stalmanagement

E�n bestand (`index.html`) — geen build nodig, werkt direct via GitHub Pages.
Dit vervangt de losse Kladblok-app: alles zit nu in één app, met twee tabbladen.

## Zetten op GitHub Pages
1. Maak een nieuwe repository aan (bijv. `Horse-nation-stalmanagement`) op je `serena-nova` account.
2. Upload `index.html` en `.nojekyll` naar de `main` branch (root van de repo).
3. Ga naar **Settings → Pages**, kies branch `main` / map `/ (root)`, sla op.
4. Na een minuutje staat je app op `https://serena-nova.github.io/Horse-nation-stalmanagement/`.

Let op: dit is een NIEUWE, LEGE stamboom-database (de losse Horse-stamboom-app blijft
gewoon bestaan op zijn eigen URL, met al je oude stambomen erin — die zijn hier nog niet
overgezet). Je Kladblok-gegevens (paarden, groepen, legenda, kleuren) staan er wel meteen in,
want die komen automatisch uit je vorige Kladblok-versie mee als je 'm in dezelfde browser opent.
Zet je oude Kladblok-versie dus niet weg voor je hebt gecontroleerd dat deze nieuwe versie
alles goed heeft overgenomen.

## De twee tabbladen
- **Kladblok** — precies wat je al had: groepen, kleuren, status-iconen, enz. Nieuw:
  elk paard heeft nu ook een "Vader" en "Moeder" veld (voor de Stamboom-tab) en optionele
  S/D/G-invulvelden.
- **Stamboom** — nieuw. Zoek een paard, vul de vader/moeder in (met auto-aanvullen uit je
  hele database, stal + extern), en zie de stamboom als boomstructuur. Voeg externe paarden
  toe (paarden die niet in jouw stal staan) via "+ Extern paard toevoegen". Onderaan zit een
  inteelt-check (COI): vul een hengst en merrie in en zie het inteeltpercentage over 4
  generaties, met welke voorouders ze delen.

## Wat er (nog) niet in zit t.o.v. je oude Stamboom-app
Bewust weggelaten om dit stap 1 behapbaar te houden — kan later alsnog toegevoegd worden:
- De sleepbare whiteboard-weergave (nu een boomstructuur in plaats van kaartjes die je verschuift)
- Automatische kleur per paard in de stamboomweergave
- De "beste combinaties"-scanner
- Bulk-import, zoom, "losse paarden"-archief

## Werking
- Alles wordt automatisch bewaard in de browser (localStorage) — geen account nodig.
- Onderaan de Kladblok-tab: **Exporteer JSON** (neemt Kladblok + Stamboom-data mee) en
  **Importeer JSON** voor een back-up.

## Dropbox-koppeling (sync tussen apparaten)
Met de "Dropbox"-knop bovenin kun je je gegevens laten synchroniseren tussen bijvoorbeeld
je telefoon en laptop. Dit gaat rechtstreeks tussen je browser en Dropbox — er is geen
apart wachtwoord of server bij betrokken.

**Eenmalig instellen:**
1. Ga naar [dropbox.com/developers/apps](https://www.dropbox.com/developers/apps) en maak een nieuwe app aan.
   - Kies **Scoped access**.
   - Kies **App folder** (dan krijgt de app alleen toegang tot zijn eigen mapje in je Dropbox, niet je hele Dropbox).
   - Geef 'm een naam, bijv. "Horse Nation Stalmanagement".
2. Ga naar het tabblad **Permissions** van je nieuwe app en vink aan: `files.content.write`, `files.content.read` en `files.metadata.read`. Klik op Submit.
3. Ga naar het tabblad **Settings**. Zoek "Redirect URIs" en voeg **exact** je GitHub Pages-adres toe, bijvoorbeeld:
   `https://serena-nova.github.io/HorseNationStablemanager/`
   (precies zoals in de adresbalk staat als je de app open hebt — geen slash te veel of te weinig).
4. Kopieer de **App key** die bovenaan de Settings-pagina staat.
5. Open de app, klik op "Dropbox" (bovenin), plak de App key, klik "Verbind met Dropbox".
   Je logt eenmalig in bij Dropbox en keurt de toegang goed — daarna spring je terug naar de app.

**Daarna:** elke wijziging wordt automatisch (na een paar seconden) naar Dropbox weggeschreven.
Open je de app op een ander apparaat (met dezelfde App key ingevuld en verbonden), dan haalt
die bij het openen automatisch de nieuwste versie op. Er is geen samenvoegen van losse
wijzigingen — de nieuwste versie (hier of op Dropbox) "wint" in zijn geheel.
