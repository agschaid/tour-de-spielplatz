
Built with Hugo: https://gohugo.io/

Using the Hugo Story Theme: https://themes.gohugo.io/themes/hugo-story/

# Setup

Install hugo. Needs to be the extended version.

## Develop

Run `hugo server` to see the site at localhost:1313. All changes to the codebase (see "Data Layout") will be reflected there in realtime.

## Deployment

* Run `hugo` to build the site.
* Copy all contents of `public/` (only the contents. Not the folder itself) to the ftp remote (in my case that is calling `mirror -e -P 10 -R <absolute-lokal-path>/tour-de-spielplatz/public .` in an `lftp` session)

# Data Layout

All relevant files for day-to-day editing can be found in the `data/` folder.

* banner.yml -> was ist die Tour-de-Spielplatz?
* spotlight1.yml -> Aktueller Termin: Wann? Wo? Status? wie sieht es dieses mal aus? Absage oder Was?
* spotlight2.yml -> Warum? Was soll das?
* spotlight3.yml -> geplante Termine
* spotlight4.yml -> Nur für Eltern? (nein. für alle)
* spotlight5.yml -> Schlechtwetter (wann und wie sagen wir ab usw)
* spotlight6.yml -> Beeinflussung der Kinder? (wir treten nicht mit grünem Branding auf)
* spotlight7.yml -> Wie kann ich mich einbringen?
* items.yml -> Impressum, Kontakt
