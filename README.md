# OSM and GIS resources that I like.

### OpenStreetMap Metrics and Visualization

(visualizing changesets in the last 7 days)
http://resultmaps.neis-one.org/osm-changesets?comment=hms_gw#12/-17.8389/31.0759
http://neis-one.org/

(looking at history and changesets of features)
On OpenStreetMap.org use the query button to view node history and changesets. This can be useful in telling what source was used during tracing.

#### live edits
http://osmlab.github.io/show-me-the-way/

##### Show me the Way
http://live.openstreetmap.fr/

### OSM Analytics
#### http://osm-analytics.org/

### ITO World Maps
#### http://product.itoworld.com/map/

### OpenStreetMap Stats
#### https://osmstats.stevecoast.com/dashboard/us/track

## Validation

### OpenStreetMap Improve
http://improveosm.org

### iOSMAnalyzer
#### https://github.com/zehpunktbarron/iOSMAnalyzer

### Map Roulette
#### http://www.maproulette.org/

### OSM BattleGrid
#### https://openstreetmap.us/2013/09/battlegrid/

### Routing
Using osm2pgrouting
https://www.hotosm.org/updates/using-open-source-tools-to-solve-routing-issues-for-solid-waste-collection-in-dar-es-salaam/
This was an interesting concept, used to improve OSM data in the US from the Tiger import
What if we introduced a similiar concept but using high-res imagery to suggest areas to fix?

## OSM Who's Around Me?
### http://neis-one.org/2013/01/
It would be nice if it was calculated by nodes instead of changesets, and if it could have an option to go back further than 6 months

## How did you contribute to OpenStreetMap?
### http://hdyc.neis-one.org/
Provides user stats

#### MapCompare: view two basemaps at once
##### http://tools.geofabrik.de/mc/

### 50NorthSpatial (GIS Blog from Ukraine)
http://www.50northspatial.org

### Overpass Turbo   http://overpass-turbo.eu/

http://overpass-turbo.eu/

query: IDP camps in Kathmandu (http://overpass-turbo.eu/s/9bw)

/*
idp camps kathmandu
*/
[out:xml][timeout:120];
way[~"idp:"~"spontaneous_camp"]({{bbox}});
// print results
out meta;
>;
out meta;

query: Severely damaged Areas

http://overpass-turbo.eu/s/afO

/*
Severely damaged areas kathmandu
*/
[out:xml][timeout:120];
way[landuse="brownfield"]({{bbox}});
// print results
out meta;
>;
out meta;

### Overpass turbo query by date
https://gist.github.com/aawiseman/ec55286c86d4612bc393

Information on OSM tags:
https://taginfo.openstreetmap.org/

### OpenStreetMap Analyzing Imagery

now built into iD editor (use 'Ctrl+Shift+B' shortcut to bring up panel)(https://github.com/openstreetmap/iD/issues/2492)

These previous services are down:

Bing Imagery Analyzer (Let's you browse dates of Bing Imagery)
http://mvexel.dev.openstreetmap.org/bing/

Ant Bing Imagery Analyzer (Let's you see which areas have high-res Imagery)
http://ant.dev.openstreetmap.org/bingimageanalyzer/

### OpenStreetMap Extracting Data
resources how to export OpenStreetMap data

Mapzen Metro Extracts (City-sized parts of the OpenStreetMap database, served up weekly.)
https://mapzen.com/metro-extracts/
https://mapzen.com/blog/metro-extracts-101

GeoFabrik (OSM extractions)
http://www.geofabrik.de/

Downloading OSM coastlines and generalized data:
http://openstreetmapdata.com/

#### HOT export tool
##### http://export.hotosm.org/en/

#### QGIS

#### ERSI ARCGIS OSM toolbar

### OpenStreetMap Training

Blake Girardot's JOSM training video
https://www.youtube.com/watch?v=GOfTJ3QDQB4&feature=youtu.be

Jim McAndrew's Leaflet tutorial
http://loc8.us/maptime2015/#/

### OSM Routing:

### OSM Routing
#### http://k1z.blog.uni-heidelberg.de/2015/07/17/openrouteservice-update/

https://github.com/Project-OSRM/osrm-backend

## Mapnificent shows you the area you can reach with public transport from any point in a given time.
http://www.mapnificent.net/washington/

#### OSM cyling:

Route planning:
http://cycle.travel/map
http://www.opencyclemap.org/


## Vector Tiles

Mapzen Vector Tile Services
https://github.com/mapzen/vector-datasource/wiki/Mapzen-Vector-Tile-Service

http://mike.teczno.com/notes/gl-solar-webgl-openstreetmap.html

http://www.mkgeomatics.com/wordpress/?p=389

http://mike.teczno.com/notes/postgreslessness-mapnik-vectiles.html

https://www.mapbox.com/mapbox-gl/
https://www.mapbox.com/mapbox-gl-style-spec/

Creation of VectorTiles: tilelive, tessera, mapbox studio

### Understanding Vector Tiles

generating vector tiles live from PostGIS:
chubbs: https://github.com/spatialdev/PGRestAPI

displaying vector tiles in leaflet:
https://github.com/SpatialServer/Leaflet.MapboxVectorTile

Mapbox vector tiles implementations: https://github.com/mapbox/vector-tile-spec/wiki/Implementations

OSM 2 vector tiles:
https://github.com/systemed/tilemaker

Styling vector tiles:
-Mapbox Studio
-what else?

Good question on self-hosting vector tiles:
http://gis.stackexchange.com/questions/125037/self-hosting-mapbox-vector-tiles

hosting vector tiles:
https://github.com/mapbox/tilelive.js

## geospatial_app_feedback
suggestions and feedback for a variety of geospatial applications

#### Digital Globe EVWHS

-Being able to download the shapefile of the imagery tile boundaries and extent before having to upload the whole strip to my library and download it. (fixed!!)
-Being able to view and download imagery with false-color bands.   
-Being able to upload or draw my own bounding box and search of imagery that is within it

-add measurement tool

#### geojson.io

-be able to drag and drop files to upload
-be able to upload multiple files in a batch

#### HOT Tasking Manager

#### ID Editor

-draw complex polygons

#### UMap

-add measurement tool

#### CartoDB

#### OpenStreetMap.org

-needs smart search (look into http://wiki.openstreetmap.org/wiki/Nominatim and TagInfo)

## Satellite Imagery

### Machine Learning and Imagery

#### Google Machine Learning: https://www.engadget.com/2016/09/29/google-opens-up-its-machine-learning-tricks-to-all/

#### SpaceNet on AWS: https://aws.amazon.com/public-data-sets/spacenet/ 
SpaceNet is a corpus of commercial satellite imagery and labeled training data being made available at no cost to the public 

## What I want to read related to GIS

Theoretical geography,
William Bunge 1928- 1966
Available at George Mason University Fenwick Stacks (G70.B8 T5 )

-good summary by Goodchild (http://www.geog.ucsb.edu/~good/papers/450.pdf)

https://www.techchange.org/online-courses/mhealth-mobile-phones-for-public-health/

https://www.techchange.org/online-courses/mobiles-for-international-development/

#### More on geospatial data standards for features and attribution
-DGIWG
-OpenStreetMap
-WorldWide Geography Working group

#### Compare OSMIUM and OSMOSIS

### osm4j is a Java library for working with OpenStreetMap data. 
http://jaryard.com/projects/osm4j/

## Conflation

-HOOTENANNY: WEB ENABELED GEOSPATIAL VECTOR-DATA CONFLATION AND MAP GENERATION

### Cygnus
### http://www.openstreetmap.org/user/mvexel/diary/36746

## QGIS

Programmer's Guide
http://pyqgis.org/book/contents/

OpenTripPlanner:
http://www.opentripplanner.org


## What I'm looking for

##### A smarter geospatial search that what is on OpenStreetMap.org
-how can I search for objects in a place, or within the user's view? Ex. 'indoor pools in Washington D.C'

##### NGA stuff:
###### Map of The World:
-http://trajectorymagazine.com/got-geoint/item/1647-nga-launches-map-of-the-world.html
-https://www1.nga.mil/MediaRoom/LeadingStories/Pages/WashingtonMapSociety.aspx
-http://www.afcea.org/content/?q=node/13903
-http://www.nextgov.com/cloud-computing/2014/12/first-intelligence-agency-host-app-amazons-c2s-cloud/100851/

NYC Historical Maps:
http://spacetime.nypl.org/

NYPL Map Warper:
http://dev.maps.nypl.org/warper/
http://mapwarper.net/

### Transportation Mobile App

got ideas from reading: Crowdsourcing and Its Application to Transportation Data Collection and Management
Aditi Misra, Aaron Gooze, Kari Watkins, Mariam Asad, and Christopher A. Le Dantec

Look into Tirimisu Transit app (http://www.tiramisutransit.com/t/livemap) and OneBusAway (http://onebusaway.org/) app and see if a app that employs similiar ideas could work for DC

### NextBus
#### http://nextbus.cubic.com/About/How-NextBus-Works
#### NextBus predictions inaccurate:  http://www.sfexaminer.com/nextbus-muni-predictions-inaccurate-during-commute-hours-almost-half-the-time-study-says/?utm_campaign=CartoDB&utm_content=25048299&utm_medium=social&utm_source=twitter 

### Mobile city Fix-it apps
http://www.codeforamerica.org/blog/2011/02/23/boston-citizens-connected/
http://www.citysdk.eu/citysdk-challenge-build-best-cross-city-smart-participation-app-win-3000-euros/
http://www.chicagoworksapp.com/
http://www.open311.org/
https://github.com/codeforamerica/open311dashboard

actually, OneBusAway is already open to partnering with Tirimisu and a beta has already been launched in Washington D.C.
https://github.com/OneBusAway/onebusaway/wiki/OneBusAway-Deployments
http://mobilitylab.org/2013/10/25/onebusaway-demo-app-offers-best-transit-info-yet-for-dc-users/

## GIS on Mobiles:

http://mousebird.github.io/WhirlyGlobe/

## Offline Mapping Apps

### OSM Mobile Apps:

#### Maps.me

#### OsmAnd




## Other GIS things

##### I'm trying to remember an online mapping app. You could upload maps and georeference them online. There was also a time component to it as well. I think it was part of a thesis or dissertation. It is not OldMaps Online, Map Warp, or MetaCarta's MapRectifier.

#### Digital Gazatteer
https://thinkwhere.wordpress.com/2015/01/19/a-digital-gazetteer-of-places-for-the-library-of-congress-and-the-nypl/

#### Geo-Visualization
http://www.imagico.de/

#### TimeMapper
http://timemapper.okfnlabs.org/

## Surveys

Field Papers

OpenMapKit

Survey123

### Peace Corps Community Training Slides
#### https://docs.google.com/presentation/d/1j-Q-_GZNbLqhek52ZHmb8ZrowT8YsqYD5C68MBd0Gnk/edit#slide=id.gc347858b8_0_102

ODK
#### https://opendatakit.org/

First Mile Geo
https://www.firstmilegeo.com/

## Open data

OpenAddresses
https://openaddresses.io/

OpenTraffic
http://opentraffic.io/

OpenTripPlanner
http://www.opentripplanner.org/

National Geospatial Advisory Committee, National Address Database:
http://www.fgdc.gov/ngac/meetings/december-2012/NGAC%20National%20Address%20Database%20Paper.pdf

GFTS:
http://blog.openplans.org/2012/08/the-openplans-guide-to-gtfs-data/

## Open data Platforms

Koordinates
https://koordinates.com

## GPS

http://gracegao.ae.illinois.edu/publications.html

## Social Media: Geo-locating messages

Samuel Lee Toepke, R. Scott Starsman
Population Distribution Estimation of an Urban Area Using Crowd Sourced Data for Disaster Response
http://iscram2015.uia.no/?p=1978

Penn State
http://www.geovista.psu.edu/

SMART   HDMS @SDSU
http://vision.sdsu.edu/hdma/smart

## OSM Scholarly Articles

Recent Developments and Future Trends in Volunteered
Geographic Information Research: The Case of OpenStreetMap
Pascal Neis 1,* and Dennis Zielstra 2

Assessing the Completeness of Bicycle Trail and Lane Features in OpenStreetMap for the
United States
Hartwig H. Hochmair1*, Dennis Zielstra1
, Pascal Neis2

Assessing the Effect of Data Imports on the Completeness
of OpenStreetMap – A United States Case Study
Dennis Zielstra,* Hartwig H. Hochmair* and Pascal Neis†

The Street Network Evolution of Crowdsourced Maps:
OpenStreetMap in Germany 2007–2011
Pascal Neis 1,*, Dennis Zielstra 2
and Alexander Zipf 1

Accessing the history of objects in OpenStreetMap
https://scholar.google.com/citations?view_op=view_citation&hl=en&user=wVs_9twAAAAJ&citation_for_view=wVs_9twAAAAJ:Y0pCki6q_DkC
Peter Mooney, Padraig Corcoran

The Annotation Process in OpenStreetMap
http://onlinelibrary.wiley.com/doi/10.1111/j.1467-9671.2012.01306.x/abstract
Peter Mooney, Padraig Corcoran

## Map Stories
Geo-report:
https://github.com/crowdcover/geo-report

ESRI Story Maps:
http://storymaps.arcgis.com/en/

### examples:
Rohingya Story from UNHCR: https://unhcr.maps.arcgis.com/apps/Cascade/index.html?appid=5fdca0f47f1a46498002f39894fcd26f


Odessey.js:
http://blog.cartodb.com/odyssey-js-new-open-source-tool-to-weave-interactive/

### USGIF Publishes GEOINT Essential Body of Knowledge
http://usgif.org/news/630-usgif-publishes-geoint-essential-body-of-knowledge

### geospatial games
#### http://www.cnet.com/news/ingress-the-friendliest-turf-war-on-earth/
 
##Drones
### http://drones.newamerica.org/
### http://drones.newamerica.org/primer/

## Big Data

### Read up on Apache Spark

## Platforms

### DHIS2
#### https://www.dhis2.org/

## OSM data quality

#### good exerpts from "Updating digital elevation models via change detection and fusion of human and remote sensor data in urban environments" p.156

Quality of OSM mainly depends on the contributer, both on their accuracy and their experience. In general, the more mappers that are active in an areas the better the quality is supposed to be. Moreover some analysis resulted in higher coverage of data in urban areas. However, it was showed that further factors such as income can also influence the results. Therefore, it is not possible to make a universal statemetn about data covergage regarding urban or rural areas. Furthermore a study had a closer look at the spatio-temporal develpment of OSM contributions. For the specific situation of the city of Heidelberg, their prediction using cellular automata revealed thap-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-ep-win-3000-et the density of contributions is linked to a certain land use type.

#### http://wiki.openstreetmap.org/wiki/Completeness

### matching gps trajectories to street segments
#### http://k1z.blog.uni-heidelberg.de/2015/08/10/matching-gps-trajectories-to-street-segments-an-open-source-implementation/

## OSM data fustion

### OSM and Lidar
#### "Updating digital elevation models via change detection and fusion of human and remote sensor data in urban environments"

### create.io
#### good for finding land parcels and information on a map

## Collaborative GIS

### GeoCollaborate
#### http://www.geocollaborate.com/ 

## Education

### ZOMBIE-BASED GEOGRAPHY
#### http://www.zombiebased.com/

## Natural Earth
### http://www.naturalearthdata.com/
#### Natural Earth is a public domain map dataset available at 1:10m, 1:50m, and 1:110 million scales. Featuring tightly integrated vector and raster data

## Admin Areas 

### GDAM: database of Global Adminstrative Areas
#### http://www.gadm.org/

## Good Articles

### GeoSpatial: An Open Source Microcosm by Paul Ramsey
### http://timreview.ca/node/234

#### THE CHANGING GEOSPATIAL LANDSCAPE A Second Look
#### A	Report	of	the	National	Geospatial	Advisory	Committee, December	2015
#### https://www.fgdc.gov/ngac/meetings/december-2015/the-changing-geospatial-landscape-second-look.pdf

## Flood Mapping

### MapBox Flood Map
#### https://www.mapbox.com/blog/chennai-flood-map/

## Remote Sensing & Satellite Imagery

### Google Earth Engine
#### https://earthengine.google.com/

## HighRes DEM
### http://www.geo-airbusds.com/worlddem/

#### Radiance and Relectance
#### http://www.exelisvis.com/Home/NewsUpdates/TabId/170/ArtMID/735/ArticleID/13592/Digital-Number-Radiance-and-Reflectance.aspx
#### http://www.seos-project.eu/modules/remotesensing/remotesensing-c01-p05.html

### Ways to support mappers in other countries
#### http://exchanges.state.gov/non-us/program/community-solutions

## Flood Modeling & Hydrography

### OpenSource tools to calculate Watersheds
#### https://grasswiki.osgeo.org/wiki/Creating_watersheds 

### Crayfish QGIS plugin: 
The Crayfish plugin aspires to be a complete set of pre- and post-processing tools for hydraulic modellers using TUFLOW, BASEMENT, ISIS 2D, Hydro_AS 2D, AnuGA and other modelling packages.
#### http://www.lutraconsulting.co.uk/products/crayfish/wiki

## Other Crowdsourcing platforms

### http://www.inaturalist.org/
### crowdsourcing observations in nature

### High-res change detection?
#### what is out ther

### CNS Project on Crowdsourced Imagery Analysis 
#### http://www.geo4nonpro.org/#!about/cluw

### OpenStreetMap as Infrastructure: Mikel Maron (SOTMUS 2014)
https://www.youtube.com/watch?v=ztXQiy0iStI#t=17.500689

## Mapillary
### Mapillary Guide in OSM from MapBox: https://www.mapbox.com/blog/get-started-mapillary/

### POSM OSM Replay Tool post: https://hi.stamen.com/merging-offline-edits-with-the-posm-replay-tool-2f39a4410d2a#.gaajvzett

### For Printing Maps: http://maperitive.net/

### For organizing projects: https://help.mapillary.com/hc/en-us/articles/360023629331-Capture-Projects-getting-started

## Education

### MapSchool.io
http://mapschool.io/

### MapHubs: https://maphubs.com/
Tool for Sharing and Finding Maps

## Story Maps

https://github.com/JackDougherty/leaflet-storymap

# GeoNode

Hypermap

hh.worldmap.harvard.edu

hypersearch.cga.terranodo.io

http://drm.moha.gov.np/  (nepal geonode)

http://geonode.geocenter.io/

## Other Crowd Sourcing Platforms

http://www.globalxplorer.org/

https://www.tomnod.com/

### URISA
URISA is the founding member of the GIS Certification Institute (https://www.gisci.org/) and GIS Corps
http://www.urisa.org/ 

### Crowdsourcing and Citizen Science Bill
https://www.congress.gov/bill/114th-congress/senate-bill/3084/text#toc-idc675e4e0-f615-4d4a-8ad5-b9cc94092dde

### State of Satellites
http://landscape.satsummit.io/

### Tufts Student GIS Expo Explorer
http://streams-dev.it.tufts.edu/#/dashboard

#### GDAL and links:
https://medium.com/planet-stories/a-gentle-introduction-to-gdal-part-1-a3253eb96082

### MIT Senseable Lab
http://senseable.mit.edu/

### Zee Maps
mapping lists
https://www.zeemaps.com/

### OSM Newsletter
https://osmnewsletter.org/

## OSM Imports
https://wiki.openstreetmap.org/wiki/Microsoft_Building_Footprint_Data

## FB imports
https://lists.openstreetmap.org/pipermail/imports/2017-March/004840.html
https://wiki.openstreetmap.org/wiki/AI-Assisted_Road_Tracing

### OpenGeoPortal
http://data.opengeoportal.org/
They also use SOLR and spatial search

### Displaying other projections in MapBox GL
https://developmentseed.org/blog/2016/12/15/dirty-reprojectors/

### ogr2ogr: convert data between GeoJSON, PostGIS, and Esri Shapefile
https://morphocode.com/using-ogr2ogr-convert-data-formats-geojson-postgis-esri-geodatabase-shapefiles/

### Global Urban Footprint
https://www.technologyreview.com/s/608156/global-urban-footprint-revealed-in-unprecedented-resolution/

### OSM Philly Food Map
Case Study publication (Sterling Quinn) http://www.tandfonline.com.mutex.gmu.edu/doi/abs/10.1080/00330124.2015.1065547
https://www.geovista.psu.edu/phillyfood/

### LandCover: CORINE Land Cover
http://land.copernicus.eu/pan-european/corine-land-cover

### Participatory GIS Training Kit
http://pgis-tk-en.cta.int/videos/index.html

### Participatory Three-dimensional Modelling PDF
http://www.iapad.org/wp-content/uploads/2015/07/p3dm_english_web.pdf

### Rasterfoundry
Raster Foundry is an earth observation analysis tool to find, combine and analyze earth imagery at any scale, and share it on the web. 
https://www.rasterfoundry.com/

## Azavea
We have been stretching the possibilities of geospatial technology to enable our clients to answer complex questions in a wide range of domains: urban ecosystems, water, infrastructure planning, economic development, public transit, elections, public safety, energy, and cultural resources management, to name a few.
https://www.azavea.com/work/

### OpenLocate
collecting location data on mobile
#### https://blog.safegraph.com/introducing-openlocate-the-open-source-location-sdk-f5c5d2739a48


https://blog.insightdatascience.com/deep-learning-for-disaster-recovery-45c8cd174d7a

### How to commit to OSM-Carto
http://www.openstreetmap.org/user/SomeoneElse/diary/43041

#### You can find a geo bounding box easy with this boundng box tool:
https://boundingbox.klokantech.com/

#### How to Serve Vector Map Tiles Locally with Tegola
https://docs.google.com/presentation/d/1UvoS-R8UBLcKB3CFNBgCw5Gi0EBLAeknGIvzbZ04GQ0/edit#slide=id.g372f61354a_0_10

### Kepler.gl
https://uber.github.io/kepler.gl/#/
http://vis.academy/#/

### Geospatial Database and algorithm considerations 

#### PostgreSQL vs Pandas
https://medium.com/carwow-product-engineering/sql-vs-pandas-how-to-balance-tasks-between-server-and-client-side-9e2f6c95677
#### database benchmarks
https://github.com/szilard/benchm-databases
#### A dive in spatial seach algorithms
https://blog.mapbox.com/a-dive-into-spatial-search-algorithms-ebd0c5e39d2a
#### Geospatial Operations at Scale with Dask and Geopandas
https://r-shekhar.github.io/posts/spatial-joins-geopandas-dask.html

### node js rest API with Express Tutorial
https://medium.com/@jeffandersen/building-a-node-js-rest-api-with-express-46b0901f29b6


## Examples of Good Stories or Interactive Products

### https://www2.ed.gov/datastory/el-characteristics/index.html#intro
uses hyperspace by pixelarity: https://pixelarity.com/hyperspace

### printing maps
https://maposmatic.osm-baustelle.de/new/

### validation: OSMCha
https://osmcha.mapbox.com/
-Osmose, KeepRight


#### Traveling Salesman problem
http://vroom-project.org/
https://www.optaplanner.org/

### StoryTelling

https://www.nytimes.com/interactive/2014/07/03/world/middleeast/syria-iraq-isis-rogue-state-along-two-rivers.html 
http://dwtkns.com/portfolio/

#### visualizing OSM attribution with IDly
https://medium.com/@kepta/when-openstreetmap-met-mapbox-gl-idly-gl-c26ecfdad93c


**Idea what if there was a tag-based pivot table you could create online? (ex. compare road classifications to widths and see if there is any correlation)

## Federating with CKAN
In order to expose datasets, GeoNode uses Catalog Service for the Web (CSW), ESRI ArcGIS Online uses DCAT (https://www.w3.org/TR/vocab-dcat/). GeoPlatform can harvest from both (https://doc.arcgis.com/en/hub/data/federating-with-ckan.htm). 

## Geosimulation (http://www.geosimulation.org/)
Geosimulation is a catch-all phrase that can be used to represent a new wave of spatial simulation modeling that has come to the fore in very recent years.

### Go Map!!
OSM editor for iOS
https://apps.apple.com/us/app/go-map/id592990211

### POSTGIS and vector tiles
https://sparkgeo.com/blog/vector-tile-server-using-postgis/

### Dev Seed and Urchn (Machine learning and OSM)
https://medium.com/devseed/make-sense-of-urban-change-fabb9ff229d7

## QGIS dev shops
- Kartoza
- opengis.ch
- source pole

### design tools
https://www.framer.com/development/

### video animations
https://www.google.com/earth/studio/

### OSM Express (OSMX)
Here are some use cases that OSM Express fits well.
- You want an offline copy of OpenStreetMap, which can be updated every day, hour or minute from the main openstreetmap.org database, instead of redownloading the entire planet.
- You want to quickly access all OSM objects in a geographical region, such as as neighborhood, city or small country. For this use, https://protomaps.com/extracts/
- You want to quickly look up OSM objects by ID, such as getting the height and name tags for a given way that represents a building, and construct geometries for ways and relations.
- You want to embed a database that does any of the above, such as in a web application that returns OSM objects as GeoJSON.

# 3D Technology

### GeoSim
https://geosimcities.com/
https://www.crunchbase.com/organization/geosim

#### Vector Tiles and POSTGIS
https://info.crunchydata.com/blog/dynamic-vector-tiles-from-postgis

#### Identifying Gaps in OSM
https://towardsdatascience.com/identifying-gaps-in-openstreetmap-coverage-through-machine-learning-257545c04330

#### Good QGIS Python scripting course
https://courses.spatialthoughts.com/pyqgis-in-a-day.html#print-layouts

## OSM Research
### OpenStreetMap in GIScience
### Experiences, Research, and Applications
https://www.google.com/books/edition/OpenStreetMap_in_GIScience/uHIKBwAAQBAJ?hl=en&gbpv=1&printsec=frontcover

# Networks and Graphs

## peartree
https://github.com/kuanb/peartree
peartree is a library for converting GTFS feed schedules into a representative directed network graph. The tool uses Partridge to convert the target operator schedule data into Pandas dataframes and then NetworkX to hold the manipulated schedule data as a directed multigraph.

## partridge
https://github.com/remix/partridge
A fast, forgiving GTFS reader built on pandas DataFrames

## Distributed Version Control

Sno
https://sno.earth/

Geogig

## CartONG Leaderboard
http://mapathon.cartong.org/


# Quality
### Lyft: Ground Truth Evaluation of OpenStreetMap Quality in North American Cities
https://drive.google.com/file/d/1Sb-dOUjeP1Ljqz4ra931D3Pe8B5C3pde/view

## geoBoundaries 3.0
Admin boundaries for the world, by William and Mary
https://www.wm.edu/as/data-science/researchlabs/geolab/get_data/geoboundaries/index.php

## Road Planning
https://road-planning.devseed.com/

## NightTime lights: World Bank
https://registry.opendata.aws/wb-light-every-night/
https://worldbank.github.io/OpenNightLights/tutorials/mod5_4_comparing_cities.html

### WSF-Evolution
https://ui.adsabs.harvard.edu/abs/2018AGUFMIN44A..06M/abstract

## Routing engines
https://github.com/conveyal/r5

ESRI 2020 Land Cover: https://www.arcgis.com/home/item.html?id=d6642f8a4f6d4685a24ae2dc0c73d4ac 

scikit-mobility is a library for human mobility analysis in Python: https://github.com/scikit-mobility/scikit-mobility

#### Example story maps and news with maps:
Rohingya Refugee Emergency at a Glance: The influx to Bangladesh is one of the largest and fastest-growing refugee crises in decades
https://unhcr.maps.arcgis.com/apps/Cascade/index.html?appid=5fdca0f47f1a46498002f39894fcd26f
America is more diverse than ever — but still segregated:
https://www.washingtonpost.com/graphics/2018/national/segregation-us-cities/
Mapping America’s wicked weather and deadly disasters:
https://www.washingtonpost.com/graphics/2019/national/mapping-disasters/
BORDERLINE: Navigating the invisible boundary and physical barriers that define the U.S.-Mexico border
https://www.washingtonpost.com/graphics/2018/national/us-mexico-border-flyover/
Good examples from the Washington Post here: https://www.washingtonpost.com/graphics/2018/ns/best-graphics/
 -you can also click on the different Graphics reporters


#### OSM in Government
https://osm.gs.mil/

#### GIS rater aligning/co-registering/re-sampling
https://pygis.io/docs/e_raster_resample.html 

#### Online GIS and Python courses
-PyGIS: https://github.com/mmann1123/pyGIS

#### GeoWombat: https://geowombat.readthedocs.io/en/latest/index.html 
open geospatial rasters as chunked Dask arrays

https://s2maps.eu/
Sentinel imagery service cloudless
