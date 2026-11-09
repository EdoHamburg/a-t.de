# automatische-treppenbeleuchtung.de

Statischer Onepager (Ratgeber), Herausgeber SEQUA Lichttechnik GmbH. Kein Build, kein JavaScript, keine Cookies.

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | Ratgeber mit Styles und strukturierten Daten (schema.org: Organization, WebSite, Article, FAQPage) |
| `impressum.html`, `datenschutz.html` | Rechtstexte (noindex) |
| `llms.txt` | Kurzfassung für KI-Suchen |
| `robots.txt`, `sitemap.xml` | für Suchmaschinen |
| `CNAME` | eigene Domain für GitHub Pages |
| `.nojekyll` | GitHub Pages liefert die Dateien unverändert aus |
| `favicon.svg` | Symbol im Browser-Tab |

## Veröffentlichen mit GitHub Pages

1. Auf GitHub ein öffentliches Repository anlegen, z. B. `EdoHamburg/automatische-treppenbeleuchtung` (GitHub Pages ist im kostenlosen Tarif nur für öffentliche Repositories verfügbar).
2. Alle Dateien in den Branch `main` hochladen, auch `.nojekyll` und `CNAME`.
3. Unter **Settings → Pages**: Source „Deploy from a branch“, Branch `main`, Ordner `/ (root)`.
4. Beim Domain-Anbieter folgende DNS-Einträge setzen:
   - `@` als A-Records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `www` als CNAME auf `edohamburg.github.io`
5. Wenn die Domain erkannt ist, unter **Settings → Pages** „Enforce HTTPS“ aktivieren.
6. Empfehlung: Domain unter **Settings → Pages → Verified domains** bestätigen (TXT-Eintrag), damit niemand anderes sie auf GitHub verwenden kann.

## Nach dem Livegang

1. Domain in der Google Search Console und den Bing Webmaster Tools anmelden, `sitemap.xml` einreichen.
2. Verlinken: aus dem Ratgeber von sequa-licht.de und von lauflicht-treppe.de. Links von beiden Shops geben der neuen Domain das nötige Gewicht.
3. Inhalte pflegen: Preise, Stufenzahlen und Datum (`dateModified` im JSON-LD, `lastmod` in der Sitemap, „Stand“ im Kopf) bei Änderungen anpassen.
