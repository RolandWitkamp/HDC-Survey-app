# Hotel survey: installeren en delen

## 1. Online zetten (GitHub Pages, gratis)
1. Maak een account op github.com en klik op **New repository**. Geef het een naam, bijvoorbeeld `hotel-survey`, en kies **Public** (gratis Pages vereist dat; alleen de code is zichtbaar, nooit de surveys).
2. Klik op **uploading an existing file** en sleep de *inhoud* van deze map erin (index.html, sw.js, manifest.webmanifest, jspdf.umd.min.js, en de mappen fonts en icons). Klik op **Commit changes**.
3. Ga naar **Settings > Pages**, kies bij Source **Deploy from a branch**, branch `main`, map `/ (root)` en klik op **Save**.
4. Na een minuut of twee staat de app op `https://<gebruikersnaam>.github.io/hotel-survey/`.

Wil je het binnen KLM hosten, geef deze map dan aan IT. Het zijn gewone statische bestanden; de enige eis is HTTPS.

## 2. Installeren op iPad of iPhone
1. Open de link in **Safari** (niet in een andere browser).
2. Tik op het deelicoon en kies **Zet op beginscherm**.
3. Open de app één keer via het nieuwe icoon terwijl je online bent. Daarna werkt hij volledig offline.

Gebruik altijd het icoon op het beginscherm. Gegevens van gewone Safari-tabbladen kunnen na een periode zonder gebruik worden gewist, die van beginscherm-apps niet.

## 3. Delen met collega's
Stuur ze de link en deze instructie. Ieder apparaat heeft zijn eigen surveys.
Surveys overdragen: **Instellingen > Alles exporteren**, stuur het bestand door, en de ontvanger kiest **Back-up terugzetten**.

## 4. Updates uitbrengen
1. Pas de bestanden aan en upload ze opnieuw naar dezelfde repository.
2. Verhoog in `sw.js` de regel `const CACHE = 'hotel-survey-v1.0.0'` (bijvoorbeeld naar v1.0.1), en `APP_VERSION` in index.html.
3. Bij de volgende keer openen met verbinding haalt de app de nieuwe versie op. Surveys blijven bewaard.

## 5. Goed om te weten
- Alle surveys staan alleen op het apparaat zelf. Exporteer regelmatig een back-up.
- Delen met PDF en Mail opstellen werken ook offline; de mail wordt verzonden zodra er weer verbinding is.
- Stem met IT af of je deze app met KLM-gegevens mag gebruiken.
