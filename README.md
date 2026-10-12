# ITBuddy Online

Professionele statische startwebsite voor `itbuddyonline.nl`, klaar voor een GitHub-repository en Cloudflare Pages.

## Lokaal bekijken
Open `index.html` in je browser. Alle bestanden zijn statisch.

## Publiceren via GitHub + Cloudflare Pages
1. Maak een nieuwe GitHub-repository en upload de bestanden uit deze map naar de hoofdmap.
2. Open Cloudflare > Workers & Pages > Create > Pages > Connect to Git en koppel de repository.
3. Framework preset: **None**. Build command: leeg laten. Output directory: `/` (of de hoofdmap volgens de actuele Cloudflare-interface).
4. Voeg onder Custom domains `itbuddyonline.nl` toe en volg de DNS-instructies van Cloudflare. Zet HTTPS aan.
5. Test op mobiel en desktop.

## Belangrijk: functionaliteit nog niet live
- **Contactformulier:** configureer in `script.js` de constante `FORM_ENDPOINT` met een HTTPS endpoint van een betrouwbare formulierdienst die POST multipart/form-data en CORS voor het domein ondersteunt. Test de verzending en spambeveiliging. Gebruik geen API-sleutels in de browser.
- **Afspraken:** maak een account bij een boekingsdienst, stel je beschikbaarheid in en vervang de `href` van `#booking-link` door de echte publieke boekings-URL. De huidige mailto-link is een tijdelijke fallback.
- **Zakelijke e-mail:** maak `support@itbuddyonline.nl` aan bij een e-mailprovider en configureer MX/SPF/DKIM/DMARC. Het adres bestaat nog niet automatisch.
- **Juridisch:** vervang `privacy.html` en `voorwaarden.html` met volledige, gecontroleerde teksten. Vul verplichte bedrijfsgegevens in, toets consumentenrechten en btw-vermelding.
- **Prijzen:** €19, €35 en €59 zijn voorgestelde tarieven, nog te bevestigen.
- **Betaling:** nog niet aangesloten; kies pas na inrichting van je bedrijfs- en betaalgegevens een betaalprovider.

Dit is een startversie, geen complete productieklare bedrijfswebsite zolang de bovenstaande stappen openstaan.
