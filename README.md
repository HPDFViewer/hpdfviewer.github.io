# hpdfviewer.github.io

Sito pubblico dell'app Android HPDFViewer, servito con GitHub Pages su https://hpdfviewer.github.io

- `index.html` — landing page (italiano), `en/index.html` — landing page (inglese)
- `assets/css/site.css` — stile condiviso; `assets/img/` — icona, screenshot e anteprime social
- `tester.html` — Diventa tester (it + en)
- `privacy.html` — informativa privacy (it + en), indicata in Play Console
- `app-ads.txt` — dichiarazione AdMob (deve stare nella radice del dominio)
- `robots.txt`, `sitemap.xml`, `llms.txt`, `site.webmanifest`, `404.html` — SEO e motori generativi

Sito statico senza build: niente framework, niente font o script di terze parti.

## Da dove arrivano i file

- `privacy.html`, `tester.html`, `app-ads.txt`: sorgente in `distribution/site/` del repo (privato) `HPDFViewer/hpdfviewer`; si copiano qui quando cambiano.
- Icona e screenshot in `assets/img/`: generati da `design/icon/` e `distribution/listings/*/images/` dello stesso repo.
- Landing page: sorgente in questo repo. Le due lingue vanno tenute allineate; quando cambiano le funzioni dell'app aggiornare anche il JSON-LD in testa alle pagine e `llms.txt`.

## Anteprima locale

    python3 -m http.server 8000
