# NWProgress.ca archive

This repository preserves a browser-recorded snapshot of [nwprogress.ca](https://nwprogress.ca/) as a WACZ web archive. The capture was created with [ArchiveWeb.page](https://archiveweb.page/) on October 22, 2026.

## View the archive

Open the [NWProgress.ca archive on GitHub Pages](https://wi-ry.github.io/nwprogress.ca-archive/). The page uses [ReplayWeb.page](https://replayweb.page/) to replay the WACZ in your browser.

The original archive is [`site/nwprogress.wacz`](site/nwprogress.wacz). A replay is a record of the pages and resources captured at the time; it is not a live copy of the website. Pages or content that were not captured may not be available.

## Create your own copy

[ArchiveWeb.page](https://archiveweb.page/) is a browser extension and standalone application for recording web pages as you browse. Its [user guide](https://archiveweb.page/guide) has installation, capture, and archive download instructions.

1. Install ArchiveWeb.page from its website and start a new recording before opening the pages you want to preserve.
2. Browse the site in the recording session. Follow links to the pages you want included, scroll through content that loads as you go, and open important images or documents so they are captured too.
3. Stop the recording and download/export the collection as a **WACZ** file. Keep the original WACZ; ReplayWeb.page can replay it without converting it into ordinary HTML.
4. To publish your own copy using this repository's viewer, replace `site/nwprogress.wacz` with your WACZ file, keeping that filename. Update the capture date in `site/index.html`, then push the change to the `main` branch. The Pages workflow deploys changes under `site/`.

ArchiveWeb.page records what you visit; it is not an unattended crawler for an entire site. For a broad, automated crawl, Webrecorder recommends [Browsertrix](https://browsertrix.com/).

## GitHub Pages deployment

The site is published from the `site/` directory by [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml). Configure the repository's Pages source as **GitHub Actions** before the first deployment. The workflow runs on pushes to `main` that change `site/`, and can also be started manually with `workflow_dispatch`.
