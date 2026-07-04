# dispatcharr-epg-mirror

Mirrors the Rytec UK/Ireland XMLTV guides (`SkyLive` + `SportMovies`) as plain,
decompressed XML on a schedule, so they can be consumed directly as EPG
sources by apps (like Dispatcharr) that don't support `.xz` decompression.

A GitHub Action re-fetches and decompresses both guides every 12 hours and
commits them back to this repo if they changed. Point your EPG source at:

- `https://raw.githubusercontent.com/noodlemctwoodle/dispatcharr-epg-mirror/main/skylive.xml`
- `https://raw.githubusercontent.com/noodlemctwoodle/dispatcharr-epg-mirror/main/sportmovies.xml`

Source data: [Rytec](http://www.xmltvepg.nl/) UK/Ireland XMLTV guides.
