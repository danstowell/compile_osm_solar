# compile_osm_solar
Script to parse an OSM XML extract for solar PV data

The extract must ALREADY have been processed by osmium to filter down to just the generator:method=photovoltaic items.

Here's what I do:

`osmium tags-filter ~/osm/great-britain/great-britain-190802.osm.pbf generator:method=photovoltaic plant:method=photovoltaic plant:source=solar -o  ~/osm/solarsearch/gb-solarextracts/gb-190802-solar-withreferenced.xml`


Requirements:

* Python 3
* Python packages:
   * numpy
   * pandas
   * matplotlib
   * scipy
* [osmium](https://osmcode.org/osmium-tool/)

