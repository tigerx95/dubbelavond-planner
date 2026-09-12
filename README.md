# Dubbelavond Planner 🎾

Een zelfstandige webtool (één HTML-bestand, geen installatie nodig) om automatisch een baanverdeling te maken voor de wekelijkse tennisclub-dubbelavond, op basis van de ledenlijst en de Google Forms-inschrijvingen.

## Functionaliteiten
- Upload van ledenlijst (CSV) en inschrijvingen (Excel-export van Google Forms, CSV, of live koppeling met de Google Sheet)
- Automatische baanverdeling: matcht spelers op niveau, houdt rekening met man/vrouw-balans (nooit 2 mannen tegen 2 vrouwen), en probeert opmerkingen zoals "graag met X spelen" te honoreren
- Enkelspel-detectie bij een tekort van exact 2 spelers (indien beide spelers dit aangaven in de ledenlijst), met mogelijkheid om dit ook handmatig per baan aan/uit te zetten
- Volledig bewerkbaar nadien: spelers naar een specifieke plaats slepen, hele banen wisselen, spelers verwijderen (afmeldingen), handmatig invallers toevoegen
- Exporteert een nette afbeelding (PNG) klaar om te delen via WhatsApp
- Bewaart automatisch een geschiedenis van elke gedownloade versie, herlaadbaar binnen de app

## Gebruik
Open `index.html` in een browser (Chrome, Firefox, Edge, Safari) — lokaal of via een gehoste versie (zie hieronder). Er is geen server, database of installatie nodig; alles draait client-side in de browser.

## Hosten via GitHub Pages
Deze repo is zo opgezet dat `index.html` in de hoofdmap staat, zodat GitHub Pages de tool direct als website kan tonen. Zie de instructies die je ontvangen hebt bij het opzetten van deze repo, of ga naar **Settings → Pages** in dit GitHub-project.

## Technische opmerking
Eén enkel HTML-bestand met ingebouwde CSS en JavaScript — geen build-stap, geen dependencies om te installeren. Gebruikt de volgende externe bibliotheken via CDN: PapaParse (CSV), SheetJS (Excel) en html2canvas (afbeelding-export).
