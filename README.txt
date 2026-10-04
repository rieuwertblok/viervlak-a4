VIERVLAK A4 - PWA-STRUCTUUR

Bestanden
- index.html: de volledige app, inclusief registratie van de service worker
- manifest.webmanifest: naam, kleuren, startpagina en app-iconen
- service-worker.js: offline cache en updatebeheer
- offline.html: terugvalpagina wanneer een niet-gecachete pagina offline wordt geopend
- icons/: iconen voor browser, beginscherm en maskable Android-weergave

Lokaal testen
1. Open een terminal in deze map.
2. Start een lokale server, bijvoorbeeld: python -m http.server 8000
3. Open http://localhost:8000
4. Controleer in browserontwikkelaarshulpmiddelen het manifest en de service worker.

Publiceren
- Upload de volledige inhoud van deze map naar één map op een HTTPS-webserver.
- Open daarna de gepubliceerde index.html op de telefoon.
- Android/Chrome: gebruik de installatieoptie van de browser.
- iPhone/Safari: gebruik Deel en vervolgens Zet op beginscherm.

Nieuwe versie publiceren
- Pas CACHE_NAME in service-worker.js aan, bijvoorbeeld van v1 naar v2.
- Upload vervolgens alle gewijzigde bestanden.

Let op
- Open index.html niet rechtstreeks via file://; service workers vereisen HTTPS of localhost.
- Verwijder of hernoem de bestanden niet zonder ook manifest.webmanifest en service-worker.js bij te werken.
