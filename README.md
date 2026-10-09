# QGIS for Transport & Road Networks: 25 days,

# 20 projects, ready to apply on day 26

##### A step-by-step system built from your uploaded QGIS Training Manual 3. 44 (

##### pages). Each project lists what to read in the manual, which datasets to download,

##### and what to deliver for your portfolio.

###### Straight talk first. 20 projects in 25 days is possible only if projects are small and scoped (about one day each,

###### flagships two). Employers hire for 4 to 6 polished projects, not 20 rough ones. So: finish all 20 quickly, then

###### spend days 24 to 25 polishing your best 6 as the portfolio you actually show. Nobody can guarantee a job in a

###### fixed time, but this plan gives you the strongest possible application pack.

## Daily 8-hour routine (use every day)

```
Time What to do
```
```
1.0 h Read the manual sections listed for the project and follow along with the exercise data. Do the "Try Yourself" tasks.
```
```
0.5 h Download and inspect datasets. Check CRS, missing values and geometry validity.
```
```
4.0 h Build the project on your own data (a European city or region, not the manual's sample data).
```
```
1.5 h Cartography: Print Layout map exported as PDF and PNG (manual 4.1, 4.2).
```
```
1.0 h Write-up: a 150-word README (problem, data, method, result, limits), then commit to GitHub.
```
###### Choose your study area now. Pick 1 main European city (for example Lisbon,

###### Utrecht, Vienna, Ljubljana or Dublin) and reuse it across projects. Data cleaned once

###### saves hours, and the portfolio looks coherent. Pick a second city only for projects 9

###### and 11 if its open data is better.

## Timeline: 26 days

```
Days Phase Projects
```
```
1 to 4 Foundations: data, CRS, cartography, first routes 1 to 4
```
```
5 to 11 Core network analysis: service areas, transit, accessibility 5 to 10
```
```
12 to 19 Advanced analysis, statistics, raster, automation 11 to 17
```
```
20 to 23 Databases, atlas, web delivery, capstone 18 to 20
```
```
24 to 25 Portfolio site, CV, LinkedIn, target firm list, cover letter polish top 6
```
```
26 Start applying (10 to 15 tailored applications a day)
```
## The 20 projects

###### Tap a project to open its manual references, datasets and deliverable.

###### Collapse all

### undefined

#### 1. Setup and clean OSM road network Day 1: https://github.com/CoolatMax/eu-osm-network-cleaner

```
Install QGIS LTR, download your city's roads, fix the CRS, remove junk attributes.
Read in the manual
2.1 to 2.3, 6.1, 9.2.2 (QuickOSM), 3.
Datasets
OSM roads (QuickOSM), GISCO LAU boundary
Deliverable
GeoPackage with clean roads plus a project file
```
#### 2. Road hierarchy cartography Day 2: https://github.com/CoolatMax/eu-road-hierarchy-cartography

```
Classify motorway to residential roads, label lines, build a print-ready map.
Read in the manual
2.4, 3.2.5 (labeling lines), 3.3, 4.1, 4.
Datasets
OSM roads (highway tag)
Deliverable
```

#### 3. Shortest and fastest route analysis Day 3: https://github.com/CoolatMax/eu-network-routing-analysis
```
Route between 5 origin-destination pairs, compare shortest vs fastest.

Read in the manual
6.3.1 to 6.3.4, 18.

Datasets
Clean roads, a few OD points you digitize

Deliverable
Route layer with distance and minutes fields, comparison map
```
#### 4. Speed-limit-aware routing Day 4: https://github.com/CoolatMax/eu-speed-aware-routing
```
Add maxspeed values (fill gaps by road class), route with the speed field.

Read in the manual
6.3.5, 18.11 (vector calculator)

Datasets
OSM maxspeed tag, national speed rules

Deliverable
Before/after map showing the route changing
```
#### 5. Walking catchments around stops Day 5: https://github.com/CoolatMax/eu-pedestrian-network-catchments
```
Service areas of 250, 500 and 800 m on the network, not straight-line buffers.

Read in the manual
6.3.6, 6.2.6 (distance buffers)

Datasets
OSM stops or GTFS stops, walkable network

Deliverable
Catchment map; compare network vs buffer area
```
#### 6. GTFS transit stop and service frequency map Day 6: https://github.com/CoolatMax/eu-gtfs-transit-frequency
```
Load GTFS stops and trips, count departures per stop in the morning peak.

Read in the manual
2.2, 3.3, 6.2 (join and count)

Datasets
City GTFS feed (stops.txt, stop_times.txt, trips.txt)

Deliverable
Stop-level frequency map plus summary table
```
#### 7. Population served by transit Day 7: https://github.com/CoolatMax/eu-transit-population-coverage
```
Overlay catchments with the population grid, find who is outside good coverage.

Read in the manual
6.2.8 (overlap), 3.3, 8.

Datasets
GEOSTAT 1 km grid or GHSL, catchments from project 5

Deliverable
Percent of population within 500 m, gap map
```
#### 8. Flagship: 15-minute city accessibility Days 8 to 9: https://github.com/CoolatMax/eu-15min-city-accessibility
```
Service areas by walk time to groceries, schools, clinics, parks, transit; score each
area.

Read in the manual
6.3.6, 6.3.4 (speed 4 km/h), 6.2, 18.

Datasets
OSM POIs, roads, population grid

Deliverable
Accessibility score map and a 1-page findings note
```
#### 9. Road collision hotspots Day 10: 
```
Map collisions, create a density surface, rank dangerous road segments.

Read in the manual
6.4, 18.14 (heatmap), 3.

Datasets
National collision records, OSM roads

Deliverable
Hotspot map and top-10 segment table
```
#### 10. Nearest facility and coverage Day 11
```
Which hospitals or fire stations serve each area in X minutes; find the underserved.

Read in the manual
6.3.6, 6.4.4 (nearest neighbour), 6.

Datasets
OSM hospitals or fire stations, roads, grid

Deliverable
Coverage gap map
```
#### 11. Traffic count interpolation Day 12
```
Estimate traffic across a network from sample counters.

Read in the manual
6.4.7, 6.4.8, 18.22, 18.

Datasets
City or national traffic counts

Deliverable
Interpolated surface plus method comparison
```
#### 12. Cycle network gap analysis Day 13
```
Find missing links between cycle lanes, edit and digitize proposed links.

Read in the manual
5.1, 5.3, 6.

Datasets
OSM cycleways, roads, schools, workplaces

Deliverable
Existing vs proposed network map
```
#### 13. Network topology and QA report Day 14
```
Detect dead ends, disconnected islands and overlaps, then fix them.

Read in the manual
5.2 (topology checker), 6.

Datasets
OSM roads

Deliverable
Before/after error counts and a QA log
```
#### 14. Flagship: automated routing model Days 15 to 16
```
Wrap routing and service-area steps into a reusable Model Designer workflow with
batch runs.

Read in the manual
18.17 to 18.21, 18.24 to 18.

Datasets
Outputs of projects 3, 5, 10

Deliverable
Saved .model3 plus a run on 3 cities or 3 stop sets
```
#### 15. EV charging site suitability Day 17
```
Score locations by road class, distance to existing chargers and population.

Read in the manual
6.2, 7.1, 8.2, 18.

Datasets
OSM charging stations or Open Charge Map, roads, grid

Deliverable
Ranked candidate sites map
```
#### 16. Road corridor slope analysis Day 18
```
Slope along a proposed road or cycle corridor from a DEM.
**Read in the manual**
Read in the manual
7.3, 18.15, 8.
Datasets
Copernicus DEM, OSM roads
Deliverable
Slope classes map and corridor profile
```
#### 17. Highway noise exposure Day 19

```
Buffer major roads, overlay with residential areas and count affected people.
Read in the manual
6.2, 3.
Datasets
OSM roads, noise maps, population grid
Deliverable
Exposure map and table
```
#### 18. Safe walking routes to schools Day 20

```
Distance from schools along roads, flag crossings of major roads, rank schools.
Read in the manual
6.2.6, 6.2.7, 6.
Datasets
OSM schools, roads, collisions
Deliverable
School ranking and map
```
#### 19. PostGIS road network database Day 21

```
Load the network into PostGIS and run spatial SQL from QGIS DB Manager.
Read in the manual
15.1 to 15.4, 16.1 to 16.4, 17.
Datasets
Your cleaned roads and POIs
Deliverable
SQL script, documented schema
```
#### 20. Capstone: transport accessibility atlas Days 22 to 23
```
Combine projects into a multi-page atlas for one city and publish web layers.

Read in the manual
14.6, 4.2, 10.1, 10.2, 9.2.1
Datasets
All previous outputs
Deliverable
Atlas PDF, short case study, GitHub repo
```

## Master dataset list

| Datasets | Use | Where to get it |
|----------|-----|-----------------|
| OpenStreetMap roads, paths, cycleways, POIs, charging stations| Almost every project| QGIS QuickOSM plugin (manual 9.2.2) or Geofabrik regional extracts|
| Administrative boundaries (NUTS, LAU)| Study area, clipping, joins| Eurostat GISCO|
| Population grid 1 km (GEOSTAT 2021)| Population served, accessibility | Eurostat GISCO; alternative: JRC GHSL population grid|
| GTFS feed (stops, routes, timetables) | Transit projects | Your city or country's national access point, Mobility Database, or Transitland |
| Road collision records | Safety hotspots | UK DfT STATS19, France BAAC (data.gouv.fr), Germany Unfallatlas, or your city's open data portal |
| Traffic counts | Interpolation | UK DfT road traffic counts, Paris, Madrid, Berlin, Barcelona open data portals |
| Elevation (DEM) | Slope, corridors | Copernicus DEM or EU-DEM (check current availability on the Copernicus site) |
| Corine Land Cover, Urban Atlas | Land-use context, suitability | Copernicus Land Monitoring Service |
| Noise maps | Exposure | European Environment Agency or national noise portals |
| Manual exercise data (network.qgz, training data) |Follow-along practice | Download from the QGIS training manual documentation page |

#### Licences and download links change. Open each portal, confirm the licence allows portfolio use, and keep a "data sources" line in every README.

## Does the manual match these projects?

###### Yes, strongly for the core. The manual has a dedicated 6.3 Network Analysis lesson

###### (shortest path point to point, fastest path, custom speed, speed-limit field, service

###### area from layer), plus 6.2 Vector Analysis , 6.4 Spatial Statistics , the modeler

###### chapter, atlas and database chapters. Roughly 40 percent of the manual is directly

###### useful for you.

|Manual module	|Relevance	|Projects|
|---------------|-----------|--------|
|2 Basic map, 3 Classifying vector data, 4 Layouts|	High	|1, 2, all map exports|
|5.2 Feature topology, 5.3 Forms (oneway checkbox example)|	High|	13, 12|
|6.1 Reprojection	|High	|1, every project|
|6.2 Vector analysis (distance from schools and roads, overlap, extract)|	High|	5 to 7, 10, 17, 18|
|6.3 Network analysis|	High (core)|	3, 4, 5, 8, 10, 14|
|6.4 Spatial statistics (nearest neighbour, interpolation)|	High|	9, 10, 11|
|7 Rasters, 8 Completing the analysis	|Medium	|15, 16|
|9.2 Plugins (QuickMapServices, QuickOSM)|	High|	1, 20|
|10 Online resources (WMS, WFS)	|Medium|	1, 20|
|14.2 Georeferencing, 14.6 Atlas|	Medium (skip the rest of forestry)|	20|
|15 to 17 PostgreSQL, PostGIS, spatial databases in QGIS|	Medium|	19|
|18 Processing: modeler, batch, interpolation, vector calculator|	High|	11, 14, 20|
|11 QGIS Server, 12 GRASS, 14 forestry, 19 contributing|	Low | skip	none|

###### Gaps the manual does not cover. I found no mention of GTFS or isochrone tools, and no PyQGIS scripting.

###### QuickOSM is covered, but only briefly. Fill these gaps yourself: GTFS stop and route files can be loaded as

###### delimited text and processed in QGIS (project 6), and Python is optional extra credit, not needed for this plan.

###### Boutique firms often value a little PyQGIS or PostGIS, so if you finish early, add 2 hours of each.

## Days 24 to 26: turn projects into interviews

###### Day 24: pick your best 6 (suggested: 5, 7, 8, 9, 14, 20). Re-export their maps, tidy the READMEs, and publish a one-

###### page portfolio (GitHub Pages or a Notion page) with a PNG and 3 lines per project.

###### Day 25: one-page CV with a "Selected projects" block near the top. Update LinkedIn headline: "GIS Analyst |

###### Transport and Road Network Analysis | QGIS". List 40 European boutique GIS, mobility and transport

###### consultancies, found through LinkedIn jobs, EU job boards and company career pages.

###### Day 26: send tailored applications. Name one project relevant to each firm's work in the first two lines of your

###### message.


