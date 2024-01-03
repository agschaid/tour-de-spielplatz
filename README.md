
Built with Hugo: https://gohugo.io/

Using the Hugo Story Theme: https://themes.gohugo.io/themes/hugo-story/

# Setup

Install hugo. Needs to be the extended version.

## With git

Usually you should get this repo with git (needed for pushing back changes that you have made)

* Run `git clone git@github.com:agschaid/tour-de-spielplatz.git` to get this repo.
* In the `tour-de-spielplatz` folder run `git submodule update --init --recursive` to download the hugo-story theme.

## Without git

If you don't know what git is (but still need to make changes to the homepage) get this repo the following way:

* download this repo as a zip file (the green `Code` button above -> "Download ZIP") and unpack it in an convenient location.
* download the the hugo-story theme in the same way from https://github.com/caressofsteel/hugo-story and copy the contents of the unziped folder to `tour-de-spielplatz/themes/hugo-story/`.

Changes that you make now can **NOT** be pushed back to the central repo.

## Development

Run `hugo server` to see the site in your browser at http://localhost:1313 . All changes to the codebase (see "Data Layout") will be reflected there in realtime (as long as the server is running).

## Deployment

* Run `hugo` to build the site und store all artifacts in `public/`.
* Copy all contents of `public/` (only the contents. Not the folder itself) to the ftp remote (in my case that is calling `mirror -e -P 10 -R <absolute-lokal-path>/tour-de-spielplatz/public .` in an `lftp` session. Choose your own poison)

# Data Layout

All relevant files for day-to-day editing can be found in the `data/` folder.

ONLY edit the html that can be found under the `content` key of the respective elements unless (you think) you know what you are doing.

* banner.yml -> was ist die Tour-de-Spielplatz?
* spotlight1.yml -> Aktueller Termin: Wann? Wo? Status? wie sieht es dieses mal aus? Absage oder Was?
* spotlight2.yml -> Warum? Was soll das?
* spotlight3.yml -> geplante Termine
* spotlight4.yml -> Nur für Eltern? (nein. für alle)
* spotlight5.yml -> Schlechtwetter (wann und wie sagen wir ab usw)
* spotlight6.yml -> Beeinflussung der Kinder? (wir treten nicht mit grünem Branding auf)
* spotlight7.yml -> Wie kann ich mich einbringen?
* items.yml -> Impressum, Kontakt

All relevant source images can be found under `static/images`.
