## Instructions

- This folder contains original osmPolyconvert.typ.xml
- The colour code in xml multiplied by 255 gives the RGB value
- The location of the file to change:
    ``` bash
    "C:/Program Files (x86)/Eclipse/Sumo/data/typemap/osmPolyconvert.typ.xml"
    ```
- Change the colours at different layers for different types of polygons in the `osmPolyconvert.typ.xml`
- The command for generating osm.sumocfg with updated colours:
   ``` bash
    polyconvert --net-file osm.net.xml.gz --osm-files osm_bbox.osm.xml.gz --osm.keep-full-type=true --osm.merge-relations=1 --type-file "C:/Program Files (x86)/Eclipse/Sumo/data/typemap/osmPolyconvert.typ.xml" --output-file osm.poly.xml.gz --verbose
    ```
# For Colleges,Universities
- All the colleges and universities are in layer -2 and +3(for point id), their colour is violet with xml colour code- "0.58, 0.0, 0.83"
- Mostly building area- resedential campus outer layers areas are in layer -3, their colour is pink with xml colour code- "1.0,0.75,0.8"
- All lanes are black and gray mostly
- All the buildings are in layer -1 with colour red with xml colour code- "1.0,.0,.0"
- All the hospitals are in layer -1 and +4(for point id), their colour is yellow with colour code- "1.0,1.0,.0"
- All the banks are in layer +4(for point id) only few in layer -1, their colour is blue with colour code- ".0,1.0,.0"
- Highways are mainly black gray with colour code- ".10,.10,.10"