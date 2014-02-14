Readme for notes about data
======================================


Sample data - Leeds
--------------------------------------

To download small amounts of data from OSM you can use the HTTP API. Details here:
https://wiki.openstreetmap.org/wiki/Downloading_data#Choose_your_region

The URL for downloading Leeds is: (using same bounding box that Nick used for capturing tweets)

http://api.openstreetmap.org/api/0.6/map?bbox=-1.800358,53.698979,-1.290341,53.945871

so the command to get the osm file and save it as 'leeds.osm' us:

wget --output-document=leeds.osm "http://api.openstreetmap.org/api/0.6/map?bbox=11.54,48.14,11.543,48.145"

These can be added to a SpatialLite database using QGIS 2.0 core functionality:

Vector -> OSM -> Import Topology from XML.

then

Vector -> OSM -> Export Topology to SpatialLite

For some reason, these lines are not correct .. needs further investigation...
