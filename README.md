# nzbfast Unraid templates

Community Applications template for [nzbfast](https://github.com/nzbfast/nzbfast),
a speed-focused Usenet (NZB) downloader written in Rust.

## Install (before it appears in Community Applications)

1. Unraid → **Docker** tab → **Add Container**.
2. Set **Template repositories** (Docker tab, bottom of the page) to
   `https://github.com/nzbfast/unraid-templates` and nzbfast then appears
   in the template dropdown, or:
3. Fill in manually: image `nzbfast/nzbfast:latest`, port `6789`, and
   paths for `/config`, `/downloads` and `/watch`.

Open `http://<server>:6789`, add your Usenet server in the Welcome
panel, and you're downloading. For Sonarr/Radarr, set an API key
(container variable `NZBFAST_APIKEY`, or dashboard → Settings) and add
nzbfast as an **SABnzbd** download client pointing at port 6789.

## Support

Issues and questions: https://github.com/nzbfast/nzbfast/issues
