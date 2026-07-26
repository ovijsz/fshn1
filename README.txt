THE COLLECTIVE — Fishing Planet reference site
================================================

WHAT'S IN THIS ZIP
- index.html         the site (Fish + Gear + Maps + Trends sections)
- data.json           the full database, incl. real player catch-report stats
- assets/maps/         16 real in-game map shapes (SVG), matched to their location
- assets/maps_unassigned/  13 more real map shapes we couldn't auto-identify yet

HOW TO RUN IT
This loads data.json with fetch(), so most browsers block it if you just
double-click index.html (file:// pages can't fetch local files). Two ways:

1) Local server (fully offline once loaded — no internet needed for data):
   - Open a terminal in this folder
   - Run:  python3 -m http.server 8000
   - Open: http://localhost:8000

2) Upload the whole folder to any static web host (Netlify, GitHub Pages,
   your own server, etc.) for a normal online site.

WHAT'S NEW THIS ROUND

1) Real in-game map shapes for 16 locations (Texas, Missouri, Colorado, New
   York, North Carolina, Netherlands, Oregon, Florida, Italy, Alberta,
   Louisiana, Michigan, California, Alaska, Peru, Bolivia) replace the
   generic placeholder photo for those maps — and catch-report pins are
   now positioned against the correct shape.

2) 13 more map shapes exist (assets/maps_unassigned/, numbered) but had no
   identifying name embedded in the file, so I couldn't safely match them
   to Brazil / Mississippi / Congo / Ukraine / Japan / Czech Republic /
   Maldives / Germany / Mongolia / Norway / United Kingdom. Open the Maps
   tab and click "Show unassigned map shapes" to browse them (zoomable) —
   if you recognize one, tell me the number + place and I'll wire it in.

3) Zoom & pan on every map: scroll/pinch to zoom, drag to pan, +/-/reset
   buttons in the corner. Works on the place detail map and in the
   unassigned-shapes browser.

4) New Trends tab: game-wide rankings built from ~15,700 real player catch
   reports — top baits, top lures, top lure types, top hooks, most-reported
   fish, and busiest maps (by number of reported catch spots). Click any
   entry to jump to it.

FISH PAGE SECTIONS (matches fp-collective.com's layout)
  Baits -> Most used baits -> Lures -> Most used lures ->
  Most used lure types -> Hooks -> Where to catch
"Most used" and "Hooks" use real "reported N catches" numbers wherever
player data exists; falls back to catalog picks (clearly labeled) if not.

DATA COVERAGE — complete
  fish: 279/279  baits: 126/126  lures: 1324/1324  hooks: 143/143
  lure types: 59/59  maps: 30/30  jigheads: 266/266
  boilies/pellets: 144/144  sinkers: 53/53  keepnets/stringers: 41/41
  catch reports: ~15,700 (covering 277 of 279 fish, all 30 maps)
