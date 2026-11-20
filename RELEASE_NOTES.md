## Volcano and tsunami API endpoints, snapshot 15 Nov 2026

- 5,280 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 903 services · 52 country codes · 3,371 keyless JSON rows

### Download

- `Volcano_Tsunami_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 5,280 rows, 261.3 kB gzipped (1.6 MB as CSV), SHA-256 `a8db56409e3f59b202d58da9c162661dbbed7e4691d53d0641037627f82dcbee`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Volcano_Tsunami_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Volcano_Tsunami_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 2,399 · Wrap one ArcGIS layer as a get_hazard_zone tool: pass a point as `geometry=lon,lat&geometryType=esriGeometryPoint&spatialRel=esriSpatialRelIntersects` and return the tsunami evacuation, lava-flow or lahar zone it falls in, with a timeout; CKAN, Socrata and OpenDataSoft rows return the zone table without a point filter.
- 📱 App features: 464 · Draw evacuation zones, assembly points and hazard areas on a map card; show the zone a user stands in and the nearest safe area, with the layer date.
- 🧠 Grounding and data pipelines: 280 · Load eruption and tsunami event lists, station lists and model-grid descriptions on a schedule into your own store, so answers about past events and exposure cite a dated source.
- 🧪 Evals and testing: 5,280 · Run your hazard tool against a fixed set of URLs across hosts; check that zone names, volcano names, dates or wave heights parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 69 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 609 class-exercise copies of the same few ArcGIS Online layers (Miami Beach sea level rise, high-risk areas without shelter, flooded areas, sea level rise and storm surge maps) across many organisations, many with a person's name in the title.
- Left out: 4 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 39 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 2 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 6 rows of server information from Mastodon, PeerTube, Lemmy, Nostr and other social network servers (instance documents name the server's contact person).
- Left out: 127 copies of population-distribution and shelter-access layers, many with initials or a person's name added to the title.
- Overlap: 46 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 64 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 166 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 33 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 115 of these URLs are also in 1.3m-government-open-data-apis.
- Overlap: 1 of these URLs is also in 290k-statistics-apis-for-agents.
- Overlap: 64 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 27 of these URLs are also in 24k-maritime-apis-for-agents.
- Overlap: 4 of these URLs are also in 380k-maps-gis-apis-for-agents.
- Overlap: 3,371 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 79 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 5,042 of these URLs are also in 53k-hazards-apis-for-agents.
- Overlap: 7 of these URLs are also in 25k-aviation-apis-for-agents.
- Overlap: 1 of these URLs is also in 12k-parking-apis-for-agents.
- Overlap: 468 of these URLs are also in 10k-earthquake-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Volcano and tsunami API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
