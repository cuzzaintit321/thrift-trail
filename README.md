![Thrift Trail — Find your next good thing](assets/thrift-trail-cover.jpg)

# Thrift Trail

A mobile-friendly thrift-store finder and resale notebook built with HTML, CSS, and JavaScript.

## Features
- Find up to 10 mapped charity/secondhand stores within 50 km, sorted by straight-line distance.
- Original Space Coast store list, search, visit tracking, and Google Maps directions.
- Resale watch list with eBay sold-listing links.
- Find notebook, estimated profit calculator, and JSON backup export.
- Open eBay shortcut (app handling depends on device/browser settings).

## Run
No build or dependencies required. Run `python3 -m http.server 8000` in this folder and open http://localhost:8000. Deploy on HTTPS for device geolocation (localhost is also supported).

## Data and privacy
Location lookup requests go directly to https://overpass-api.de/api/interpreter. Coordinates are not saved by this app. OpenStreetMap coverage may be incomplete; results include mapped charity and secondhand shops and are not guaranteed to be the closest 10 actual thrift stores. Distances are not driving distances. Current store hours are not supplied.

Saved finds, visited stops, and nearby results stay in browser localStorage; there is no account sync. Export finds to keep a backup. Nearby results retain store coordinates, not the user's coordinates.

Fee percentage is an editable planning assumption. Profit estimates exclude tax and travel. Research exact models, condition, authenticity, shipping costs, and recent comparable sales before buying.

## Map data
© OpenStreetMap contributors, available under the Open Database License: https://www.openstreetmap.org/copyright

## GitHub
From this folder, with GitHub CLI authenticated:

```bash
git init
git add .
git commit -m "Initial release of Thrift Trail"
git branch -M main
gh repo create thrift-trail --public --source=. --remote=origin --push
```
