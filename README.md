# Startline race data

`races.json` is the race information used by the Startline iPhone app: dates, entry fees, ballot windows,
expo details, sold-out labels, exchange rates and airports.

The app downloads it from https://tyiannis.github.io/startline-data/races.json and only switches to a copy
whose `updated` timestamp is newer and that passes its checks, so a bad upload never breaks the app.

Publish changes from the Startline project with `tools/publish-races.sh` (it validates the file first).
