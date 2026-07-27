# The Everything Playlist

Interactive visualizations of a collaborative Spotify playlist — 1,400+ tracks
spanning 1900–2026. Plain HTML/SVG/JS, no libraries, light & dark mode.

**What's on the page**

- Playlist growth over time, split by contributor
- A "mood map" scatter of every track (valence × energy) with genre filters
- Release-decade and tempo histograms
- Top genres and most-added artists
- Average sound of each decade (energy / danceability / valence)
- Playlist superlatives (happiest, saddest, longest, loudest…)
- A searchable, sortable table of every track

## Updating the data

Export the playlist as CSV (e.g. with [Exportify](https://exportify.net/)),
then regenerate `data.js`:

```
node scripts/prep.mjs "path/to/export.csv"
```

## Hosting

It's a static site — `index.html` + `data.js` is all it needs. Works on
GitHub Pages out of the box.
