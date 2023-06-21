# Comparing `tmp/commonroad_scenario_designer-0.7.0.tar.gz` & `tmp/commonroad_scenario_designer-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad_scenario_designer-0.7.0.tar", max compression
+gzip compressed data, was "commonroad_scenario_designer-0.7.1.tar", max compression
```

## Comparing `commonroad_scenario_designer-0.7.0.tar` & `commonroad_scenario_designer-0.7.1.tar`

### file list

```diff
@@ -1,239 +1,234 @@
--rw-r--r--   0        0        0    35148 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0    11596 2023-03-27 15:04:16.367944 commonroad_scenario_designer-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/configurations/__init__.py
--rw-r--r--   0        0        0     2521 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/configurations/configuration.py
--rw-r--r--   0        0        0     2953 2023-02-11 09:29:52.350372 commonroad_scenario_designer-0.7.0/crdesigner/configurations/configuration_builder.py
--rw-r--r--   0        0        0      382 2023-03-23 10:04:08.771185 commonroad_scenario_designer-0.7.0/crdesigner/configurations/custom_settings.yaml
--rw-r--r--   0        0        0     2566 2023-03-23 10:04:08.771185 commonroad_scenario_designer-0.7.0/crdesigner/configurations/custom_settings_osm2cr.yaml
--rw-r--r--   0        0        0      382 2023-02-08 02:03:14.542675 commonroad_scenario_designer-0.7.0/crdesigner/configurations/default_settings.yaml
--rw-r--r--   0        0        0     2564 2023-02-08 02:03:14.542675 commonroad_scenario_designer-0.7.0/crdesigner/configurations/default_settings_osm2cr.yaml
--rw-r--r--   0        0        0      135 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/configurations/defaults/file_header.yaml
--rw-r--r--   0        0        0      622 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/configurations/defaults/opendrive.yaml
--rw-r--r--   0        0        0       47 2023-02-08 02:03:14.542675 commonroad_scenario_designer-0.7.0/crdesigner/configurations/definition.py
--rw-r--r--   0        0        0      581 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/configurations/get_configs.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/common/__init__.py
--rw-r--r--   0        0        0    18519 2023-03-23 11:26:35.293326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/common/conversion_lanelet.py
--rw-r--r--   0        0        0    69176 2023-03-23 11:26:35.297326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/common/conversion_lanelet_network.py
--rw-r--r--   0        0        0     1470 2023-03-23 11:26:35.297326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/common/utils.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.872960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/__init__.py
--rw-r--r--   0        0        0     1447 2023-03-23 11:26:35.297326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/config.py
--rw-r--r--   0        0        0    29254 2023-03-26 12:47:03.756666 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/cr2lanelet.py
--rw-r--r--   0        0        0    11566 2023-03-26 12:47:03.756666 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/lanelet2.py
--rw-r--r--   0        0        0     4645 2023-03-23 11:26:35.297326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/lanelet2_parser.py
--rw-r--r--   0        0        0    45391 2023-03-23 11:26:35.297326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/lanelet2cr.py
--rw-r--r--   0        0        0     6300 2023-03-23 10:04:08.771185 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/map_conversion_interface.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/__init__.py
--rw-r--r--   0        0        0    10337 2023-02-11 09:29:52.350372 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/converter.py
--rw-r--r--   0        0        0    37242 2023-03-23 11:26:35.297326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/network.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/__init__.py
--rw-r--r--   0        0        0     5372 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/border.py
--rw-r--r--   0        0        0     1982 2023-03-23 11:26:35.301326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/crosswalks.py
--rw-r--r--   0        0        0      925 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/geo_reference.py
--rw-r--r--   0        0        0    16917 2023-02-09 17:56:25.886072 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane.py
--rw-r--r--   0        0        0    22233 2023-03-23 11:26:35.301326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane_group.py
--rw-r--r--   0        0        0    11740 2023-02-21 08:30:59.147245 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/traffic_signals.py
--rw-r--r--   0        0        0     4490 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/utils.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/__init__.py
--rw-r--r--   0        0        0     3975 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/eulerspiral.py
--rw-r--r--   0        0        0    18376 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/geometry.py
--rw-r--r--   0        0        0     5862 2023-02-01 09:37:39.876960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/junction.py
--rw-r--r--   0        0        0     4754 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/opendrive.py
--rw-r--r--   0        0        0     6096 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road.py
--rw-r--r--   0        0        0      632 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadElevationProfile.py
--rw-r--r--   0        0        0    21787 2023-02-09 17:56:25.886072 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLanes.py
--rw-r--r--   0        0        0     5275 2023-02-08 02:03:14.546675 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLateralProfile.py
--rw-r--r--   0        0        0     7605 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLink.py
--rw-r--r--   0        0        0     8218 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadObject.py
--rw-r--r--   0        0        0    12550 2023-03-23 11:26:35.301326 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadPlanView.py
--rw-r--r--   0        0        0     8212 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadSignal.py
--rw-r--r--   0        0        0     1430 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road_record.py
--rw-r--r--   0        0        0     3922 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadtype.py
--rw-r--r--   0        0        0    28362 2023-02-09 17:56:25.886072 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/parser.py
--rw-r--r--   0        0        0       47 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/.gitignore
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/__init__.py
--rw-r--r--   0        0        0     7546 2023-03-23 10:04:08.771185 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/config.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/__init__.py
--rw-r--r--   0        0        0     5613 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/converter.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/__init__.py
--rw-r--r--   0        0        0    19464 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/cleanup.py
--rw-r--r--   0        0        0    10423 2023-02-21 08:30:59.147245 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/export.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/__init__.py
--rw-r--r--   0        0        0     4131 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/intersection_merger.py
--rw-r--r--   0        0        0    36721 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/lane_linker.py
--rw-r--r--   0        0        0     2801 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/mapillary.py
--rw-r--r--   0        0        0     4448 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/offsetter.py
--rw-r--r--   0        0        0     2161 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/restrictions.py
--rw-r--r--   0        0        0      501 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/__init__.py
--rw-r--r--   0        0        0    31637 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph.py
--rw-r--r--   0        0        0    18447 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_edge.py
--rw-r--r--   0        0        0     6496 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_functions.py
--rw-r--r--   0        0        0     9586 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_lane.py
--rw-r--r--   0        0        0     4150 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_node.py
--rw-r--r--   0        0        0     1192 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_light.py
--rw-r--r--   0        0        0     1966 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_sign.py
--rw-r--r--   0        0        0     2729 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_sublayered_graph.py
--rw-r--r--   0        0        0    14898 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/segment_clusters.py
--rw-r--r--   0        0        0    11702 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/traffic_sign_parser.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/__init__.py
--rw-r--r--   0        0        0      237 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/__init__.py
--rw-r--r--   0        0        0     6345 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_edge.py
--rw-r--r--   0        0        0    21156 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_format.py
--rw-r--r--   0        0        0      607 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_node.py
--rw-r--r--   0        0        0    12814 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intersection_enhancement.py
--rw-r--r--   0        0        0     2333 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/traffic_light_generator.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/__init__.py
--rw-r--r--   0        0        0     3482 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/downloader.py
--rw-r--r--   0        0        0     7332 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/info_deduction.py
--rw-r--r--   0        0        0    36880 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/osm_parser.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/__init__.py
--rw-r--r--   0        0        0      508 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/custom_types.py
--rw-r--r--   0        0        0    28332 2023-02-01 09:37:39.880960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/geometry.py
--rw-r--r--   0        0        0     2055 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/geonamesID.py
--rw-r--r--   0        0        0     1286 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/graph_analysis.py
--rw-r--r--   0        0        0      857 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/idgenerator.py
--rw-r--r--   0        0        0     9259 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/plots.py
--rw-r--r--   0        0        0     3554 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/main.py
--rw-r--r--   0        0        0      198 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/.gitignore
--rw-r--r--   0        0        0      288 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/__init__.py
--rw-r--r--   0        0        0     8301 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/config.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/__init__.py
--rw-r--r--   0        0        0   116978 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/converter.py
--rw-r--r--   0        0        0     9601 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/mapping.py
--rw-r--r--   0        0        0     5087 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_light.py
--rw-r--r--   0        0        0     9635 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_sign.py
--rw-r--r--   0        0        0      387 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/errors.py
--rw-r--r--   0        0        0     2769 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/merge.py
--rw-r--r--   0        0        0     2155 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/sumo2cr.py
--rw-r--r--   0        0        0    62888 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/sumolib_net.py
--rw-r--r--   0        0        0     5629 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/DEU.typ.xml
--rw-r--r--   0        0        0      647 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/README.md
--rw-r--r--   0        0        0     4613 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/USA.typ.xml
--rw-r--r--   0        0        0     5629 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/ZAM.typ.xml
--rw-r--r--   0        0        0      796 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/default.sumo.cfg
--rw-r--r--   0        0        0    20378 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/util.py
--rw-r--r--   0        0        0      731 2023-02-08 02:03:14.546675 commonroad_scenario_designer-0.7.0/crdesigner/start_gui.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/cli/__init__.py
--rw-r--r--   0        0        0     6063 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/cli/command_line.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/__init__.py
--rw-r--r--   0        0        0      427 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/gui.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/__init__.py
--rw-r--r--   0        0        0     4670 2023-03-27 14:17:19.277609 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/animated_viewer_wrapper.py
--rw-r--r--   0        0        0       44 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/__init__.py
--rw-r--r--   0        0        0    15261 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/animated_viewer.py
--rw-r--r--   0        0        0    46687 2023-03-27 10:06:04.022492 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/dynamic_canvas.py
--rw-r--r--   0        0        0     2154 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/helper.py
--rw-r--r--   0        0        0      346 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/__init__.py
--rw-r--r--   0        0        0     8704 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/draw_params_updater.py
--rw-r--r--   0        0        0      566 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/general_services.py
--rw-r--r--   0        0        0     1511 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/scenario_resizer.py
--rw-r--r--   0        0        0     6239 2023-02-21 08:30:59.147245 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/gui_sumo_simulation.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/__init__.py
--rw-r--r--   0        0        0      828 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/crdesigner_console_wrapper.py
--rw-r--r--   0        0        0     6882 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/mwindow.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/__init__.py
--rw-r--r--   0        0        0    10320 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/aerial_data.py
--rw-r--r--   0        0        0      690 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/config.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/converter_modules/__init__.py
--rw-r--r--   0        0        0      499 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/converter_modules/converter_interface.py
--rw-r--r--   0        0        0     3467 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/converter_modules/opendrive_interface.py
--rw-r--r--   0        0        0     2203 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/converter_modules/osm_interface.py
--rw-r--r--   0        0        0      883 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/errors.py
--rw-r--r--   0        0        0     5193 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/general_services.py
--rw-r--r--   0        0        0     1567 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.py
--rw-r--r--   0        0        0     2702 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.ui
--rw-r--r--   0        0        0     6650 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.py
--rw-r--r--   0        0        0     6134 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.ui
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/__init__.py
--rw-r--r--   0        0        0    23092 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/gui_settings_ui.py
--rw-r--r--   0        0        0    34788 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/osm_settings_ui.py
--rw-r--r--   0        0        0    10566 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog.py
--rw-r--r--   0        0        0     5960 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog_ui.py
--rw-r--r--   0        0        0     5536 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/settings_ui.py
--rw-r--r--   0        0        0      464 2023-02-01 09:37:39.884960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/size_policies.py
--rw-r--r--   0        0        0    41909 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/sumo_settings_ui.py
--rw-r--r--   0        0        0     9993 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_settings.py
--rw-r--r--   0        0        0  1852651 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.py
--rw-r--r--   0        0        0     1136 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.qrc
--rw-r--r--   0        0        0    33556 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/Groupe_6.png
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/__init__.py
--rw-r--r--   0        0        0     8020 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_left.png
--rw-r--r--   0        0        0      645 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_right.png
--rw-r--r--   0        0        0      770 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_lane.png
--rw-r--r--   0        0        0    21597 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_redo.png
--rw-r--r--   0        0        0    21742 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_undo.png
--rw-r--r--   0        0        0    32283 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/close.png
--rw-r--r--   0        0        0    67646 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr.ico
--rw-r--r--   0        0        0    89174 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.ico
--rw-r--r--   0        0        0    26980 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.png
--rw-r--r--   0        0        0    96318 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr2.ico
--rw-r--r--   0        0        0    17853 2023-02-01 09:37:39.896960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/drawing_mode.png
--rw-r--r--   0        0        0    68262 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.ico
--rw-r--r--   0        0        0      646 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.png
--rw-r--r--   0        0        0      207 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/iconmonstr-trash-can-darkmode.png
--rw-r--r--   0        0        0      409 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/iconmonstr-trash-can.svg
--rw-r--r--   0        0        0     1417 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/merge_lanelet.png
--rw-r--r--   0        0        0    26374 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/new_file.png
--rw-r--r--   0        0        0    12185 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.png
--rw-r--r--   0        0        0   140025 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.svg
--rw-r--r--   0        0        0    25413 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/open_file.png
--rw-r--r--   0        0        0     1438 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause.png
--rw-r--r--   0        0        0     3976 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause_darkmode.png
--rw-r--r--   0        0        0     2303 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/play.png
--rw-r--r--   0        0        0   109822 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.png
--rw-r--r--   0        0        0    90702 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.svg
--rw-r--r--   0        0        0   432254 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/save.ico
--rw-r--r--   0        0        0    10339 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_file.png
--rw-r--r--   0        0        0     1673 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.png
--rw-r--r--   0        0        0     3382 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.svg
--rw-r--r--   0        0        0      734 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/split_lanelet.png
--rw-r--r--   0        0        0     4596 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/target-darkmode.png
--rw-r--r--   0        0        0     8300 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/target.png
--rw-r--r--   0        0        0    67646 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/tools.ico
--rw-r--r--   0        0        0      956 2023-02-01 09:37:39.900960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/help_actions.py
--rw-r--r--   0        0        0    71248 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/map_creator.py
--rw-r--r--   0        0        0    29430 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/osm_settings.py
--rw-r--r--   0        0        0    29122 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/osm_settings_ui.py
--rw-r--r--   0        0        0        0 2023-03-23 14:12:45.011703 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/services/__init__.py
--rw-r--r--   0        0        0     6254 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/services/config_default.py
--rw-r--r--   0        0        0    22445 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/services/plots_interactive.py
--rw-r--r--   0        0        0     7409 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/services/waitingspinnerwidget.py
--rw-r--r--   0        0        0      115 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/settings.json
--rw-r--r--   0        0        0     3965 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/settings.py
--rw-r--r--   0        0        0     8395 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/sumo_settings.py
--rw-r--r--   0        0        0      356 2023-02-08 02:03:14.550675 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/transfer.py
--rw-r--r--   0        0        0     2064 2023-02-06 14:01:29.894354 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/util.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/__init__.py
--rw-r--r--   0        0        0      934 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/create_converter_toolbox.py
--rw-r--r--   0        0        0    18502 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox.py
--rw-r--r--   0        0        0     7878 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox_ui.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/__init__.py
--rw-r--r--   0        0        0      770 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/create_obstacle_toolbox.py
--rw-r--r--   0        0        0    54836 2023-02-06 14:01:29.894354 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox.py
--rw-r--r--   0        0        0    15463 2023-02-06 14:01:29.898354 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox_ui.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/__init__.py
--rw-r--r--   0        0        0      926 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/create_road_network_toolbox.py
--rw-r--r--   0        0        0   113978 2023-03-23 10:04:08.775185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox.py
--rw-r--r--   0        0        0    79772 2023-03-23 10:04:08.779185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox_ui.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/service_layer/__init__.py
--rw-r--r--   0        0        0      383 2023-03-23 10:04:08.779185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/service_layer/general_services.py
--rw-r--r--   0        0        0    14360 2023-03-23 10:04:08.779185 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/toolbox_ui.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/__init__.py
--rw-r--r--   0        0        0     3183 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/menu_bar_wrapper.py
--rw-r--r--   0        0        0      510 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/__init__.py
--rw-r--r--   0        0        0     4670 2023-03-27 09:52:36.213980 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/file_actions.py
--rw-r--r--   0        0        0      993 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/general_services.py
--rw-r--r--   0        0        0      451 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/help_actions.py
--rw-r--r--   0        0        0     1391 2023-02-21 08:30:59.147245 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/setting_actions.py
--rw-r--r--   0        0        0        0 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/__init__.py
--rw-r--r--   0        0        0    12620 2023-03-27 14:31:46.900067 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/toolbar_wrapper.py
--rw-r--r--   0        0        0     1230 2023-02-01 09:37:39.904960 commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/top_bar_wrapper.py
--rw-r--r--   0        0        0     2195 2023-03-27 15:04:16.367944 commonroad_scenario_designer-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    13614 1970-01-01 00:00:00.000000 commonroad_scenario_designer-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-26 01:03:30.014174 commonroad_scenario_designer-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0    11418 2023-06-21 05:40:36.506124 commonroad_scenario_designer-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.462115 commonroad_scenario_designer-0.7.1/crdesigner/__init__.py
+-rw-r--r--   0        0        0     8245 2023-06-19 10:49:53.585780 commonroad_scenario_designer-0.7.1/crdesigner/config/config.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/configurations/__init__.py
+-rw-r--r--   0        0        0      382 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/custom_settings.yaml
+-rw-r--r--   0        0        0     2566 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/custom_settings_osm2cr.yaml
+-rw-r--r--   0        0        0      382 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/default_settings.yaml
+-rw-r--r--   0        0        0     2564 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/default_settings_osm2cr.yaml
+-rw-r--r--   0        0        0       47 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/configurations/definition.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/__init__.py
+-rw-r--r--   0        0        0    17976 2023-06-14 05:25:23.786499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/conversion_lanelet.py
+-rw-r--r--   0        0        0    71077 2023-06-14 05:25:23.786499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/conversion_lanelet_network.py
+-rw-r--r--   0        0        0    28332 2023-06-14 05:25:23.786499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/geometry.py
+-rw-r--r--   0        0        0     1470 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/__init__.py
+-rw-r--r--   0        0        0    31052 2023-06-19 10:49:53.585780 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/cr2lanelet.py
+-rw-r--r--   0        0        0    12890 2023-06-20 13:58:00.286809 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2.py
+-rw-r--r--   0        0        0     4645 2023-04-26 01:03:30.018174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2_parser.py
+-rw-r--r--   0        0        0    47862 2023-06-19 11:30:56.919488 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2cr.py
+-rw-r--r--   0        0        0     6758 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/map_conversion_interface.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/__init__.py
+-rw-r--r--   0        0        0    10196 2023-06-14 05:25:23.786499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/converter.py
+-rw-r--r--   0        0        0    37032 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/network.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/__init__.py
+-rw-r--r--   0        0        0     4821 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/border.py
+-rw-r--r--   0        0        0     1982 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/crosswalks.py
+-rw-r--r--   0        0        0      944 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/geo_reference.py
+-rw-r--r--   0        0        0    16247 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane.py
+-rw-r--r--   0        0        0    23257 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane_group.py
+-rw-r--r--   0        0        0    11695 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/traffic_signals.py
+-rw-r--r--   0        0        0     3935 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/utils.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/__init__.py
+-rw-r--r--   0        0        0     3985 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/eulerspiral.py
+-rw-r--r--   0        0        0    18380 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/geometry.py
+-rw-r--r--   0        0        0     5862 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/junction.py
+-rw-r--r--   0        0        0     4828 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/opendrive.py
+-rw-r--r--   0        0        0     6096 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road.py
+-rw-r--r--   0        0        0      632 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadElevationProfile.py
+-rw-r--r--   0        0        0    21954 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLanes.py
+-rw-r--r--   0        0        0     5275 2023-04-26 01:03:30.022174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLateralProfile.py
+-rw-r--r--   0        0        0     7605 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLink.py
+-rw-r--r--   0        0        0     8351 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadObject.py
+-rw-r--r--   0        0        0    12550 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadPlanView.py
+-rw-r--r--   0        0        0     8212 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadSignal.py
+-rw-r--r--   0        0        0     1430 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road_record.py
+-rw-r--r--   0        0        0     3922 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadtype.py
+-rw-r--r--   0        0        0    28758 2023-06-20 09:20:47.449328 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/parser.py
+-rw-r--r--   0        0        0       47 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/__init__.py
+-rw-r--r--   0        0        0     7546 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/config.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/__init__.py
+-rw-r--r--   0        0        0     5613 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/converter.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/__init__.py
+-rw-r--r--   0        0        0    19464 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/cleanup.py
+-rw-r--r--   0        0        0    10397 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/export.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/__init__.py
+-rw-r--r--   0        0        0     4131 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/intersection_merger.py
+-rw-r--r--   0        0        0    36721 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/lane_linker.py
+-rw-r--r--   0        0        0     2801 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/mapillary.py
+-rw-r--r--   0        0        0     4422 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/offsetter.py
+-rw-r--r--   0        0        0     2161 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/restrictions.py
+-rw-r--r--   0        0        0      501 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/__init__.py
+-rw-r--r--   0        0        0    31611 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph.py
+-rw-r--r--   0        0        0    18421 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_edge.py
+-rw-r--r--   0        0        0     6470 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_functions.py
+-rw-r--r--   0        0        0     9630 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_lane.py
+-rw-r--r--   0        0        0     4124 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_node.py
+-rw-r--r--   0        0        0     1192 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_light.py
+-rw-r--r--   0        0        0     1966 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_sign.py
+-rw-r--r--   0        0        0     2729 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_sublayered_graph.py
+-rw-r--r--   0        0        0    14872 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/segment_clusters.py
+-rw-r--r--   0        0        0    11702 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/traffic_sign_parser.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/__init__.py
+-rw-r--r--   0        0        0     6345 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_edge.py
+-rw-r--r--   0        0        0    21200 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_format.py
+-rw-r--r--   0        0        0      581 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_node.py
+-rw-r--r--   0        0        0    12858 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intersection_enhancement.py
+-rw-r--r--   0        0        0     2333 2023-04-26 01:03:30.026174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/traffic_light_generator.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/__init__.py
+-rw-r--r--   0        0        0     3482 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/downloader.py
+-rw-r--r--   0        0        0     7332 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/info_deduction.py
+-rw-r--r--   0        0        0    36854 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/osm_parser.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.466115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/__init__.py
+-rw-r--r--   0        0        0      508 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/custom_types.py
+-rw-r--r--   0        0        0     2055 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/geonamesID.py
+-rw-r--r--   0        0        0     1286 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/graph_analysis.py
+-rw-r--r--   0        0        0      857 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/idgenerator.py
+-rw-r--r--   0        0        0     9259 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/plots.py
+-rw-r--r--   0        0        0     3554 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/main.py
+-rw-r--r--   0        0        0      198 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/.gitignore
+-rw-r--r--   0        0        0      288 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/__init__.py
+-rw-r--r--   0        0        0     8301 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/config.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/__init__.py
+-rw-r--r--   0        0        0   116978 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/converter.py
+-rw-r--r--   0        0        0     9601 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/mapping.py
+-rw-r--r--   0        0        0     5087 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_light.py
+-rw-r--r--   0        0        0     9635 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_sign.py
+-rw-r--r--   0        0        0      387 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/errors.py
+-rw-r--r--   0        0        0     2769 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/merge.py
+-rw-r--r--   0        0        0     2050 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/sumo2cr.py
+-rw-r--r--   0        0        0    62888 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/sumolib_net.py
+-rw-r--r--   0        0        0     5629 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/DEU.typ.xml
+-rw-r--r--   0        0        0      647 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/README.md
+-rw-r--r--   0        0        0     4613 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/USA.typ.xml
+-rw-r--r--   0        0        0     5629 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/ZAM.typ.xml
+-rw-r--r--   0        0        0      796 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/default.sumo.cfg
+-rw-r--r--   0        0        0    20378 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/util.py
+-rw-r--r--   0        0        0      731 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/start_gui.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/cli/__init__.py
+-rw-r--r--   0        0        0     7028 2023-06-19 11:30:56.919488 commonroad_scenario_designer-0.7.1/crdesigner/ui/cli/command_line.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/gui.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/__init__.py
+-rw-r--r--   0        0        0     4670 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/animated_viewer_wrapper.py
+-rw-r--r--   0        0        0       44 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/__init__.py
+-rw-r--r--   0        0        0    16825 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/animated_viewer.py
+-rw-r--r--   0        0        0    44796 2023-06-19 10:49:53.585780 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/dynamic_canvas.py
+-rw-r--r--   0        0        0     2154 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/helper.py
+-rw-r--r--   0        0        0      346 2023-04-26 01:03:30.030174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/__init__.py
+-rw-r--r--   0        0        0     8704 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/draw_params_updater.py
+-rw-r--r--   0        0        0      566 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/general_services.py
+-rw-r--r--   0        0        0     1511 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/scenario_resizer.py
+-rw-r--r--   0        0        0     6239 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/gui_sumo_simulation.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/__init__.py
+-rw-r--r--   0        0        0      828 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/crdesigner_console_wrapper.py
+-rw-r--r--   0        0        0     6882 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/mwindow.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/__init__.py
+-rw-r--r--   0        0        0    11509 2023-06-19 10:49:53.585780 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/aerial_data.py
+-rw-r--r--   0        0        0      690 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/config.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/__init__.py
+-rw-r--r--   0        0        0      499 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/converter_interface.py
+-rw-r--r--   0        0        0     3382 2023-06-14 05:25:23.790499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/opendrive_interface.py
+-rw-r--r--   0        0        0     2203 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/osm_interface.py
+-rw-r--r--   0        0        0      883 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/errors.py
+-rw-r--r--   0        0        0     5193 2023-05-17 01:03:25.147459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/general_services.py
+-rw-r--r--   0        0        0     1567 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.py
+-rw-r--r--   0        0        0     2702 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.ui
+-rw-r--r--   0        0        0     6650 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.py
+-rw-r--r--   0        0        0     6134 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.ui
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.470115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/__init__.py
+-rw-r--r--   0        0        0    23092 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/gui_settings_ui.py
+-rw-r--r--   0        0        0    34788 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/osm_settings_ui.py
+-rw-r--r--   0        0        0    10566 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog.py
+-rw-r--r--   0        0        0     5960 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog_ui.py
+-rw-r--r--   0        0        0     5536 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/settings_ui.py
+-rw-r--r--   0        0        0      464 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/size_policies.py
+-rw-r--r--   0        0        0    41909 2023-04-26 01:03:30.034174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/sumo_settings_ui.py
+-rw-r--r--   0        0        0     9993 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_settings.py
+-rw-r--r--   0        0        0  1852651 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.py
+-rw-r--r--   0        0        0     1136 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.qrc
+-rw-r--r--   0        0        0    33556 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/Groupe_6.png
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/__init__.py
+-rw-r--r--   0        0        0     8020 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_left.png
+-rw-r--r--   0        0        0      645 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_right.png
+-rw-r--r--   0        0        0      770 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_lane.png
+-rw-r--r--   0        0        0    21597 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_redo.png
+-rw-r--r--   0        0        0    21742 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_undo.png
+-rw-r--r--   0        0        0    32283 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/close.png
+-rw-r--r--   0        0        0    67646 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr.ico
+-rw-r--r--   0        0        0    89174 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.ico
+-rw-r--r--   0        0        0    26980 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.png
+-rw-r--r--   0        0        0    96318 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr2.ico
+-rw-r--r--   0        0        0    17853 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/drawing_mode.png
+-rw-r--r--   0        0        0    68262 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.ico
+-rw-r--r--   0        0        0      646 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.png
+-rw-r--r--   0        0        0      207 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/iconmonstr-trash-can-darkmode.png
+-rw-r--r--   0        0        0      409 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/iconmonstr-trash-can.svg
+-rw-r--r--   0        0        0     1417 2023-04-26 01:03:30.046174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/merge_lanelet.png
+-rw-r--r--   0        0        0    26374 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/new_file.png
+-rw-r--r--   0        0        0    12185 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.png
+-rw-r--r--   0        0        0   140025 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.svg
+-rw-r--r--   0        0        0    25413 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/open_file.png
+-rw-r--r--   0        0        0     1438 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause.png
+-rw-r--r--   0        0        0     3976 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause_darkmode.png
+-rw-r--r--   0        0        0     2303 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/play.png
+-rw-r--r--   0        0        0   109822 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.png
+-rw-r--r--   0        0        0    90702 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.svg
+-rw-r--r--   0        0        0   432254 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save.ico
+-rw-r--r--   0        0        0    10339 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_file.png
+-rw-r--r--   0        0        0     1673 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.png
+-rw-r--r--   0        0        0     3382 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.svg
+-rw-r--r--   0        0        0      734 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/split_lanelet.png
+-rw-r--r--   0        0        0     4596 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/target-darkmode.png
+-rw-r--r--   0        0        0     8300 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/target.png
+-rw-r--r--   0        0        0    67646 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/tools.ico
+-rw-r--r--   0        0        0      956 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/help_actions.py
+-rw-r--r--   0        0        0    71248 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/map_creator.py
+-rw-r--r--   0        0        0    29430 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/osm_settings.py
+-rw-r--r--   0        0        0    29122 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/osm_settings_ui.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/__init__.py
+-rw-r--r--   0        0        0     6254 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/config_default.py
+-rw-r--r--   0        0        0    22397 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/plots_interactive.py
+-rw-r--r--   0        0        0     7409 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/waitingspinnerwidget.py
+-rw-r--r--   0        0        0      115 2023-04-26 01:03:30.050174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/settings.json
+-rw-r--r--   0        0        0     3965 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/settings.py
+-rw-r--r--   0        0        0     8395 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/sumo_settings.py
+-rw-r--r--   0        0        0      356 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/transfer.py
+-rw-r--r--   0        0        0     2064 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/util.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/__init__.py
+-rw-r--r--   0        0        0      940 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/create_converter_toolbox.py
+-rw-r--r--   0        0        0    18391 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox.py
+-rw-r--r--   0        0        0     7878 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox_ui.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/__init__.py
+-rw-r--r--   0        0        0      770 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/create_obstacle_toolbox.py
+-rw-r--r--   0        0        0    54836 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox.py
+-rw-r--r--   0        0        0    15463 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox_ui.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/__init__.py
+-rw-r--r--   0        0        0      926 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/create_road_network_toolbox.py
+-rw-r--r--   0        0        0   114598 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox.py
+-rw-r--r--   0        0        0    79596 2023-06-20 09:11:13.860075 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox_ui.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/service_layer/__init__.py
+-rw-r--r--   0        0        0      450 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/service_layer/general_services.py
+-rw-r--r--   0        0        0    14360 2023-05-17 01:03:25.151459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/toolbox_ui.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.474115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/__init__.py
+-rw-r--r--   0        0        0     3183 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/menu_bar_wrapper.py
+-rw-r--r--   0        0        0      510 2023-04-26 01:03:30.054174 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/__init__.py
+-rw-r--r--   0        0        0     4665 2023-06-14 05:25:23.794499 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/file_actions.py
+-rw-r--r--   0        0        0      993 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/general_services.py
+-rw-r--r--   0        0        0      451 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/help_actions.py
+-rw-r--r--   0        0        0     1391 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/setting_actions.py
+-rw-r--r--   0        0        0        0 2023-06-21 06:48:08.478115 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/__init__.py
+-rw-r--r--   0        0        0    12620 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/toolbar_wrapper.py
+-rw-r--r--   0        0        0     1230 2023-05-17 01:03:25.155459 commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/top_bar_wrapper.py
+-rw-r--r--   0        0        0     2211 2023-06-21 05:40:36.510124 commonroad_scenario_designer-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    13271 1970-01-01 00:00:00.000000 commonroad_scenario_designer-0.7.1/PKG-INFO
```

### Comparing `commonroad_scenario_designer-0.7.0/LICENSE.txt` & `commonroad_scenario_designer-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/README.md` & `commonroad_scenario_designer-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)  
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)  
 [![PyPI version fury.io](https://badge.fury.io/py/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)
 [![PyPI download week](https://img.shields.io/pypi/dw/commonroad-scenario-designer.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-scenario-designer/) 
 [![PyPI download month](https://img.shields.io/pypi/dm/commonroad-scenario-designer.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-scenario-designer/)  
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)
-[![Documentation Status](https://readthedocs.org/projects/commonroad-scenario-designer/badge/?version=latest)](http://commonroad-scenario-designer.readthedocs.io/?badge=latest) 
 
 This toolbox provides map converters for [OpenStreetMap](https://www.openstreetmap.de/karte.html) (OSM), 
 [Lanelet](https://www.mrt.kit.edu/software/libLanelet/libLanelet.html) / [Lanelet2](https://github.com/fzi-forschungszentrum-informatik/Lanelet2), 
 [OpenDRIVE](https://www.asam.net/standards/detail/opendrive/), and [SUMO](https://sumo.dlr.de/docs/index.html) to the [CommonRoad](https://commonroad.in.tum.de/) 
 (CR) format and for some formats vice versa.  
 Additionally, a graphical user interface (GUI) is included, which allows one to efficiently create and manipulate 
 CommonRoad maps and scenarios.
@@ -139,15 +138,15 @@
 The titles of module pages have to be set manually!  
 The full documentation of the API and introducing examples can also be found [here](https://commonroad-scenario-designer.readthedocs.io/en/latest/).
 
 ## Changelog
 A detailed overview about the changes in each version is provided in the [Changelog](https://gitlab.lrz.de/tum-cps/commonroad-scenario-designer/-/blob/main/CHANGELOG.md).
 
 ## Bug and feature reporting
-This release (v0.7.0) is still a BETA version.  
+This release (v0.7.1) is still a BETA version.  
 In case you detect a bug or you want to suggest a new feature, please report it in our [forum](https://commonroad.in.tum.de/forum/c/scenario-designer/18).   
 If you want to contribute to the toolbox, you can also post it in the [forum](https://commonroad.in.tum.de/forum/c/scenario-designer/18) or contact [Sebastian Maierhofer](sebastian.maierhofer@tum.de).
 
 ## Authors
 
 Responsible: Sebastian Maierhofer, Sebastian Mair
 Contribution (in alphabetic order by last name): Daniel Asch, Hamza Begic, Florian Braunmiller, Tim Dang,
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/configurations/custom_settings_osm2cr.yaml` & `commonroad_scenario_designer-0.7.1/crdesigner/configurations/custom_settings_osm2cr.yaml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/configurations/default_settings_osm2cr.yaml` & `commonroad_scenario_designer-0.7.1/crdesigner/configurations/default_settings_osm2cr.yaml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/common/conversion_lanelet.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/conversion_lanelet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+import logging
 from typing import Tuple, Optional, Union, Set
 import numpy as np
+from pyproj import Transformer
 from commonroad.scenario.lanelet import Lanelet, LaneletType, LineMarking, RoadUser
-from crdesigner.map_conversion.opendrive.opendrive_conversion.utils import CustomDefaultLaneletType
-from crdesigner.configurations.get_configs import get_configs
-
-config = get_configs()
+from crdesigner.config.config import OpenDRIVEConversionParams
 
 
 class ConversionLanelet(Lanelet):
     """Change some properties of the Lanelet class so that it can be used to conversions to Lanelet. This means
     especially that lanelet_ids can be other types than a natural number and that these ids can be changed
     more than once. Adjacent neighbors and pre- and successor can be changed more than once.
     This class is being used in Opendrive and Lanelet2 format conversions
@@ -33,30 +32,29 @@
         line_marking_right_vertices=LineMarking.UNKNOWN,
         stop_line=None,
         lanelet_type=None,
         user_one_way=None,
         user_bidirectional=None,
         traffic_signs=None,
         traffic_lights=None,
-        custom_default_lanelet_types=CustomDefaultLaneletType(config.opendrive.general_lanelet_type_activ,
-                                                              config.opendrive.general_lanelet_type,
-                                                              config.opendrive.driving_default_lanelet_type,
-                                                              config.opendrive.lanelet_types_backwards_compatible),
-            speed=None,
+        speed=None,
+        config: OpenDRIVEConversionParams = OpenDRIVEConversionParams(),
+
     ):
+
         if lanelet_type is None:
             lanelet_type = {LaneletType.UNKNOWN}
         self.parametric_lane_group = parametric_lane_group
-        self._default_lanelet_type = {LaneletType(custom_default_lanelet_types.general_lanelet_type) if LaneletType(
-                custom_default_lanelet_types.general_lanelet_type) is not None else LaneletType.UNKNOWN} if \
-            custom_default_lanelet_types.general_lanelet_type_activ else set()
-        self._driving_default_lanelet_type = LaneletType(custom_default_lanelet_types.driving_default_lanelet_type) \
-            if LaneletType(custom_default_lanelet_types.driving_default_lanelet_type) is not None \
+        self._default_lanelet_type = {LaneletType(config.general_lanelet_type) if LaneletType(
+                config.general_lanelet_type) is not None else LaneletType.UNKNOWN} if \
+            config.general_lanelet_type_activ else set()
+        self._driving_default_lanelet_type = LaneletType(config.driving_default_lanelet_type) \
+            if LaneletType(config.driving_default_lanelet_type) is not None \
             else LaneletType.UNKNOWN
-        self._lanelet_types_backwards_compatible = custom_default_lanelet_types.lanelet_types_backwards_compatible
+        self._lanelet_types_backwards_compatible = config.lanelet_types_backwards_compatible
         _user_bidirectional = None
         _user_one_way = None
         if user_one_way is not None:
             _user_one_way = set(map(lambda x: RoadUser(x), user_one_way))
         if user_bidirectional is not None:
             _user_bidirectional = set(map(lambda x: RoadUser(x), user_bidirectional))
 
@@ -143,15 +141,16 @@
         elif value == 'stop':
             self._lanelet_type = {LaneletType.SHOULDER}.union(self._default_lanelet_type)
         elif value == 'biking':
             self._lanelet_type = {LaneletType.BICYCLE_LANE}
         elif value == 'driving':
             self._lanelet_type = {LaneletType(self._driving_default_lanelet_type)}
         else:
-            self._lanelet_type = {LaneletType.UNKNOWN}.union(self._default_lanelet_type)
+            logging.warning("ConversionLanelet::lanelet_type: Unknown lane type: {}".format(value))
+            self._lanelet_type = {LaneletType(self._driving_default_lanelet_type)}
 
     @property
     def lanelet_id(self) -> int:
         """Get or set id of this lanelet.
 
         :return: The ID of the lanelet.
         :rtype: int
@@ -436,34 +435,32 @@
 
     def move_border(
         self,
         mirror_border: str,
         mirror_interval: Tuple[float, float],
         distance: np.ndarray,
         adjacent_lanelet: "ConversionLanelet",
-        precision: float
+        precision: float,
+        transformer: Transformer
     ):
         """Move vertices of one border by mirroring other border with
         a specified distance.
 
         :param mirror_border: Which border to mirror, either 'left' or 'right'.
-        :type mirror_border: str
         :param mirror_interval: Tuple of two values, specifying start and end of mirroring.
-        :type mirror_interval: Tuple[float, float]
         :param distance: Specifying distance at start and at end of mirroring
-        :type distance: np.ndarray
         :param adjacent_lanelet: The adjacent conversion lanelet.
-        :type adjacent_lanelet: ConversionLanelet
         :param precision: Specifies precision with which to convert the plane group to lanelet w. mirroring
-        :type precision: float
+        :param transformer: Coordinate projection transformer.
         """
         if mirror_border == "left":
             distance[:] = [-1 * x for x in distance]
 
         lanelet = self.parametric_lane_group.to_lanelet_with_mirroring(
+            transformer=transformer,
             mirror_border=mirror_border,
             distance=distance,
             mirror_interval=mirror_interval,
             adjacent_lanelet=adjacent_lanelet,
             precision=precision,
         )
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/common/conversion_lanelet_network.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/conversion_lanelet_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 """Module to enhance LaneletNetwork class,
 so it can be used for conversion from the opendrive format."""
 import itertools
+import logging
 import warnings
 from typing import List, Optional, Tuple
 from queue import Queue
 import numpy as np
+import shapely
+from shapely.validation import make_valid
+from pyproj import Transformer
 
 from commonroad.scenario.lanelet import LaneletNetwork, StopLine
 from commonroad.scenario.intersection import IntersectionIncomingElement, Intersection
 from commonroad.scenario.traffic_sign import TrafficLightDirection, TrafficLight, TrafficSign
 
-from crdesigner.map_conversion.osm2cr import config
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
-
+from crdesigner.config.config import OpenDRIVEConversionParams
+from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.common.utils import convert_to_new_lanelet_id
 from crdesigner.map_conversion.common.conversion_lanelet import ConversionLanelet
 from crdesigner.map_conversion.common.utils import generate_unique_id
 
 
 class ConversionLaneletNetwork(LaneletNetwork):
     """
     Add functions to LaneletNetwork which further enable it to modify its Lanelets.
-    This class is being used in Opendrive and Lanelet2 format conversions
+    This class is being used in OpenDrive and Lanelet2 format conversions
     """
 
-    def __init__(self, config):
-        """Initializes a ConversionLaneletNetwork"""
+    def __init__(self, config: OpenDRIVEConversionParams = OpenDRIVEConversionParams(),
+                 transformer: Optional[Transformer] = None):
+        """
+        Initializes a ConversionLaneletNetwork
+
+        :param config: OpenDRIVE config parameters.
+        :param transformer: Coordinate projection transformer.
+        """
         super().__init__()
-        self.config = config
+        self._config = config
         self._old_lanelet_ids = {}
+        self._transformer = transformer
 
     def old_lanelet_ids(self) -> dict:
         """Get the old lanelet ids.
 
         :return: Dict containing all old lanelet IDs.
         :rtype: dict
         """
@@ -308,16 +318,16 @@
             if not lanelet.successor and np.allclose(
                     lanelet.left_vertices[-1], lanelet.right_vertices[-1]
             ):
                 lanelet_join = True
 
             if lanelet_join or lanelet_split:
                 js_targets.append(
-                    _JoinSplitTarget(self, lanelet, lanelet_split, lanelet_join,
-                                     self.config.precision)
+                    _JoinSplitTarget(self, lanelet, lanelet_split, lanelet_join, self._transformer,
+                                     self._config.precision)
                 )
 
         for js_target in js_targets:
             js_target.determine_apt_js_pairs()
             js_target.move_borders()
             js_target.add_adjacent_predecessor_or_successor()
 
@@ -686,16 +696,27 @@
         :rtype: bool
         """
         for incoming_lane in intersection_map.keys():
             for successor in self.find_lanelet_by_id(incoming_lane).successor:
                 if successor != lanelet.lanelet_id:
                     successor_lane_polygon = self.find_lanelet_by_id(successor).polygon
                     lanelet_polygon = lanelet.polygon
-                    if successor_lane_polygon.shapely_object.intersects(lanelet_polygon.shapely_object):
-                        return True
+                    if not lanelet_polygon.shapely_object.is_valid:
+                        make_valid(lanelet_polygon.shapely_object)
+                    if not successor_lane_polygon.shapely_object.is_valid:
+                        make_valid(successor_lane_polygon.shapely_object)
+                    try:
+                        if successor_lane_polygon.shapely_object.intersects(lanelet_polygon.shapely_object):
+                            return True
+                    except shapely.errors.GEOSException:
+                        logging.error("ConversionLaneletNetwork::check_if_lanelet_in_intersection: "
+                                      "Invalid lanelet shape lanelet {} or {}. "
+                                      "We assume this lanelet is not part of "
+                                      "the intersection.".format(successor, lanelet.lanelet_id))
+                        continue
         return False
 
     def check_if_successor_is_intersecting(self, intersection_map, successors_list) -> bool:
         """
         Check if successors of an incoming intersect with successors of other incoming of the intersection
         using the shapely crosses method.
 
@@ -745,15 +766,15 @@
         # take the incomings which have less than 90 degrees in between
         index = 0
         min_angle = 360
         while index < len(incomings):
             angle = angles[index][1] - angles[prev][1]
             if angle < 0:
                 angle += 360
-            if angle > config.LANE_SEGMENT_ANGLE and angle <= 180 - config.LANE_SEGMENT_ANGLE and angle < min_angle:
+            if self._config.lane_segment_angle < angle <= 180 - self._config.lane_segment_angle and angle < min_angle:
                 # is left of the previous incoming
                 is_left_of = angles[prev][0]
                 data_index = angles[index][0]
                 incomings[data_index].left_of = incomings[is_left_of].incoming_id
                 min_angle = angle
                 if abs(prev) >= len(incomings):
                     max_angle = 360
@@ -818,15 +839,15 @@
         Find all directions of an incoming lane's successors
 
         :param incoming_lane: incoming lane from intersection
         :type incoming_lane: :class:`ConversionLanelet`
         :return: Dict containing the directions "left", "right" or "through"
         :rtype: dict
         """
-        straight_threshold_angel = config.INTERSECTION_STRAIGHT_THRESHOLD
+        straight_threshold_angel = self._config.intersection_straight_threshold
         assert 0 < straight_threshold_angel < 90
 
         angels = {}
         directions = {}
 
         for successor in incoming_lane.successor:
             # only use the last three waypoints of the incoming for angle calculation
@@ -1106,35 +1127,41 @@
         if _mode == 2
     :var linking_side str: Side on which the split/join happens, either "left" or "right"
     :var _js_pairs list: List of :class:`._JoinSplitPair` elements
     :var _single_lanelet_operation bool: Indicates whether only one lanelet and its adjacent lanelet can be used for the
         join/split
     """
 
-    def __init__(
-        self,
-        lanelet_network: ConversionLaneletNetwork,
-        main_lanelet: ConversionLanelet,
-        split: bool,
-        join: bool,
-        precision: float,
-    ):
+    def __init__(self,lanelet_network: ConversionLaneletNetwork, main_lanelet: ConversionLanelet, split: bool,
+                 join: bool, transformer: Optional[Transformer] = None,
+                 precision: float = OpenDRIVEConversionParams.precision):
+        """
+
+        :param lanelet_network: LaneletNetwork where join/split occurs.
+        :param main_lanelet: Lanelet where split starts or join ends.
+        :param split: Boolean indicating whether a lanelet split should be performed.
+        :param join: Boolean indicating whether a lanelet join should be performed.
+        :param transformer: Coordinate projection transformer.
+        :param precision: precision with which to convert plane group to lanelet
+        """
+
         self.main_lanelet = main_lanelet
         self.lanelet_network = lanelet_network
         if split and join:
             self._mode = 2
         elif split:
             self._mode = 1
         else:
             self._mode = 0
         self.change_width = None
         self.linking_side = None
         self._js_pairs = []
         self._single_lanelet_operation = False
         self.precision = precision
+        self._transformer = transformer
 
     @property
     def split(self) -> bool:
         """Lanelet splits at start.
 
         :return: True if lanelet splits from other lanelet at start.
         :rtype: bool
@@ -1261,15 +1288,15 @@
         for js_pair in js_pairs:
             [pos_start, pos_end] = js_pair.change_interval
             distance = np.interp(
                 [pos_start + running_pos, pos_end + running_pos],
                 [0, length],
                 [width_start, width_end],
             )
-            js_pair.move_border(width=distance, linking_side=self.linking_side)
+            js_pair.move_border(width=distance, linking_side=self.linking_side, transformer=self._transformer)
             running_pos += pos_end - pos_start
 
     def _move_borders_if_split_and_join(self):
         """Move borders of lanelets if it is split and join.
 
         Calculate the new vertices twice:
         1. Only for the split (first pair in self._js_pairs)
@@ -1488,31 +1515,32 @@
             )
         return None
 
 
 class _JoinSplitPair:
     """Pair of lanelet whose border is changed and its adjacent neighbor."""
 
-    def __init__(self, lanelet, adjacent_lanelet, change_interval, precision):
+    def __init__(self, lanelet, adjacent_lanelet, change_interval,
+                 precision: float = OpenDRIVEConversionParams.precision):
         self.lanelet = lanelet
         self.adjacent_lanelet = adjacent_lanelet
         self.change_interval = change_interval
         self.precision = precision
 
-    def move_border(self, width: np.ndarray, linking_side: str) -> ConversionLanelet:
+    def move_border(self, width: np.ndarray, linking_side: str,
+                    transformer: Optional[Transformer] = None) -> ConversionLanelet:
         """Move border of self.lanelet.
 
         :param width: Start and end value of new width of lanelet.
-        :type width: np.ndarray
         :param linking_side: Side on which the split/join happens, either "left" or "right"
-        :type linking_side: str
+        :param transformer: Coordinate projection transformer.
         :return: Resulting lanelet after border movement.
-        :rtype: :class:`ConversionLanelet`
         """
         self.lanelet.move_border(
             mirror_border=linking_side,
             mirror_interval=self.change_interval,
             distance=width,
             adjacent_lanelet=self.adjacent_lanelet,
             precision=self.precision,
+            transformer=transformer
         )
         return self.lanelet
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/common/utils.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/utils.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/cr2lanelet.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/cr2lanelet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,117 +1,136 @@
 from typing import List, Optional, Tuple, Union, Dict
 
 import numpy as np
-from pyproj import Proj
+from pyproj import CRS, Transformer
 from commonroad.scenario.lanelet import Lanelet  # type: ignore
 from commonroad.scenario.traffic_sign import TrafficLight, TrafficSign  # type: ignore
-from crdesigner.map_conversion.lanelet2 import config
 
+from crdesigner.config.config import Lanelet2ConversionParams
+from crdesigner.map_conversion.common.utils import generate_unique_id
 from crdesigner.map_conversion.lanelet2.lanelet2 import OSMLanelet, Node, Way, WayRelation, RegulatoryElement
-from crdesigner.map_conversion.lanelet2.config import DEFAULT_PROJ_STRING
 
 
-def _convert_subtype_names(subtype: str) -> [str, bool]:
+def _convert_subtype_names(subtype: str, subtypes: List[str]) -> [str, bool]:
     """
     Function that converts names of some subtypes that are slightly different
     in two formats.
 
     :param subtype: name of the subtype of the lanelet
+    :param subtypes: lanelet2 subtypes that are available in commonroad
     :return: name of the subtype (converted if needed) and the boolean value that states if the subtype corresponds
         to one of the possible L2 format subtypes
     """
     subtype_in = False
-    if subtype in config.L2_LANELET_SUBTYPES:
+    if subtype in subtypes:
         subtype_in = True
         if subtype == "urban" or subtype == "country":
             subtype = "road"
         elif subtype == "busLane":
             subtype = "bus_lane"
         elif subtype == "bicycleLane":
             subtype = "bicycle_lane"
         elif subtype == "exitRamp":
             subtype = "exit"
         elif subtype == "sidewalk":
             subtype = "walkway"
     return subtype, subtype_in
 
 
-def _vertices_are_equal(vertices1: List[np.ndarray], vertices2: List[np.ndarray]) -> bool:
+def _vertices_are_equal(vertices1: List[np.ndarray], vertices2: List[np.ndarray],
+                        ways_are_equal_tolerance: float) -> bool:
     """
     Checks if two list of vertices are equal up to a tolerance.
 
     :param vertices1: First vertices to compare.
     :param vertices2: Second vertices to compare.
+    :param ways_are_equal_tolerance: value of the tolerance for which we mark ways as equal
     :return: True if every vertex in one list is nearly equal to the
         corresponding vertices at the same position in the other list.
     """
     if len(vertices1) != len(vertices2):
         return False
     diff = np.array(vertices1) - np.array(vertices2)
-    if np.abs(np.max(diff)) < config.WAYS_ARE_EQUAL_TOLERANCE:
+    if np.abs(np.max(diff)) < ways_are_equal_tolerance:
         return True
     return False
 
 
 class CR2LaneletConverter:
     """
     Class to convert CommonRoad lanelet to the OSM representation.
     """
 
-    def __init__(self, proj_string=None):
+    def __init__(self, config: Lanelet2ConversionParams = Lanelet2ConversionParams()):
         """
         Initialization of CR2LaneletConverter
         
-        :param proj_string: String name used for the initialization of the converter
+        :param config: Lanelet2 config parameters.
         """
-        if proj_string:
-            self.proj = Proj(proj_string)
-        else:
-            self.proj = Proj(DEFAULT_PROJ_STRING)
+        generate_unique_id(0)  # reset ID counter for next test case
+        self._config = config
+        self.transformer = None
         self.osm = None
-        self._id_count = -1
+        self._id_count = 1
         self.first_nodes, self.last_nodes = None, None
         self.left_ways, self.right_ways = None, None
         self.lanelet_network = None
-        self.origin_utm = None
+        self.origin_utm = (0, 0)
+
+    def _create_transformer(self, scenario):
+        # TODO: currently, we only consider `GeoTransformation.geo_reference`. The other specifications
+        #   there should be used if specified.
+        loc = scenario.location
+        proj_string_from = None
+        if loc is not None and loc.geo_transformation is not None:
+            proj_string_from = loc.geo_transformation.geo_reference
+        if proj_string_from is None:
+            proj_string_from = self._config.proj_string
+        crs_from = CRS(proj_string_from)
+        crs_to = CRS("ETRF89")
+        self.transformer = Transformer.from_proj(crs_from, crs_to)
 
     @property
     def id_count(self) -> int:
         """
         Internal counter for giving IDs to the members of the OSM.
         Each call returns the count and increases it by one.
 
         :return: current id count.
         """
         tmp = self._id_count
-        self._id_count -= 1
+        self._id_count += 1
         return tmp
 
     def __call__(self, scenario):
         """
         Convert a scenario to an OSM xml document.
 
         :param scenario: Scenario that will be used for conversion
         """
+        self._create_transformer(scenario)
         self.osm = OSMLanelet()
         self.lanelet_network = scenario.lanelet_network
         self.first_nodes = {}  # saves first left and right node | dict() but with a faster execution
         self.last_nodes = {}  # saves last left and right node
         self.left_ways = {}
         self.right_ways = {}
-        if scenario.location is not None and not isinstance(scenario.location.gps_longitude, str) and\
-                abs(scenario.location.gps_longitude) <= 180 and abs(scenario.location.gps_latitude) <= 90:
-            self.origin_utm = self.proj(scenario.location.gps_longitude, scenario.location.gps_latitude)
-        elif scenario.location is not None and isinstance(scenario.location.gps_longitude, str) and\
-                abs(float(scenario.location.gps_longitude)) <= 180 and abs(float(scenario.location.gps_latitude)) <= 90:
-            self.origin_utm = self.proj(float(scenario.location.gps_longitude), float(scenario.location.gps_latitude))
-        else:
-            self.proj = Proj(DEFAULT_PROJ_STRING)
-            # set origin point (TUM MI building) in default UTM 32 zone
-            self.origin_utm = self.proj(config.TUM_MI_BUILDING_X, config.TUM_MI_BUILDING_Y)
+        if self._config.translate:
+            if scenario.location is not None and not isinstance(scenario.location.gps_longitude, str) and\
+                    abs(scenario.location.gps_longitude) <= 180 and abs(scenario.location.gps_latitude) <= 90:
+                self.origin_utm = self.transformer.transform(scenario.location.gps_latitude,
+                                                              scenario.location.gps_longitude)
+            elif scenario.location is not None and isinstance(scenario.location.gps_longitude, str) and\
+                    abs(float(scenario.location.gps_longitude)) <= 180 \
+                    and abs(float(scenario.location.gps_latitude)) <= 90:
+                self.origin_utm = \
+                    self.transformer.transform(float(scenario.location.gps_latitude),
+                                                float(scenario.location.gps_longitude))
+            else:
+                self.origin_utm = self.transformer.transform(0, 0)
 
             # convert lanelets
         for lanelet in scenario.lanelet_network.lanelets:
             self._convert_lanelet(lanelet)
 
         # convert traffic signs
         for traffic_sign in scenario.lanelet_network.traffic_signs:
@@ -139,15 +158,15 @@
             for lightID in ll.traffic_lights:
                 # find the coordinates of the CR traffic light
                 # and check them with traffic light in L2 format that we have created
 
                 # x,y = self.lanelet_network._traffic_lights[lightID].position
                 x, y = self.lanelet_network.find_traffic_light_by_id(lightID).position
 
-                xsign, ysign = self.proj(self.origin_utm[0] + x, self.origin_utm[1] + y, inverse=True)
+                xsign, ysign = self.transformer.transform(self.origin_utm[0] + x, self.origin_utm[1] + y)
                 for way in self.osm.ways:
                     if self.osm.find_way_by_id(way).tag_dict.get('type') == "traffic_light":
 
                         nx = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lon
                         ny = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lat
 
                         if str(xsign) == nx and str(ysign) == ny:
@@ -167,32 +186,33 @@
 
     def _convert_traffic_light(self, light: TrafficLight):
         """
         Add traffic light to the lanelet2 format
         """
         traffic_light_id = self.id_count
         # create a node that represent the sign position
-        x1, y1 = self.proj(self.origin_utm[0] + light.position[0], self.origin_utm[1] + light.position[1], inverse=True)
+        x1, y1 = self.transformer.transform(self.origin_utm[0] + light.position[0],
+                                            self.origin_utm[1] + light.position[1])
 
         id1 = self.id_count
 
         # since 3 nodes are needed to represent the sign in the l2 format (only 1 in the cr format)
         # create another 2 nodes that are close to the first one
 
-        x2, y2 = self.proj(self.origin_utm[0] + light.position[0] + 0.1, self.origin_utm[1] + light.position[1] + 0.1,
-                           inverse=True)
-        x3, y3 = self.proj(self.origin_utm[0] + light.position[0] - 0.1, self.origin_utm[1] + light.position[1] - 0.1,
-                           inverse=True)
+        x2, y2 = self.transformer.transform(self.origin_utm[0] + light.position[0] + 0.1,
+                                             self.origin_utm[1] + light.position[1] + 0.1)
+        x3, y3 = self.transformer.transform(self.origin_utm[0] + light.position[0] - 0.1,
+                                             self.origin_utm[1] + light.position[1] - 0.1)
         id2 = self.id_count
         id3 = self.id_count
 
         # creating and adding those nodes to our osm
-        self.osm.add_node(Node(id1, y1, x1))
-        self.osm.add_node(Node(id2, y2, x2))
-        self.osm.add_node(Node(id3, y3, x3))
+        self.osm.add_node(Node(id1, y1, x1, autoware=self._config.autoware))
+        self.osm.add_node(Node(id2, y2, x2, autoware=self._config.autoware))
+        self.osm.add_node(Node(id3, y3, x3, autoware=self._config.autoware))
 
         # get the first light color as subtype
         traffic_light_subtype = light.cycle[0].state.value
 
         self.osm.add_way(Way(traffic_light_id, [id1, id2, id3],
                              tag_dict={"subtype": traffic_light_subtype, "type": "traffic_light"}))
 
@@ -218,15 +238,15 @@
                 nx = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lon
                 ny = self.osm.find_node_by_id(self.osm.find_way_by_id(way).nodes[0]).lat
 
                 # go through the lanelets to find the lanelet that has the matching traffic_sign in its attribute
                 for ll in self.lanelet_network.lanelets:
                     for traffic_sign_id in ll.traffic_signs:
                         x, y = self.lanelet_network.find_traffic_sign_by_id(traffic_sign_id).position
-                        x_sign, y_sign = self.proj(self.origin_utm[0] + x, self.origin_utm[1] + y, inverse=True)
+                        x_sign, y_sign = self.transformer.transform(self.origin_utm[0] + x, self.origin_utm[1] + y)
                         # have to map the signs based on the position,
                         # as the same 2 signs do not have the same ID in L2 and CR format
                         if nx == str(x_sign) and ny == str(y_sign):
                             # position matches, found the corresponding lanelet with selected sign
                             # extract the way that corresponds to our lanelet
                             # sign -> lanelet -> way (right+left) -> wayrelation
                             right_way_id = self.right_ways[ll.lanelet_id]
@@ -255,21 +275,21 @@
             if ll.stop_line:
                 # found a lanelet with a stop line
                 stop_line = ll.stop_line
                 # stop line has 2 points (each point has x and y coordinates)
                 stop_line_start = stop_line.start
                 stop_line_end = stop_line.end
                 # transform the x and y coordinates to the L2 coordinate system
-                x_start, y_start = self.proj(self.origin_utm[0] + stop_line_start[0],
-                                             self.origin_utm[1] + stop_line_start[1], inverse=True)
-                x_end, y_end = self.proj(self.origin_utm[0] + stop_line_end[0], self.origin_utm[1] + stop_line_end[1],
-                                         inverse=True)
+                x_start, y_start = self.transformer.transform(self.origin_utm[0] + stop_line_start[0],
+                                                              self.origin_utm[1] + stop_line_start[1])
+                x_end, y_end = self.transformer.transform(self.origin_utm[0] + stop_line_end[0],
+                                                          self.origin_utm[1] + stop_line_end[1])
                 # create nodes from the points and add them to the osm
-                node_start = Node(self.id_count, y_start, x_start)
-                node_end = Node(self.id_count, y_end, x_end)
+                node_start = Node(self.id_count, y_start, x_start, autoware=self._config.autoware)
+                node_end = Node(self.id_count, y_end, x_end, autoware=self._config.autoware)
                 self.osm.add_node(node_start)
                 self.osm.add_node(node_end)
                 # create a way from newly created nodes and add it to the osm
                 stop_line_way = Way(self.id_count, [node_start.id_, node_end.id_], tag_dict={"type": "stop_line"})
                 self.osm.add_way(stop_line_way)
                 # map the way with the lanelet
                 dict_stop_lines[ll.lanelet_id] = stop_line_way.id_
@@ -292,15 +312,15 @@
         right_of_ways = []
         ref_line = []
         # subtype from the L2 format, i.e. "de205" -> CR format, i.e. "205"
         subtype = self.osm.find_way_by_id(way).tag_dict.get('subtype')[2:]
         # iterate through sign IDs to find the corresponding sign with that subtype
         sign_name = ""
         sign_found = False
-        for country in config.CR2LANELET_SUPPORTED_COUNTRIES_LIST:
+        for country in self._config.supported_countries:
             if sign_found is True:
                 break
             for countrySign in country:
                 if subtype == str(countrySign.value):
                     sign_name = countrySign.name
                     sign_found = True
         # no need to add the speed limit sign to the way of rel
@@ -323,43 +343,44 @@
         """
         Convert a traffic sign to way which will be mapped by RightOfWay Regulatory element
         Add the resulting right of way relation to the OSM.
 
         :param sign: Traffic Sign to be converted.
         """
         # create a node that represent the sign position
-        x1, y1 = self.proj(self.origin_utm[0] + sign.position[0], self.origin_utm[1] + sign.position[1], inverse=True)
+        x1, y1 = self.transformer.transform(self.origin_utm[0] + sign.position[0],
+                                             self.origin_utm[1] + sign.position[1])
         id1 = self.id_count
 
         # since 2 nodes are needed to represent the sign in the l2 format (only 1 in the cr format)
         # create another node that is close to the first one
-        x2, y2 = self.proj(self.origin_utm[0] + sign.position[0] + 0.25, self.origin_utm[1] + sign.position[1] + 0.25,
-                           inverse=True)
+        x2, y2 = self.transformer.transform(self.origin_utm[0] + sign.position[0] + 0.25,
+                                             self.origin_utm[1] + sign.position[1] + 0.25)
         id2 = self.id_count
 
         # creating and adding those nodes to our osm
-        self.osm.add_node(Node(id1, y1, x1))
-        self.osm.add_node(Node(id2, y2, x2))
+        self.osm.add_node(Node(id1, y1, x1, autoware=self._config.autoware))
+        self.osm.add_node(Node(id2, y2, x2, autoware=self._config.autoware))
 
         # matching the type of the traffic sign
         sign_id = sign.traffic_sign_elements[0].traffic_sign_element_id
         val = ""
-        for country in config.CR2LANELET_SUPPORTED_COUNTRIES_LIST:
+        for country in self._config.supported_countries:
             for k in country:
                 if k == sign_id:
                     val = k.value
 
         traffic_sign_wayid = self.id_count
         virtual = sign.virtual
 
         # extract the country name of the sign, so we can map it to a dictionary
         sign_country_name = str(type(sign.traffic_sign_elements[0].traffic_sign_element_id).__name__)
 
         # map the supported countries to their 2 letter prefixs
-        country_prefix_dictionary = config.CR2LANELET_SUPPORTED_COUNTRIES_PREFIX_DICTIONARY
+        country_prefix_dictionary = self._config.supported_countries_prefixes
 
         subtype = country_prefix_dictionary[sign_country_name]
 
         # if it is a speed sign, don't add way but add regulatory element "speed_limit"
         self.osm.add_way(Way(traffic_sign_wayid, [id1, id2],
                              tag_dict={"subtype": subtype + str(val), "type": "traffic_sign", "virtual": str(virtual)}))
 
@@ -389,15 +410,15 @@
             right_way_id = right_way.id_
 
         # get the lanelet type of the lanelet we are converting
         subtype = ""
         if len(lanelet.lanelet_type) > 0:
             subtype = list(lanelet.lanelet_type)[0].value
         # have to convert the names as they are slightly different in both formats
-        subtype, subtype_in = _convert_subtype_names(subtype)
+        subtype, subtype_in = _convert_subtype_names(subtype, self._config.supported_lanelet2_subtypes)
 
         # append left and right way
         self.left_ways[lanelet.lanelet_id] = left_way_id
         self.right_ways[lanelet.lanelet_id] = right_way_id
 
         # create the way relation
         way_rel = WayRelation(self.id_count, left_way_id, right_way_id, tag_dict={"type": "lanelet"})
@@ -443,16 +464,16 @@
         else:
             first_left_node = pot_first_left_node
             last_left_node = pot_last_left_node
             left_nodes = self._create_nodes_from_vertices(lanelet.left_vertices[start_index:end_index])
         if right_way_id:
             first_right_node: Optional[str]
             last_right_node: Optional[str]
-            first_right_node, last_right_node = self._get_first_and_last_nodes_from_way\
-            (right_way_id, lanelet.adj_right_same_direction)
+            first_right_node, last_right_node = \
+                self._get_first_and_last_nodes_from_way(right_way_id, lanelet.adj_right_same_direction)
         else:
             first_right_node = pot_first_right_node
             last_right_node = pot_last_right_node
             right_nodes = self._create_nodes_from_vertices(lanelet.right_vertices[start_index:end_index])
 
         if first_left_node:
             left_nodes.insert(0, first_left_node)
@@ -484,16 +505,20 @@
         Create nodes and add them to the OSM.
 
         :param vertices: List of vertices from a lanelet boundary.
         :return: Ids of nodes which were created.
         """
         nodes = []
         for vertex in vertices:
-            lon, lat = self.proj(self.origin_utm[0] + vertex[0], self.origin_utm[1] + vertex[1], inverse=True)
-            node = Node(self.id_count, lat, lon)
+            lat, lon = self.transformer.transform(self.origin_utm[0] + vertex[0], self.origin_utm[1] + vertex[1])
+            if self._config.use_local_coordinates:
+                node = Node(self.id_count, lat, lon, autoware=self._config.autoware, local_x=vertex[0],
+                            local_y=vertex[1])
+            else:
+                node = Node(self.id_count, lat, lon, autoware=self._config.autoware)
             nodes.append(node.id_)
             self.osm.add_node(node)
         return nodes
 
     def _get_potential_right_way(self, lanelet) -> Union[None, int]:
         """
         Check if a shared right boundary with another lanelet can be transformed
@@ -507,15 +532,15 @@
                 potential_right_way = self.left_ways.get(lanelet.adj_right)
             else:
                 potential_right_way = self.right_ways.get(lanelet.adj_right)
             if potential_right_way:
                 adj_right = self.lanelet_network.find_lanelet_by_id(lanelet.adj_right)
                 vertices = (
                     adj_right.left_vertices if lanelet.adj_right_same_direction else adj_right.right_vertices[::-1])
-                if _vertices_are_equal(lanelet.right_vertices, vertices):
+                if _vertices_are_equal(lanelet.right_vertices, vertices, self._config.ways_are_equal_tolerance):
                     return potential_right_way
 
         return None
 
     def _get_potential_left_way(self, lanelet) -> Union[None, int]:
         """
         Check if a shared left boundary with another lanelet can be transformed
@@ -529,15 +554,15 @@
                 potential_left_way = self.right_ways.get(lanelet.adj_left)
             else:
                 potential_left_way = self.left_ways.get(lanelet.adj_left)
             if potential_left_way:
                 adj_left = self.lanelet_network.find_lanelet_by_id(lanelet.adj_left)
                 vertices = (
                     adj_left.right_vertices if lanelet.adj_left_same_direction else adj_left.left_vertices[::-1])
-                if _vertices_are_equal(lanelet.left_vertices, vertices):
+                if _vertices_are_equal(lanelet.left_vertices, vertices, self._config.ways_are_equal_tolerance):
                     return potential_left_way
 
         return None
 
     def _get_shared_first_nodes_from_other_lanelets(self, lanelet: Lanelet) \
             -> Tuple[Union[str, None], Union[str, None]]:
         """
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/lanelet2.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,60 @@
 
 
 class Node:
     """
     OSM Node.
     """
 
-    def __init__(self, id_, lat, lon):
+    def __init__(self, id_, lat, lon, ele: float = 0.0, autoware: bool = False,
+                 local_x: Optional[float] = None, local_y: Optional[float] = None):
         """
         Initialization of Node
         
         :param lat: Latitude geo position information
         :param lon: Longitude geo position information
+        :param ele: Elevation (height information)
+        :param autoware: Boolean indicating whether the map is autoware-compatible.
+        :param local_x: local x-position instead of latitude/longitude (lon/lat values have no meaning)
+        :param local_y: local y-position instead of latitude/longitude (lon/lat values have no meaning)
         """
         self.id_ = str(id_)
         self.lat = str(lat)
         self.lon = str(lon)
+        self.ele = str(ele)
+        self.autoware = autoware
+        self.local_x = local_x
+        self.local_y = local_y
 
     def serialize_to_xml(self) -> etree:
         """
         Serializes the Node object to the xml format
         """
         node = etree.Element("node")
         node.set("id", self.id_)
         node.set("action", "modify")
         node.set("visible", "true")
+        node.set("version", "1")
         node.set("lat", self.lat)
         node.set("lon", self.lon)
+        if self.local_x is not None and self.local_y is not None:
+            local_x = etree.SubElement(node, "tag")
+            local_x.set("k", "local_x")
+            local_x.set("v", str(self.local_x))
+            local_y = etree.SubElement(node, "tag")
+            local_y.set("k", "local_y")
+            local_y.set("v", str(self.local_y))
+            node.append(local_x)
+            node.append(local_y)
+        if self.ele != "0.0" or self.autoware:
+            ele = etree.SubElement(node, "tag")
+            ele.set("k", "ele")
+            ele.set("v", self.ele)
+            node.append(ele)
+
         return node
 
 
 class Way:
     """
     OSM Way
     """
@@ -53,14 +78,15 @@
         """
         Serializes the Way object to the xml format
         """
         way = etree.Element("way")
         way.set("id", self.id_)
         way.set("action", "modify")
         way.set("visible", "true")
+        way.set("version", "1")
         for node in self.nodes:
             xml_node = etree.SubElement(way, "nd")
             xml_node.set("ref", node)
         for tag_key, tag_value in self.tag_dict.items():
             xml_node = etree.SubElement(way, "tag")
             xml_node.set("k", tag_key)
             xml_node.set("v", tag_value)
@@ -95,14 +121,15 @@
         """
         Serializes the WayRelation object to the xml format
         """
         rel = etree.Element("relation")
         rel.set("id", self.id_)
         rel.set("action", "modify")
         rel.set("visible", "true")
+        rel.set("version", "1")
         right_way = etree.SubElement(rel, "member")
         right_way.set("type", "way")
         right_way.set("ref", self.right_way)
         right_way.set("role", "right")
         left_way = etree.SubElement(rel, "member")
         left_way.set("type", "way")
         left_way.set("ref", self.left_way)
@@ -146,14 +173,15 @@
     def serialize_to_xml(self) -> etree.Element:
         """
         Serializes the RegulatoryElement object to the xml format
         """
         rel = etree.Element("relation")
         rel.set("id", self.id_)
         rel.set("action", "modify")
+        rel.set("version", "1")
         rel.set("visible", "true")
         for r in self.refers:
             right_way = etree.SubElement(rel, "member")
             right_way.set("type", "way")
             right_way.set("ref", r)
             right_way.set("role", "refers")
         for y in self.yield_ways:
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/lanelet2_parser.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2_parser.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/lanelet2/lanelet2cr.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/lanelet2/lanelet2cr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from collections import defaultdict
 from typing import List, Optional, Tuple, Dict, Union
-
 from shapely.geometry import LineString  # type: ignore
 import numpy as np
-from pyproj import Proj
+from pyproj import Transformer, CRS
+import logging
 
 from commonroad.scenario.lanelet import StopLine, LineMarking, RoadUser, Lanelet, LaneletNetwork  # type: ignore
 from commonroad.scenario.traffic_sign import (TrafficSignElement, TrafficSignIDGermany,  # type: ignore
                                               TrafficSignIDUsa,  # type: ignore
                                               TrafficSignIDZamunda, TrafficLightCycleElement,
                                               TrafficLightState, TrafficLightDirection)  # type: ignore
-from commonroad.scenario.scenario import Scenario, ScenarioID, TrafficSign, Location, TrafficLight  # type: ignore
+from commonroad.scenario.scenario import Scenario, ScenarioID, TrafficSign, Location, TrafficLight, \
+    GeoTransformation  # type: ignore
 
+from crdesigner.map_conversion.lanelet2.lanelet2 import OSMLanelet
 from crdesigner.map_conversion.common.utils import generate_unique_id
 from crdesigner.map_conversion.common.conversion_lanelet import ConversionLanelet
 from crdesigner.map_conversion.common.conversion_lanelet_network import \
     ConversionLaneletNetwork
 from crdesigner.map_conversion.common.utils import convert_to_new_lanelet_id
 from crdesigner.map_conversion.lanelet2.lanelet2 import WayRelation, Node, RegulatoryElement, Way
-from crdesigner.map_conversion.osm2cr.converter_modules.utility.geometry import (point_to_line_distance,
-                                                                                 distance as point_to_polyline_distance)
-from crdesigner.configurations.get_configs import get_configs
-from crdesigner.map_conversion.lanelet2 import config
+from crdesigner.map_conversion.common.geometry import (point_to_line_distance,
+                                                       distance as point_to_polyline_distance)
+from crdesigner.config.config import Lanelet2ConversionParams, GeneralParams
+
+
+date_strftime_format = "%d-%b-%y %H:%M:%S"
+message_format = "%(asctime)s - %(levelname)s - %(message)s"
+logging.basicConfig(level=logging.INFO, format=message_format, datefmt=date_strftime_format)
 
 
 def _add_closest_traffic_sign_to_lanelet(lanelets: List[Lanelet], traffic_signs: List[TrafficSign]) -> set:
     """
     Assumes that it is given traffic signs and lanelets that should get matched (all to each)
     Each lanelet gets assigned exactly the single traffic sign closest to it
     Does nothing if the list of traffic signs is empty
@@ -148,108 +154,118 @@
     if state == "yellow":
         cycle_list.append(TrafficLightCycleElement(TrafficLightState.YELLOW, 5))
     else:
         cycle_list.append(TrafficLightCycleElement(TrafficLightState.INACTIVE, 5))
     return cycle_list
 
 
-def _two_vertices_coincide(vertices1: np.ndarray, vertices2: np.ndarray) -> bool:
+def _two_vertices_coincide(vertices1: np.ndarray, vertices2: np.ndarray,
+                           adjacent_way_distance_tolerance: float) -> bool:
     """
-    Check if two vertices coincide and describe the same trajectory.
-    For each vertex of vertices2 the minimal distance to the trajectory
+    Check if two vertices coincide and describe the same linestring.
+    For each vertex of vertices2 the minimal distance to the linestring
     described by vertices1 is calculated. If this distance crosses a certain
     threshold, the vertices are deemed to be different.
 
     :param vertices1: List of vertices which describe first trajectory.
     :param vertices2: List of vertices which describe second trajectory.
+    :param adjacent_way_distance_tolerance: Threshold indicating adjacent ways.
     :return: True if the vertices coincide, else False.
     """
     segments = np.diff(vertices1, axis=0)
 
     for vert in vertices2:
         distances = np.empty([len(vertices1) + 1])
         distances[0] = np.linalg.norm(vert - vertices1[0])
         distances[-1] = np.linalg.norm(vert - vertices1[-1])
         for i, diff in enumerate(segments):
             distances[i + 1] = np.abs(np.cross(diff, vertices1[i] - vert)) / np.linalg.norm(diff)
-        if np.min(distances) > config.ADJACENT_WAY_DISTANCE_TOLERANCE:
+        if np.min(distances) > adjacent_way_distance_tolerance:
             return False
 
     return True
 
 
 class Lanelet2CRConverter:
     """
     Class to convert OSM to the Commonroad representation of Lanelets.
     """
 
-    def __init__(self, proj_string=None):
+    def __init__(self, lanelet2_config: Lanelet2ConversionParams = Lanelet2ConversionParams(),
+                 cr_config: GeneralParams = GeneralParams()):
         """
         Initialization of the Lanelet2CRConverter
 
-        :param proj_string:
-        """
-        if proj_string:
-            self.proj = Proj(proj_string)
-        else:
-            self.proj = Proj(config.DEFAULT_PROJ_STRING)
+        :param proj_string: Projection string used for conversion.
+        :param lanelet2_config: Lanelet2 conversion parameters.
+        :param cr_config: General config parameters.
+        """
+        self._config = lanelet2_config
+        self._cr_config = cr_config
+        crs_from = CRS("ETRF89")
+        crs_to = CRS(self._config.proj_string)
+        self.transformer = Transformer.from_proj(crs_from, crs_to)
         self._left_way_ids, self._right_way_ids = None, None
         self.first_left_pts, self.last_left_pts = None, None
         self.first_right_pts, self.last_right_pts = None, None
         self.osm = None
         self.lanelet_network = None
         self.origin_utm = None
 
-    def __call__(self, osm, detect_adjacencies: bool = True, left_driving_system: bool = False, ) -> \
-            Union[Scenario, None]:
+    def __call__(self, osm: OSMLanelet) -> Union[Scenario, None]:
         """
         Convert OSM to Scenario.
         For each lanelet in OSM format, we have to save their first and last
         point of the left and right boundaries to determine their predecessors,
         successors and adjacent neighbors.
 
         :param osm: OSM object which includes nodes, ways and lanelet relations.
-        :param detect_adjacencies: Compare vertices which might be adjacent. Set
-            to false if you consider it too computationally intensive.
-        :param left_driving_system: Set to true if map describes a left_driving_system.
         :return: A scenario with a lanelet network which describes the
             same map as the osm input.
         """
         # dicts to save relation of nodes to ways and lanelets
         # so the adjacencies can be determined
 
         self.osm = osm
         self._left_way_ids, self._right_way_ids = defaultdict(list), defaultdict(list)
         self.first_left_pts, self.last_left_pts = defaultdict(list), defaultdict(list)
         self.first_right_pts, self.last_right_pts = defaultdict(list), defaultdict(list)
         if len(self.osm.nodes.values()) == 0:
-            print("__Warning__: Selected Scenario is empty.")
+            logging.warning("Lanelet2CRConverter: Selected Scenario is empty.")
             return None
 
-        origin = next(iter(self.osm.nodes.values()))  # use a random node as origin
-        self.origin_utm = self.proj(origin.lon, origin.lat)
-        scenario_id = ScenarioID(country_id=config.DEFAULT_SCENARIO_COUNTRY_ID,
-                                 map_name=config.DEFAULT_SCENARIO_MAP_NAME, map_id=config.DEFAULT_SCENARIO_MAP_ID)
-        scenario = Scenario(dt=config.GLOBAL_TIMESTEP, scenario_id=scenario_id,
-                            location=Location(gps_latitude=origin.lat, gps_longitude=origin.lon))
-        self.lanelet_network = ConversionLaneletNetwork(get_configs().opendrive)
+        origin_lat = min([node.lat for node in self.osm.nodes.values()])
+        origin_lon = min([node.lon for node in self.osm.nodes.values()])  # use left-most lower corner as origin
+        logging.info("Lanelet2CRConverter OSM bounds - lower-left: {}/{} - "
+                     "upper right {}/{}".format(origin_lat, origin_lon,
+                                                max([node.lat for node in self.osm.nodes.values()]),
+                                                max([node.lon for node in self.osm.nodes.values()])))
+        if self._config.translate:
+            self.origin_utm = self.transformer.transform(origin_lat, origin_lon)
+        else:
+            self.origin_utm = (0, 0)
+        scenario_id = ScenarioID(country_id=self._cr_config.country_id,
+                                 map_name=self._cr_config.map_name, map_id=self._cr_config.map_id)
+        scenario = Scenario(dt=self._cr_config.time_step_size, scenario_id=scenario_id,
+                            location=Location(gps_latitude=origin_lat, gps_longitude=origin_lon))
+        self.lanelet_network = ConversionLaneletNetwork()
 
         speed_limits = {}
         speed_limit_lanelets = {}  # type: ignore
         for speed_limit_key in osm.speed_limit_signs.keys():
             light_id = generate_unique_id()
             speed_limits[speed_limit_key] = light_id
-            speed_limit_lanelets[speed_limit_key] = []  # scenario.add_objects(speed_limit)
+            speed_limit_lanelets[speed_limit_key] = []
 
         for way_rel in osm.way_relations.values():
             # add traffic sign id to traffic signs for speed limit
             # create dictionary for mapping of osm id to cr id and keep id constant
             # later add speed limit as traffic sign
-            lanelet = self._way_rel_to_lanelet(way_rel, detect_adjacencies, left_driving_system, speed_limits,
-                                               speed_limit_lanelets)
+            lanelet = self._way_rel_to_lanelet(way_rel, self._config.adjacencies, self._config.left_driving,
+                                               speed_limits, speed_limit_lanelets)
             if lanelet is not None:
                 self.lanelet_network.add_lanelet(lanelet)
 
         # dictionary
         new_ids = self.lanelet_network.convert_all_lanelet_ids()
 
         # right of way conversion
@@ -267,39 +283,46 @@
                 yield_signs_stop_lines_id = _add_stop_line_to_lanelet(
                         [self.lanelet_network.find_lanelet_by_id(i) for i in yield_lanelets], stop_lines)
                 # add any used traffic sign
                 for s in (priority_signs | yield_signs_lanelets | {y for y in yield_signs if
                                                                    y.traffic_sign_id in yield_signs_stop_lines_id}):
                     self.lanelet_network.add_traffic_sign(s, set())
             except NotImplementedError as e:
-                print(str(e))
+                logging.error("Lanelet2CRConverter: " + str(e))
 
         # speed limit sign conversion
         for speed_limit_key in osm.speed_limit_signs.keys():
             speed, traffic_sign_id = osm.speed_limit_signs[speed_limit_key]
             light_id = speed_limits[speed_limit_key]
             first_occurrence = {self.lanelet_network._old_lanelet_ids[l_id] for l_id in
                                 speed_limit_lanelets[speed_limit_key]}
             position = self.lanelet_network.find_lanelet_by_id(
                     self.lanelet_network._old_lanelet_ids[speed_limit_lanelets[speed_limit_key][0]]).left_vertices[0]
             speed_limit = TrafficSign(light_id, [TrafficSignElement(traffic_sign_id, [speed])], first_occurrence,
                                       position, True)
             self.lanelet_network.add_traffic_sign(speed_limit,
                                                   first_occurrence)
-            # scenario.add_objects(speed_limit, first_occurrence)
 
         # traffic light conversion
         for way in osm.ways:
             if osm.ways[way].tag_dict.get('type') == 'traffic_light':
                 self.traffic_light_conversion(osm.ways[way], new_ids)
 
         for la in self.lanelet_network.lanelets:
             la.__class__ = Lanelet
         self.lanelet_network.__class__ = LaneletNetwork
-        scenario.add_objects(self.lanelet_network)        
+
+        # if lanelet2 map is a sub-map of another map, relations could be wrong
+        self.lanelet_network.cleanup_lanelet_references()
+        self.lanelet_network.cleanup_traffic_sign_references()
+        self.lanelet_network.cleanup_traffic_light_references()
+
+        scenario.add_objects(self.lanelet_network)
+
+        scenario.location.geo_transformation = GeoTransformation(geo_reference=self._config.proj_string)
 
         return scenario
     
     def traffic_light_conversion(self, traffic_light_way: Way, new_lanelet_ids: Dict[str, int]):
         """
         Converting a traffic light, which is formatted as Way in Lanelet2 format, to
         CommonRoad format
@@ -315,15 +338,15 @@
 
         # TL in L2 format is represented with 3 nodes, we will take the one in the middle
         node = self.osm.nodes[traffic_light_way.nodes[1]]
         node_x = node.lon
         node_y = node.lat
 
         # convert to CR space
-        x, y = self.proj(node_x, node_y)
+        x, y = self.transformer.transform(node_x, node_x)
         x -= self.origin_utm[0]
         y -= self.origin_utm[1]
         
         # need to assign lanelet to that trafficLight
         # find the traffic_light_relations corresponding to our traffic_light_way and add them to the list
         traffic_light_relations = []
         for tl_relation in self.osm.traffic_light_relations:
@@ -383,24 +406,26 @@
         priority_lanelets = []
         for i in right_of_way_rel.right_of_ways:
             # never create new lanelet ids here,
             # if they don't exist yet, they are never created
             if i in new_lanelet_ids.keys():
                 priority_lanelets.append(new_lanelet_ids[i])
             else:
-                print(f"Warning: some priority sign references non-existing lanelet {i}")
+                logging.warning("Lanelet2CRConverter::_right_of_way_to_traffic_sign: some priority sign "
+                                "references non-existing lanelet {}".format(i))
 
         yield_lanelets = []
         for i in right_of_way_rel.yield_ways:
             # never create new lanelet ids here,
             # if they don't exist yet, they are never created
             if i in new_lanelet_ids.keys():
                 yield_lanelets.append(new_lanelet_ids[i])
             else:
-                print(f"Warning: some yield sign references non-existing lanelet {i}")
+                logging.warning("Lanelet2CRConverter::_right_of_way_to_traffic_sign: some yield sign "
+                                "references non-existing lanelet {}".format(i))
 
         stop_lines = []
         for stop_line in right_of_way_rel.ref_line:
             # extract geometrical features
             stop_line_way = self.osm.find_way_by_id(stop_line)
             stop_line_way_vertices = self._convert_way_to_vertices(stop_line_way)
             start = stop_line_way_vertices[0]
@@ -458,37 +483,42 @@
 
             # find the traffic sign
             traffic_sign_found = False
             tsid = TrafficSignIDZamunda.STOP  # default sign
             for country in supported_country_list:
                 for countrySign in country:
                     if countrySign.value == filtered_traffic_sign_type_name:
-                        tsid = country(countrySign.value)
+                        # traffic sign ID 252 is replaced by 260
+                        if (country is TrafficSignIDGermany or country is TrafficSignIDZamunda) \
+                                and countrySign.value == "252":
+                            tsid = country("260")
+                        else:
+                            tsid = country(countrySign.value)
                         traffic_sign_found = True
                 if traffic_sign_found:
                     break
             if traffic_sign_found == 0:
                 raise NotImplementedError(f"Lanelet type {traffic_sign_way.tag_dict['subtype']} not implemented")
 
             # create the element of the traffic sign
             traffic_sign_element = TrafficSignElement(tsid, [])
 
             # extract position
-            x, y = self.proj(float(traffic_sign_node.lon), float(traffic_sign_node.lat))
+            x, y = self.transformer.transform(float(traffic_sign_node.lat), float(traffic_sign_node.lon))
             x -= self.origin_utm[0]
             y -= self.origin_utm[1]
             ref_t_id = convert_to_new_lanelet_id(traffic_sign_way.id_, new_lanelet_ids)
 
             # create the traffic sign
             traffic_sign = TrafficSign(ref_t_id, traffic_sign_elements=[traffic_sign_element], first_occurrence=set(),
                                        position=np.array([x, y]), virtual=virtual)
             # traffic sign names need to be universal(i.e."YIELD" should be the name of both German and USA Yield signs)
 
             # append the sign to either priority or yield signs
-            if tsid.name in config.PRIORITY_SIGNS:
+            if tsid.name in self._config.priority_signs:
                 priority_signs.append(traffic_sign)
             else:
                 yield_signs.append(traffic_sign)
 
         return priority_signs, yield_signs
 
     def _way_rel_to_lanelet(self, way_rel: WayRelation, detect_adjacencies, left_driving_system=False,
@@ -512,21 +542,23 @@
             speed_limit_dict = {}
         if speed_limit_lanelets is None:
             speed_limit_lanelets = {}
 
         left_way = self.osm.find_way_by_id(way_rel.left_way)
         right_way = self.osm.find_way_by_id(way_rel.right_way)
         if len(left_way.nodes) != len(right_way.nodes):
-            print(f"Trying to fix relation {way_rel.id_}...")
+            logging.info("Lanelet2CRConverter::_way_rel_to_lanelet: Trying to fix relation {}...".format(way_rel.id_))
+
             self._fix_relation_unequal_ways(left_way, right_way)
 
         # If for some reason, relation couldn't be fixed, notify user
         if len(left_way.nodes) != len(right_way.nodes):
-            print(f"Error: Relation {way_rel.id_} has left and right ways which are not equally long! "
-                  f"Please check your data! Discarding this lanelet relation.")
+            logging.error("Lanelet2CRConverter::_way_rel_to_lanelet: Error: Relation {} has left and right "
+                          "ways which are not equally long! Please check your data! Discarding this "
+                          "lanelet relation.".format(way_rel.id_))
             return None
 
         # set only if not set before
         # one way can only have two lanelet relations which use it
         if not self._left_way_ids.get(way_rel.left_way):
             self._left_way_ids[way_rel.left_way] = way_rel.id_
         if not self._right_way_ids.get(way_rel.right_way):
@@ -713,51 +745,55 @@
         # first case: left adjacent, same direction
         if lanelet.adj_left is None:
             potential_left_front = self._find_lanelet_ids_of_suitable_nodes(self.first_right_pts, first_left_node)
             potential_left_back = self._find_lanelet_ids_of_suitable_nodes(self.last_right_pts, last_left_node)
             potential_left_same_direction = list(set(potential_left_front) & set(potential_left_back))
             for lanelet_id in potential_left_same_direction:
                 nb_lanelet = self.lanelet_network.find_lanelet_by_id(lanelet_id)
-                if nb_lanelet is not None and _two_vertices_coincide(lanelet.left_vertices, nb_lanelet.right_vertices):
+                if nb_lanelet is not None and _two_vertices_coincide(lanelet.left_vertices, nb_lanelet.right_vertices,
+                                                                     self._config.adjacent_way_distance_tolerance):
                     self.lanelet_network.set_adjacent_left(lanelet, nb_lanelet.lanelet_id, True)
                     break
 
         # second case: right adjacent, same direction
         if lanelet.adj_right is None:
             potential_right_front = self._find_lanelet_ids_of_suitable_nodes(self.first_left_pts, first_right_node)
             potential_right_back = self._find_lanelet_ids_of_suitable_nodes(self.last_left_pts, last_right_node)
             potential_right_same_direction = list(set(potential_right_front) & set(potential_right_back))
             for lanelet_id in potential_right_same_direction:
                 nb_lanelet = self.lanelet_network.find_lanelet_by_id(lanelet_id)
-                if nb_lanelet is not None and _two_vertices_coincide(lanelet.right_vertices, nb_lanelet.left_vertices):
+                if nb_lanelet is not None and _two_vertices_coincide(lanelet.right_vertices, nb_lanelet.left_vertices,
+                                                                     self._config.adjacent_way_distance_tolerance):
                     self.lanelet_network.set_adjacent_right(lanelet, nb_lanelet.lanelet_id, True)
                     break
 
         # third case: left adjacent, opposite direction
         if lanelet.adj_left is None:
             potential_left_front = self._find_lanelet_ids_of_suitable_nodes(self.last_left_pts, first_left_node)
             potential_left_back = self._find_lanelet_ids_of_suitable_nodes(self.first_left_pts, last_left_node)
             potential_left_other_direction = list(set(potential_left_front) & set(potential_left_back))
             for lanelet_id in potential_left_other_direction:
                 nb_lanelet = self.lanelet_network.find_lanelet_by_id(lanelet_id)
                 # compare right vertex of nb_lanelet with left vertex of lanelet
                 if nb_lanelet is not None and _two_vertices_coincide(lanelet.left_vertices,
-                                                                     nb_lanelet.left_vertices[::-1]):
+                                                                     nb_lanelet.left_vertices[::-1],
+                                                                     self._config.adjacent_way_distance_tolerance):
                     self.lanelet_network.set_adjacent_left(lanelet, nb_lanelet.lanelet_id, False)
                     break
 
         # fourth case: right adjacent, opposite direction
         if lanelet.adj_right is None:
             potential_right_front = self._find_lanelet_ids_of_suitable_nodes(self.last_right_pts, first_right_node)
             potential_right_back = self._find_lanelet_ids_of_suitable_nodes(self.first_right_pts, last_right_node)
             potential_right_other_direction = list(set(potential_right_front) & set(potential_right_back))
             for lanelet_id in potential_right_other_direction:
                 nb_lanelet = self.lanelet_network.find_lanelet_by_id(lanelet_id)
                 if nb_lanelet is not None and _two_vertices_coincide(lanelet.right_vertices,
-                                                                     nb_lanelet.right_vertices[::-1]):
+                                                                     nb_lanelet.right_vertices[::-1],
+                                                                     self._config.adjacent_way_distance_tolerance):
                     self.lanelet_network.set_adjacent_right(lanelet, nb_lanelet.lanelet_id, True)
                     break
 
     def _check_right_and_left_neighbors(self, way_rel: WayRelation, lanelet: ConversionLanelet):
         """
         Check if lanelet has adjacent right and lefts.
         Determines it by checking if they share a common way.
@@ -792,15 +828,15 @@
 
         :param way: Way to be converted.
         :return: The vertices of the new lanelet border.
         """
         vertices = np.empty((len(way.nodes), 2))
         for i, node_id in enumerate(way.nodes):
             nd = self.osm.find_node_by_id(node_id)
-            x, y = self.proj(float(nd.lon), float(nd.lat))
+            x, y = self.transformer.transform(float(nd.lat), float(nd.lon))
             x -= self.origin_utm[0]
             y -= self.origin_utm[1]
             vertices[i] = [x, y]
 
         return vertices
 
     def node_distance(self, node_id1: str, node_id2: str) -> float:
@@ -809,16 +845,16 @@
 
         :param node_id1: Id of first node.
         :param node_id2: id of second node.
         :return: Distance of the nodes
         """
         node1 = self.osm.find_node_by_id(node_id1)
         node2 = self.osm.find_node_by_id(node_id2)
-        vec1 = np.array(self.proj(float(node1.lon), float(node1.lat)))
-        vec2 = np.array(self.proj(float(node2.lon), float(node2.lat)))
+        vec1 = np.array(self.transformer.transform(float(node1.lat), float(node1.lon)))
+        vec2 = np.array(self.transformer.transform(float(node2.lat), float(node2.lon)))
         return np.linalg.norm(vec1 - vec2)
 
     def _find_lanelet_ids_of_suitable_nodes(self, nodes_dict: Dict[str, List[str]], node_id: str) -> List:
         """
         Find values of a dict where the keys are node ids.
         Return the entries if there is a value in the node_dict
         for the node_id, but also the values for nodes which are in
@@ -827,15 +863,15 @@
         :param nodes_dict: Dict which saves lanelet ids with node ids as keys.
         :param node_id: Id of node for which the other entries are searched for.
         :return: List of lanelet ids which match the above-mentioned rules.
         """
         suitable_lanelet_ids = []
         suitable_lanelet_ids.extend(nodes_dict.get(node_id, []))
         for nd, lanelet_ids in nodes_dict.items():
-            if self.node_distance(nd, node_id) < config.NODE_DISTANCE_TOLERANCE:
+            if self.node_distance(nd, node_id) < self._config.node_distance_tolerance:
                 suitable_lanelet_ids.extend(lanelet_ids)
         return suitable_lanelet_ids
 
     def create_additional_nodes(self, shorter_way: Way, longer_way: Way):
         """
         Function that creates additional nodes and adds them to the shorter way in order
         to fix the relation of unequal ways
@@ -849,15 +885,15 @@
         start_node = self.osm.find_node_by_id(shorter_way.nodes[mid])
         end_node = self.osm.find_node_by_id(shorter_way.nodes[mid - 1])
         # Parse to nodes with numeric values
         start_node_f = np.array([float(start_node.lat), float(start_node.lon)])
         end_node_f = np.array([float(end_node.lat), float(end_node.lon)])
         # Add n nodes, start from last one
         for i in range(n, 0, -1):
-            k = config.DEFAULT_START_NODE_VALUE
+            k = self._config.start_node_id_value
             new_id = int(start_node.id_) + k * 100 + i
             while self.osm.find_node_by_id(str(new_id)) is not None:
                 k = k + 1
                 new_id = int(start_node.id_) + k * 100 + i
             # For Getting n additional nodes, we need to split the segment into n+1 smaller segments
             new_lat = round(start_node_f[0] + (end_node_f[0] - start_node_f[0]) * i / (n + 1), 11)
             new_lon = round(start_node_f[1] + (end_node_f[1] - start_node_f[1]) * i / (n + 1), 11)
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/map_conversion_interface.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/map_conversion_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import subprocess
 from pathlib import Path
-
+from typing import Optional
 from lxml import etree
 import uuid
 import os
 
 from commonroad.scenario.scenario import Scenario
 from commonroad.common.file_reader import CommonRoadFileReader
 
@@ -24,105 +24,106 @@
     from crdesigner.map_conversion.sumo_map.cr2sumo.converter import CR2SumoMapConverter
     from crdesigner.map_conversion.sumo_map.sumo2cr import convert_net_to_cr
 
 from crdesigner.map_conversion.osm2cr.converter_modules.cr_operations.export import (
     convert_to_scenario,
 )
 from crdesigner.map_conversion.osm2cr.converter_modules.converter import GraphScenario
-from crdesigner.configurations.get_configs import get_configs
+from crdesigner.config.config import Lanelet2ConversionParams, OpenDRIVEConversionParams, GeneralParams
 
 
 def lanelet_to_commonroad(
-    input_file: str, proj: str, left_driving: bool = False, adjacencies: bool = False
+        input_file: str,
+        general_config: GeneralParams = GeneralParams(),
+        lanelet2_config: Lanelet2ConversionParams = Lanelet2ConversionParams()
 ) -> Scenario:
     """
     Converts lanelet/lanelet2 file to CommonRoad
 
-    @param input_file: Path to lanelet/lanelet2 file
-    @param proj: proj-string
-    @param left_driving: Map describes left driving system.
-    @param adjacencies: Detect left and right adjacencies of lanelets if they do not share a common way
-    @return: CommonRoad scenario
+    :param input_file: Path to lanelet/lanelet2 file
+    :param general_config: General config parameters.
+    :param lanelet2_config: Lanelet2 config parameters.
+    :return: CommonRoad scenario
     """
     parser = Lanelet2Parser(etree.parse(input_file).getroot())
     lanelet2_content = parser.parse()
 
-    lanelet2_converter = Lanelet2CRConverter(proj_string=proj)
-    scenario = lanelet2_converter(
-        lanelet2_content,
-        detect_adjacencies=adjacencies,
-        left_driving_system=left_driving,
-    )
+    lanelet2_converter = Lanelet2CRConverter(lanelet2_config=lanelet2_config, cr_config=general_config)
+    scenario = lanelet2_converter(lanelet2_content)
 
     return scenario
 
 
-def commonroad_to_lanelet(input_file: str, output_name: str, proj: str):
+def commonroad_to_lanelet(input_file: str, output_name: str, 
+                          config: Lanelet2ConversionParams = Lanelet2ConversionParams()):
     """
     Converts CommonRoad map to lanelet format
 
-    @param input_file: Path to CommonRoad map
-    @param output_name: Name and path of lanelet file.
-    @param proj: proj-string
+    :param input_file: Path to CommonRoad map
+    :param output_name: Name and path of lanelet file.
+    :param config: Lanelet2 config parameters.
     """
     try:
         commonroad_reader = CommonRoadFileReader(input_file)
         scenario, _ = commonroad_reader.open()
 
     except etree.XMLSyntaxError as xml_error:
         print(f"SyntaxError: {xml_error}")
         print(
             "There was an error during the loading of the selected CommonRoad file.\n"
         )
         return
 
-    l2osm = CR2LaneletConverter(proj)
+    l2osm = CR2LaneletConverter(config)
     osm = l2osm(scenario)
     with open(f"{output_name}", "wb") as file_out:
         file_out.write(
             etree.tostring(
                 osm, xml_declaration=True, encoding="UTF-8", pretty_print=True
             )
         )
 
 
-def opendrive_to_commonroad(input_file: str) -> Scenario:
+def opendrive_to_commonroad(input_file: str,
+                            general_config: GeneralParams = GeneralParams(),
+                            odr_config: OpenDRIVEConversionParams = OpenDRIVEConversionParams()) -> Scenario:
     """
     Converts OpenDRIVE file to CommonRoad
 
-    @param input_file: Path to OpenDRIVE file
-    @return: CommonRoad scenario
+    :param input_file: Path to OpenDRIVE file
+    :param general_config: General config parameters.
+    :param odr_config: OpenDRIVE config parameters.
+    :return: CommonRoad scenario
     """
     opendrive = parse_opendrive(input_file)
-    # load configs
-    configs = get_configs()
-    road_network = Network(configs.opendrive)
+    road_network = Network(odr_config)
     road_network.load_opendrive(opendrive)
     for index in range(len(road_network._traffic_lights)):
-        road_network._traffic_lights[index]._traffic_light_id = abs(road_network._traffic_lights[index].traffic_light_id)
-    return road_network.export_commonroad_scenario()
+        road_network._traffic_lights[index]._traffic_light_id = \
+            abs(road_network._traffic_lights[index].traffic_light_id)
+    return road_network.export_commonroad_scenario(general_config, odr_config)
 
 
 def sumo_to_commonroad(input_file: str) -> Scenario:
     """
     Converts SUMO net file to CommonRoad
 
-    @param input_file: Path to SUMO net file
-    @return: CommonRoad scenario
+    :param input_file: Path to SUMO net file
+    :return: CommonRoad scenario
     """
     return convert_net_to_cr(input_file)
 
 
 def commonroad_to_sumo(input_file: str, output_file: str):
     """
     Converts CommonRoad file to SUMO net file and stores it
 
-    @param input_file: Path to CommonRoad file
-    @param output_file: Path where files should be stored
-    @return: CommonRoad scenario
+    :param input_file: Path to CommonRoad file
+    :param output_file: Path where files should be stored
+    :return: CommonRoad scenario
     """
     try:
         commonroad_reader = CommonRoadFileReader(input_file)
         scenario, _ = commonroad_reader.open()
     except etree.XMLSyntaxError as xml_error:
         print(f"SyntaxError: {xml_error}")
         print(
@@ -138,46 +139,46 @@
         converter.create_sumo_files(path)
 
 
 def osm_to_commonroad(input_file: str) -> Scenario:
     """
     Converts OpenStreetMap file to CommonRoad scenario
 
-    @param input_file: Path to OpenStreetMap file
-    @return: CommonRoad scenario
+    :param input_file: Path to OpenStreetMap file
+    :return: CommonRoad scenario
     """
     osm_graph = GraphScenario(input_file).graph
     return convert_to_scenario(osm_graph)
 
 
-def osm_to_commonroad_using_sumo(input_file: str) -> Scenario:
+def osm_to_commonroad_using_sumo(input_file: str) -> Optional[Scenario]:
     """
     Converts OpenStreetMap file to CommonRoad scenario using SUMO: SUMO offers the tool netconvert
     (https://sumo.dlr.de/docs/netconvert.html), which can be used to convert an OSM-file to OpenDrive (.xodr).
     This OpenDrive-file is then transformed to CommonRoad using the implementation here.
     Compared to the OSM-to-CommonRoad-conversion implemented here (see method :osm_to_commonroad), the
     road-interpolation is different. Furthermore, motorway services ("Raststätten") are currently not parsed
     when using :osm_to_commonroad.
 
-    @param input_file: Path to OpenStreetMap file
-    @return: CommonRoad scenario
+    :param input_file: Path to OpenStreetMap file
+    :return: CommonRoad scenario
     """
     input_file_pth = Path(input_file)
     scenario_name = str(input_file_pth.name)
     opendrive_file = str(input_file_pth.parent / f"{scenario_name}.xodr")
     # convert to OpenDRIVE file using netconvert
     try:
         subprocess.check_output(
-        [
-            "netconvert",
-            "--osm-files",
-            input_file,
-            "--opendrive-output",
-            opendrive_file,
-            "--junctions.scurve-stretch",
-            "1.0",
-        ]
+                [
+                    "netconvert",
+                    "--osm-files",
+                    input_file,
+                    "--opendrive-output",
+                    opendrive_file,
+                    "--junctions.scurve-stretch",
+                    "1.0",
+                ]
         )
     except Exception as e:
         print("__Warning__: {}.".format(e))
-        return
-    return opendrive_to_commonroad(opendrive_file)
+        return None
+    return opendrive_to_commonroad(opendrive_file)
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/converter.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from typing import Tuple, List
 from crdesigner.map_conversion.opendrive.opendrive_conversion.plane_elements.plane import ParametricLane, \
     ParametricLaneBorderGroup
 from crdesigner.map_conversion.opendrive.opendrive_conversion.plane_elements.plane_group import ParametricLaneGroup
 from crdesigner.map_conversion.opendrive.opendrive_conversion.plane_elements.border import Border
-from crdesigner.map_conversion.opendrive.opendrive_conversion.utils import encode_road_section_lane_width_id, encode_mark_lane_width_id
+from crdesigner.map_conversion.opendrive.opendrive_conversion.utils import encode_road_section_lane_width_id, \
+    encode_mark_lane_width_id
+from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadLanes import Lane
+from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadLanes import LaneSection, LaneWidth
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadPlanView import PlanView
-import numpy as np
 
 
 class OpenDriveConverter:
     """Class for static methods to convert lane_sections to parametric_lanes."""
 
     @staticmethod
     def create_reference_border(plan_view: PlanView, lane_offsets: List[float]) -> Border:
@@ -50,23 +52,21 @@
         else:
             reference_border.width_coefficient_offsets.append(0.0)
             reference_border.width_coefficients.append([0.0])
 
         return reference_border
 
     @staticmethod
-    def lane_section_to_parametric_lanes(lane_section, reference_border) -> List[ParametricLaneGroup]:
+    def lane_section_to_parametric_lanes(lane_section: LaneSection, reference_border: Border) \
+            -> List[ParametricLaneGroup]:
         """Convert a whole lane section into a list of ParametricLane objects.
 
         :param lane_section: LaneSection from which to create the list of ParametricLane Objects
-        :type lane_section: :class:`LaneSection`
         :param reference_border: The reference border of the lane section, created from create_reference_border()
-         :type reference_border: :class:`Border`
-         :return: The converted ParametricLane objects.
-         :rtype: List
+        :return: The converted ParametricLane objects.
         """
 
         plane_groups = []
 
         for side in ["right", "left"]:
 
             # lanes loaded by opendriveparser are aleady sorted by id
@@ -122,28 +122,24 @@
                 # for borders in lane.borders:
 
                 if plane_group.length > 0:
                     plane_groups.append(plane_group)
         return plane_groups
 
     @staticmethod
-    def create_parametric_lane(lane_borders: List[Border], width, lane, side, mark_idx) -> ParametricLane:
+    def create_parametric_lane(lane_borders: List[Border], width: LaneWidth, lane: Lane, side: str, mark_idx: int) \
+            -> ParametricLane:
         """Create a parametric lane for a certain width section.
 
         :param lane_borders: Array with already created lane borders.
         :param width: Width section with offset and coefficient information.
-        :type width: :class:`LaneWidth`
         :param lane: Lane in which new parametric lane is created.
-        :type lane: :class:`Lane`
         :param side: Which side of the lane section where the parametric lane is created.
-        :type side: str
-        :param speed: Speed limit for this individual lane
-        :type speed: float
+        :param mark_idx: Index of line marking belonging to lane.
         :return: A ParametricLane object with specified borders and a unique id.
-        :rtype: :class:`ParametricLane`
         """
         if len(lane.road_mark) > 0:
             marking = lane.road_mark[mark_idx]
         else:
             marking = None
 
         border_group = ParametricLaneBorderGroup(
@@ -167,26 +163,23 @@
             line_marking=marking,
             side=side,
             access=lane.access
         )
         return parametric_lane
 
     @staticmethod
-    def _create_outer_lane_border(lane_borders, lane, coeff_factor) -> Border:
+    def _create_outer_lane_border(lane_borders: List[Border], lane: Lane, coeff_factor: int) -> Border:
         """Create an outer lane border of a lane.
         InnerBorder is already saved in lane_borders, as it is
         the outer border of the inner neighbour of the lane.
 
         :param lane_borders: Previous calculated lane borders of more inner lanes.
-        :type lane_borders: list[:class:`Border`]
         :param lane: Lane for which outer border shall be created.
-        :type lane: :class:`Lane`
         :param coeff_factor: Factor of -1 or 1, depending on which side of the reference path the lane is.
             Right side is -1.
-        :type coeff_factor: float
         :return: The created outer lane border.
         """
 
         # Create outer lane border
         # Offset from reference border is already included in first inner border
         # (lane_border[0])
         # reference_border starts at beginning of road, prev: lane section
@@ -204,19 +197,18 @@
             border.width_coefficient_offsets.append(width.start_offset)
             border.width_coefficients.append(
                 [x * coeff_factor for x in width.polynomial_coefficients]
             )
         return border
 
     @staticmethod
-    def determine_neighbours(lane) -> Tuple[str, str, bool]:
+    def determine_neighbours(lane: Lane) -> Tuple[str, str, bool]:
         """Determines neighbors of a lane.
 
         :param lane: Lane to find neighbors to.
-        :type lane: :class:`Lane`
         :return: IDs of the inner and outer neighbor, and whether the inner neighbor has the same direction.
         """
         if abs(lane.id) > 1:
 
             if lane.id > 0:
                 inner_lane_id = lane.id - 1
                 outer_lane_id = lane.id + 1
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/network.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import copy
 import numpy as np
 import iso3166
 from collections import deque
-from typing import Union
+from typing import Union, List, Optional
+from pyproj import CRS, Transformer
 from commonroad.scenario.scenario import Scenario, GeoTransformation, Location, ScenarioID
 from commonroad.scenario.lanelet import LaneletNetwork, Lanelet, StopLine, LineMarking
-from crdesigner.map_conversion.opendrive.opendrive_conversion import utils
+from commonroad.scenario.lanelet import LaneletType
+from commonroad.scenario.traffic_sign import TrafficSign, TrafficSignElement, TrafficSignIDGermany, \
+    TrafficSignIDZamunda, TrafficSignIDUsa, TrafficSignIDChina, TrafficSignIDSpain, \
+    TrafficSignIDRussia
 
+from crdesigner.map_conversion.opendrive.opendrive_conversion import utils
 from crdesigner.map_conversion.opendrive.opendrive_conversion.plane_elements.crosswalks import get_crosswalks
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.opendrive import OpenDrive
 from crdesigner.map_conversion.opendrive.opendrive_conversion.utils import encode_road_section_lane_width_id
 from crdesigner.map_conversion.common.conversion_lanelet_network import ConversionLaneletNetwork
 from crdesigner.map_conversion.common.conversion_lanelet import ConversionLanelet
 from crdesigner.map_conversion.opendrive.opendrive_conversion.converter import OpenDriveConverter
 from crdesigner.map_conversion.opendrive.opendrive_conversion.plane_elements.traffic_signals import get_traffic_signals
 from crdesigner.map_conversion.opendrive.opendrive_conversion.plane_elements.geo_reference import get_geo_reference
-from crdesigner.configurations.configuration import OpenDrive2CRConfiguration
-from commonroad.scenario.traffic_sign import TrafficSign, TrafficSignElement, TrafficSignIDGermany, \
-    TrafficSignIDZamunda, TrafficSignIDUsa, TrafficSignIDChina, TrafficSignIDSpain, \
-    TrafficSignIDRussia
+from crdesigner.config.config import OpenDRIVEConversionParams, GeneralParams
 from crdesigner.map_conversion.common.utils import generate_unique_id
-from commonroad.scenario.lanelet import LaneletType
-from typing import List
+from crdesigner.map_conversion.opendrive.opendrive_parser.elements.road import Road
 
 
 def convert_to_base_lanelet_network(lanelet_network: ConversionLaneletNetwork) -> LaneletNetwork:
     """Converts a ConversionLaneletNetwork to a LaneletNetwork.
 
     :param lanelet_network: ConversionLaneletNetwork that should be converted to a LaneletNetwork.
     :return: The converted LaneletNetwork.
@@ -48,27 +49,26 @@
 
 
 class Network:
     """Represents a network of parametric lanes, with a LinkIndex
     which stores the neighbor relations between the parametric lanes.
     """
 
-    def __init__(self, config: OpenDrive2CRConfiguration):
+    def __init__(self, config: OpenDRIVEConversionParams = OpenDRIVEConversionParams()):
         """Initializes a network object."""
-        self.config = config
+        self._config = config
         self._planes = []
         self._link_index = None
         self._geo_ref = None
+        self._offset = None
         self._traffic_lights = []
         self._traffic_signs = []
         self._stop_lines = []
         self._crosswalks = []
         self._country_ID = None
-        self.error_tolerance = self.config.error_tolerance
-        self.min_delta_s = self.config.min_delta_s
 
     def assign_country_id(self, value: str):
         """Assign country ID according to the ISO 3166-1 3 letter standard
 
         :param value: Nae of location as a string.
         """
         value = value.upper()
@@ -88,29 +88,26 @@
         """
         # TODO: Extract location information from Geotranformation in opendrive
         # proj_string_transformed = Transformer.from_pipeline(opendrive.header.geo_reference)
 
         self._link_index = LinkIndex()
         self._link_index.create_from_opendrive(opendrive)
 
-        try:
-            self._geo_ref = opendrive.header.geo_reference
-        except TypeError:
-            self._geo_ref = None
+        self._geo_ref = opendrive.header.geo_reference
+        self._offset = opendrive.header.offset
 
         # Get country ID form signal data in openDrive and set it as attribute of the network object
         self.assign_country_id(Network.get_country_id_from_opendrive(opendrive.roads))
-
+        # transformed_start_coord = transformer.transform(float(road_geometry.get("x")), float(road_geometry.get("y")))
+        # start_coord = np.array([transformed_start_coord[0], transformed_start_coord[1]])
         # Convert all parts of a road to parametric lanes (planes)
         for road in opendrive.roads:
             road.planView.precalculate()
             # The reference border is the baseline for the whole road
-            reference_border = OpenDriveConverter.create_reference_border(
-                road.planView, road.lanes.laneOffsets
-            )
+            reference_border = OpenDriveConverter.create_reference_border(road.planView, road.lanes.laneOffsets)
             # Extracting signals, signs and stop lines from each road
 
             # signal_references = get_traffic_signal_references(road)
             # A lane section is the smallest part that can be converted at once
             for lane_section in road.lanes.lane_sections:
                 parametric_lane_groups = OpenDriveConverter.lane_section_to_parametric_lanes(
                     lane_section, reference_border
@@ -153,30 +150,32 @@
                         position_2 = np.array(
                                 [position[0] + road_object.validLength * np.cos(angle),
                                  position[1] + road_object.validLength * np.sin(angle)])
 
                     stop_line = StopLine(position_1, position_2, LineMarking.SOLID)
                     self._stop_lines.append(stop_line)
 
-    def export_lanelet_network(self, filter_types: list = None) -> LaneletNetwork:
+    def export_lanelet_network(self, transformer: Transformer, filter_types: Optional[List[str]] = None) \
+            -> LaneletNetwork:
         """Export network as lanelet network.
 
+        :param transformer: Coordinate projection transformer.
         :param filter_types: Types of ParametricLane objects to be filtered. Default value is None.
         :return: The converted LaneletNetwork object.
         """
 
         # Convert groups to lanelets
-        lanelet_network = ConversionLaneletNetwork(self.config)
+        lanelet_network = ConversionLaneletNetwork(self._config, transformer)
 
         for parametric_lane in self._planes:
             if filter_types is not None and parametric_lane.type not in filter_types:
                 # Remove lanelets from intersections dictionary that do not fit the filtered type criterion
                 self._link_index.clean_intersections(parametric_lane.id_)
                 continue
-            lanelet = parametric_lane.to_lanelet(self.error_tolerance, self.min_delta_s)
+            lanelet = parametric_lane.to_lanelet(self._config.error_tolerance, self._config.min_delta_s, transformer)
             lanelet.predecessor = self._link_index.get_predecessors(parametric_lane.id_)
             lanelet.successor = self._link_index.get_successors(parametric_lane.id_)
             lanelet_network.add_lanelet(lanelet)
 
             # Create a map of lanelet_description to traffic signs/lights so that they can be assigned as
             # reference to the correct lanelets later
 
@@ -332,17 +331,15 @@
                     break
 
     def find_lane_speed_changes(self, lanelets: List[int], lanelet_network: ConversionLaneletNetwork):
         """Iteratively finds changes in lane speed between a lanelet and its predecessors. If there is a change, a
         virtual speed sign is added to the lanelet.
 
         :param lanelets: The list of lanelets that is checked for changes in lane speeds.
-        :type lanelets: List[ConversionLanelet]
         :param lanelet_network: The lanelet network that the lanelets belong to.
-        :type lanelet_network: ConversionLaneletNetwork
         """
         visited = []
         for lane in lanelets:
             lane = lanelet_network.find_lanelet_by_id(lane)
             visited.append(lane.lanelet_id)
             if lane.speed is None:
                 break
@@ -354,26 +351,22 @@
                 if pred not in visited:
                     lanelets.extend(
                             [p for p in lanelet_network.find_lanelet_by_id(pred).predecessor if p not in lanelets]
                     )
 
     def get_traffic_sign_with_equal_speed(
             self, lanelet: ConversionLanelet, lanelet_network: ConversionLaneletNetwork, speed: float
-    ) -> Union[TrafficSign, None]:
+    ) -> Optional[TrafficSign]:
         """Checks if the supplied lanelet has a traffic sign with a speed limit equal to the value given by the
         argument speed. If a sign was found, it is returned.
 
         :param lanelet: The lanelet to check for a sign with equal speed.
-        :type lanelet: ConversionLanelet
         :param lanelet_network: The lanelet network the lanelet belongs to.
-        :type lanelet_network: ConversionLanelet
         :param speed: The speed to compare the sign's speed to.
-        :type speed: float
         :return: The traffic sign with equal speed, if one is found. Returns None else.
-        :rtype: Union[TrafficSign, None]
         """
         for id in lanelet.traffic_signs:
             sign = lanelet_network.find_traffic_sign_by_id(id)
             for elem in sign.traffic_sign_elements:
                 if elem.traffic_sign_element_id in [TrafficSignIDZamunda.MAX_SPEED, TrafficSignIDGermany.MAX_SPEED,
                                                     TrafficSignIDUsa.MAX_SPEED, TrafficSignIDChina.MAX_SPEED,
                                                     TrafficSignIDSpain.MAX_SPEED, TrafficSignIDRussia.MAX_SPEED] \
@@ -381,87 +374,73 @@
                     return sign
         return None
 
     def add_virtual_traffic_sign(self, lanelet: ConversionLanelet, network: ConversionLaneletNetwork):
         """Adds a virtual traffic sign to a lanelet.
 
         :param lanelet: Lanelet to add virtual traffic signal to.
-        :type lanelet: ConversionLanelet
         :param network: The lanelet network to which the lanelet belongs to.
-        :type network: ConversionLaneletNetwork
         """
         traffic_sign_enum = utils.get_traffic_sign_enum_from_country(
-                utils.get_signal_country(network.config.default_country_id)
+                utils.get_signal_country(self._country_ID)
         )
         element_id = traffic_sign_enum.MAX_SPEED
         additional_values = [str(float(lanelet.speed))]
         traffic_sign_element = TrafficSignElement(traffic_sign_element_id=element_id,
                                                   additional_values=additional_values)
         traffic_sign = TrafficSign(traffic_sign_id=generate_unique_id(),
                                    traffic_sign_elements=list([traffic_sign_element]),
                                    first_occurrence={lanelet.lanelet_id}, position=lanelet.center_vertices[0],
                                    virtual=True)
         network.add_traffic_signs_to_network([traffic_sign])
         lanelet.add_traffic_sign_to_lanelet(traffic_sign.traffic_sign_id)
 
-    def export_commonroad_scenario(
-            self, dt: float = 0.1, map_name="OpenDrive", map_id=1, filter_types=None
-    ):
+    def export_commonroad_scenario(self, general_config: GeneralParams = GeneralParams(),
+                                   opendrive_config: OpenDRIVEConversionParams = OpenDRIVEConversionParams()):
         """Export a full CommonRoad scenario
 
-        :param dt: Delta time step, default is 0.1
-        :type dt: float
-        :param map_name: Name of the map in the scenario ID, default value is "OpenDrive".
-        :type map_name: str
-        :param map_id: Running index of the map in the scenario ID, default value is 1.
-        :type map_id: int
-        :param filter_types: Types of ParametricLanes to be filtered. Default is None.
-        :type filter_types: list
+        :param general_config: General config parameters.
+        :param opendrive_config: OpenDRIVE specific config parameters.
         """
+        transformer = None
+        location_kwargs = {}
         if self._geo_ref is not None:
             longitude, latitude = get_geo_reference(self._geo_ref)
-            geo_transformation = GeoTransformation(geo_reference=self._geo_ref)
-
             if longitude is not None and latitude is not None:
-                location = Location(
-                    geo_transformation=geo_transformation,
-                    gps_latitude=latitude, gps_longitude=longitude
-                )
+                location_kwargs = dict(gps_latitude=latitude, gps_longitude=longitude)
 
-            else:
-                location = Location(geo_transformation=geo_transformation)
-        else:
-            location = Location()
-
-        scenario_id = ScenarioID(country_id=self._country_ID, map_name=map_name, map_id=map_id)
+            crs_from = CRS(self._geo_ref)
+            crs_to = CRS(self._config.proj_string)
+            transformer = Transformer.from_proj(crs_from, crs_to)
+
+        location = Location(geo_transformation=GeoTransformation(geo_reference=self._config.proj_string),
+                            **location_kwargs)
+
+        scenario_id = ScenarioID(
+                country_id=general_config.country_id if self._country_ID == "ZAM" else self._country_ID,
+                map_name=general_config.map_name,
+                map_id=general_config.map_id)
 
         scenario = Scenario(
-            dt=dt, scenario_id=scenario_id,
+            dt=general_config.time_step_size, scenario_id=scenario_id,
             location=location
         )
 
-        scenario.add_objects(
-            self.export_lanelet_network(
-                filter_types=filter_types
-                if isinstance(filter_types, list)
-                else ["driving", "restricted", "onRamp", "offRamp", "exit", "entry", "sidewalk", "shoulder",
-                      "crosswalk", "bidirectional"]
-            )
-        )
+        scenario.add_objects(self.export_lanelet_network(transformer=transformer,
+                                                         filter_types=opendrive_config.filter_types))
 
         return scenario
 
     @staticmethod
-    def get_country_id_from_opendrive(roads):
+    def get_country_id_from_opendrive(roads: List[Road]) -> str:
         """
         Get country id of a specific lanelet network
+
         :param roads: Roads from which country id should be returned.
-        :type roads: list[:class:`Road`]
         :return: The country id.
-        :rtype: str
         """
         for road in roads:
             for signal in road.signals:
                 return signal.country
         return "ZAM"
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/border.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/border.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,51 @@
 import math
-import warnings
 from functools import lru_cache
-from typing import Optional, Any, Tuple
+from typing import Optional, Any, Tuple, List
 import numpy as np
 
 
 class Border:
     """ A lane border defines a path along a whole lane section. A lane always uses an inner and outer lane border.
     The reference can be another lane border or a plan view."""
 
     def __init__(self, ref_offset: float = 0.0):
         """Initializes a Border object.
         :param ref_offset: Offset in s-direction to the reference object after which the border begins.
-        :type ref_offset: float, default: 0.0
         """
         self.ref_offset = float(ref_offset)
         self.width_coefficient_offsets = []
         self.width_coefficients = []
 
         self.reference = None
 
     def _get_width_index(self, s_pos: float, is_last_pos: bool) -> float:
         """Get the index of the width which applies at position s_pos.
 
         :param s_pos: Position on border in curve_parameter ds
-        :type s_pos: float
         :param is_last_pos: Whether s_pos is the last position
-        :type s_pos: bool
         :return: Index of width that applies at position s_pos
-        :rtype: float
         """
         return next((
                 self.width_coefficient_offsets.index(n)
                 for n in self.width_coefficient_offsets[::-1]
                 if (
                     (n <= s_pos and (not is_last_pos or s_pos == 0))
                     or (n < s_pos and is_last_pos)
                 )
             ),
             len(self.width_coefficient_offsets)-1,
         )
 
-    def get_next_width_coeffs(self, s_pos: float, is_last_pos: bool = False) -> list:
+    def get_next_width_coeffs(self, s_pos: float, is_last_pos: bool = False) -> List[float]:
         """Get width coefficients which apply at position s_pos.
 
         :param s_pos: Position on border in curve_parameter ds
-        :type s_pos: float
         :param is_last_pos: Whether s_pos is the last position
-        :type is_last_pos: bool, default is False
         :return: An array with coefficients [a, b, c, d] for the polynomial w = a + b*ds + c*ds² + d*ds³
-        :rtype: list
         """
         width_idx = self._get_width_index(s_pos, is_last_pos)
         return self.width_coefficients[width_idx]
 
     # NOTE: might by more efficient to calculate each border once
     # instead of recalculating them over and over.
     @lru_cache(maxsize=200000)
@@ -61,28 +53,20 @@
              compute_curvature=True) -> Tuple[Optional[Any], Any, Any, Any]:
         """Calculate the Cartesian coordinates and the tangential direction of
         the border by calculating position of reference border at s_pos
         and then adding the width in orthogonal direction to the reference position.
 
         :param s_pos: Position s_pos specified in curve parameter ds where to calculate the cartesian coordinates on
                         the border
-        :type s_pos: float
         :param width_offset: Offset to add to calculated width at position s_pos
-        :type width_offset: float
         :param is_last_pos: Whether s_pos is the last position
-        :type is_last_pos: bool
         :param reverse: Whether to calculate positions in a reverse order, default is False
-        :type reverse: bool
         :param compute_curvature: Whether to computer curvature, default is True
-        :type compute_curvature: bool
-        :return: coord: (x,y) tuple of cartesian coordinates and the direction angle in radians.
-        tang: Tangential at s_pos, a float.
-        curv: Curvature at s_pos, a float, optional.
-        max_geometry_length: Maximum length of the geometry, a float.
-        :rtype: tuple[Optional[Any], Any, Any, Any]
+        :return: coord: (x,y) tuple of cartesian coordinates, tangential at s_pos, curvature at s_pos,
+        and maximum length of the geometry
         """
         # Last reference has to be a reference geometry (PlanView)
         # Offset of all inner lanes (Border)
         # calculate position of reference border
         if np.isclose(s_pos, 0):
             s_pos = 0
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/crosswalks.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/crosswalks.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/geo_reference.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/geo_reference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import re
+from typing import Tuple, Optional
 
 
-def get_geo_reference(geo_reference: str) -> float:
-    """Gets the geographic location information from the geo string extracted from opendrive files.
+def get_geo_reference(geo_reference: str) -> Tuple[Optional[float], Optional[float]]:
+    """Gets the geographic location information from the geo string extracted from OpenDRIVE files.
 
     :param geo_reference: Input string from which longitude and latitude should be extracted.
-    :type geo_reference: String
     :return: longitude and latitude parsed from input string
-    :rtype: float
     """
     elements = []
     elements.extend(re.split(r'\+', geo_reference))
 
     longitude = None
     latitude = None
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,148 +1,121 @@
-"""Module for parametric lanes, which is an intermediate step between OpenDRIVE lanes
-and lanelets."""
-from typing import Tuple
+from typing import Tuple, Optional, List
 import numpy as np
+from numpy.polynomial import polynomial
+from pyproj import Transformer
+from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadLanes import RoadMark
 from crdesigner.map_conversion.opendrive.opendrive_conversion.plane_elements.border import Border
-from crdesigner.map_conversion.opendrive.opendrive_parser.elements.geometry import calc_next_s
-from numpy.polynomial import polynomial as P
 
 
 class ParametricLaneBorderGroup:
     """Group Borders and BorderOffsets of ParametricLanes into one class."""
 
     # NOTE: not checking types with getter/setter because duck typing
     # should be possible
     def __init__(
         self,
-        inner_border=None,
-        inner_border_offset=None,
-        outer_border=None,
-        outer_border_offset=None,
+        inner_border: Optional[Border] = None,
+        inner_border_offset: Optional[float] = None,
+        outer_border: Optional[Border] = None,
+        outer_border_offset: Optional[float] = None,
     ):
         """Initializes a ParametricLaneBorderGroup object.
 
         :param inner_border: Inner Border of a ParametricLane
-        :type inner_border: :class:`opendrive.opendrive_conversion.plane_elements.border.Border`
         :param outer_border: Outer Border of a ParametricLane
-        :type outer_border: :class:`opendrive.opendrive_conversion.plane_elements.border.Border`
         :param inner_border_offset: Offset of start of parametric lane to start of border.
                                     This is necessary as a Border can be used by multiple ParametricLanes
-        :type inner_border_offset: float
         :param outer_border_offset: Same concept as inner_border_offset, but for outer border.
-        :type outer_border_offset: float
         """
         self.inner_border: Border = inner_border
         self.inner_border_offset = inner_border_offset
         self.outer_border: Border = outer_border
         self.outer_border_offset = outer_border_offset
 
     def calc_border_position(
         self, border: str, s_pos: float, width_offset: float, is_last_pos: bool = False, reverse=False,
-            compute_curvature=True
-    ) -> Tuple[Tuple[float, float], float]:
+            compute_curvature: bool = True) -> Tuple[Tuple[float, float], float]:
         """Calc vertices point of inner or outer Border.
 
         :param border: Which border to calculate (inner or outer)
-        :type border: str
         :param s_pos: Position of parameter ds where to calc the cartesian coordinates
-        :type s_pos: float
         :param width_offset: Offset to add to calculated width in reference to the reference border
-        :type width_offset: float
         :param is_last_pos: Whether it's the last position, default is False
-        :type is_last_pos: bool
         :param reverse: Whether to calculate in reverse order
-        :type reverse: bool
         :param compute_curvature: Whether to computer curvature, default is True
-        :type compute_curvature: bool
         :return: Cartesian coordinates of point on inner border and tangential direction.
-        :rtype: Tuple[Tuple[float, float], float]
         """
         if border not in ("inner", "outer"):
             raise ValueError("Border specified must be 'inner' or 'outer'!")
 
         select_border = self.inner_border if border == "inner" else self.outer_border
         select_offset = (
             self.inner_border_offset if border == "inner" else self.outer_border_offset
         )
 
         return select_border.calc(
             select_offset + s_pos, width_offset=width_offset, is_last_pos=is_last_pos, reverse=reverse,
             compute_curvature=compute_curvature
         )
 
-    def get_width_coefficients(self) -> list:
+    def get_width_coefficients(self) -> List:
         """Get the width coefficients which apply to this ParametricLane.
 
         :return: The width coefficients in format [a, b, c, distance_from_other_border]
-        :rtype: list
         """
         # TODO: expand implementation to consider border offset record
         return self.outer_border.get_next_width_coeffs(self.outer_border_offset)
 
 
 class ParametricLane:
     """A lane defines a part of a road along a
     reference trajectory (plan view), using lane borders
     and start/stop positions (parametric)"""
     def __init__(
         self,
         id_: str,
         type_: str,
         border_group: ParametricLaneBorderGroup,
-        length: float = None,
-        line_marking = None,
-        side: str = None,
-        speed: float = None,
-        access: list = []
+        length: Optional[float] = None,
+        line_marking: Optional[RoadMark] = None,
+        side: Optional[str] = None,
+        speed: Optional[float] = None,
+        access: Optional[List] = None
     ):
         """Initializes a ParametricLane object.
 
         :param border_group: Reference to object which manages borders.
-        :type border_group: :class:`ParametricLaneBorderGroup`
         :param id_: Unique string identifier.
-        :type id_: str
         :param type_: Identifies type of ParametricLane
-        :type type_: str
         :param length: Length of ParametricLane, default is None
-        :type length: float
         :param line_marking: Line marking object. Default is None
-        :type line_marking: :class:`RoadMark`
         :param side: the side in lane section. Used for determining the line marking side. Default is None
-        :type side: str
         :param speed: Speed limit for this individual plane
-        :type speed: float
         :param access: equivalent to access restrictions from opendrive lanes
-        :type access: list
         """
         self.border_group = border_group
         self.id_ = id_
         self.type_ = type_
         self.length = length
         self.reverse = False
         self.line_marking = line_marking
         self.side = side
         self.speed = speed
-        self.access = access
+        self.access = access if access is not None else []
 
     def calc_border(
-        self, border: str, s_pos: float, width_offset: float = 0.0, compute_curvature=True
+        self, border: str, s_pos: float, width_offset: float = 0.0, compute_curvature: bool = True
     ) -> Tuple[Tuple[float, float], float, float, float]:
         """Calc vertices point of inner or outer Border.
 
         :param border: Which border to calculate (inner or outer).
-        :type border: str
         :param s_pos: Position of parameter ds where to calc the cartesian coordinates
-        :type: float
         :param width_offset: Offset to add to calculated width in reference to the reference border. Default is 0.0.
-        :type width_offset: float
         :param compute_curvature: Whether to computer curvature. Default is True.
-        :type: bool
         :return: Cartesian coordinates of point on inner border and tangential direction.
-        :rtype: Tuple[Tuple[float, float], float, float, float]
         """
         if self.reverse:
             border_pos = self.length - s_pos
         else:
             border_pos = s_pos
 
         is_last_pos = np.isclose(self.length, border_pos)
@@ -150,28 +123,25 @@
             border, border_pos, width_offset, is_last_pos, self.reverse, compute_curvature=compute_curvature)
         return r1, r2, r3, la
 
     def calc_width(self, s_pos: float) -> float:
         """Calc width of border at position s_pos.
 
         :param s_pos: Position of ParametricLane (in curve parameter ds) where width should be calculated.
-        :type: float
         :return: The width at position s_pos
-        :rtype: float
         """
-        innerCoords = self.calc_border("inner", s_pos)
-        outerCoords = self.calc_border("outer", s_pos)
+        inner_coords = self.calc_border("inner", s_pos)
+        outer_coords = self.calc_border("outer", s_pos)
 
-        return np.linalg.norm(innerCoords[0] - outerCoords[0])
+        return np.linalg.norm(inner_coords[0] - outer_coords[0])
 
     def has_zero_width_everywhere(self) -> bool:
         """Checks if width is zero at every point of this ParametricLaneGroup.
 
         :return: True if every ParametricLane has width_coefficients equal to only zero.
-        :rtype: bool
         """
         # TODO: expand this method to include border offset records
         return self.border_group.get_width_coefficients() == [0, 0, 0, 0]
 
     # def to_lanelet_with_mirroring(
     #     self,
     #     mirror_border: str,
@@ -270,29 +240,28 @@
 
     #     return (
     #         np.array(left_vertices),
     #         np.array(right_vertices),
     #         last_width_difference,
     #     )
 
-    def calc_vertices(self, error_tolerance, min_delta_s) -> Tuple[np.ndarray, np.ndarray]:
+    def calc_vertices(self, error_tolerance: float, min_delta_s: float,
+                      transformer: Optional[Transformer] = None) -> Tuple[np.ndarray, np.ndarray]:
         """Convert a ParametricLane to Lanelet.
 
         :param error_tolerance: Max. error between reference geometry and polyline of vertices.
-        :type error_tolerance: float
         :param min_delta_s: Min. step length between two sampling positions on the reference geometry
-        :type min_delta_s: float
+        :param transformer: Coordinate transformer/projection.
         :return: left and right vertices of the created Lanelet
-        :rtype: Tuple[np.ndarray, np.ndarray]
         """
         left_vertices = []
         right_vertices = []
         # calculate left and right vertices of lanelet
-        s = 0
-        check_3 = True
+        # s = 0
+        # check_3 = True
 
         # old version from opendrive2lanelet start
         # no sampling of s and "distance" between two consecutive s is similar
         #
         if self.length < 0:
             return np.array(left_vertices), np.array(right_vertices)
         num_steps = int(max(3, np.ceil(self.length / float(0.5))))
@@ -302,16 +271,20 @@
         # old version end
 
         # version with sampling
         # while s <= self.length:
             # s_cache = s + 0.0
             inner_pos, _, curvature, max_geometry_length = self.calc_border("inner", s)
             outer_pos = self.calc_border("outer", s, compute_curvature=False)[0]
-            left_vertices.append(inner_pos)
-            right_vertices.append(outer_pos)
+            if transformer is not None:
+                left_vertices.append(transformer.transform(inner_pos[0], inner_pos[1]))
+                right_vertices.append(transformer.transform(outer_pos[0], outer_pos[1]))
+            else:
+                left_vertices.append(inner_pos)
+                right_vertices.append(outer_pos)
 
             # version with sampling
             # if s >= self.length:
             #     break
             #
             # if s == max_geometry_length:
             #     s += min_delta_s
@@ -329,60 +302,57 @@
         # assert len(left_vertices) >= 3, f"Not enough vertices, len: {len(left_vertices)}"
         return np.array(left_vertices), np.array(right_vertices)
 
     def zero_width_change_positions(self) -> float:
         """Position where the inner and outer Border have zero minimal distance change.
 
         :return: Positions (in curve parameter ds) where width change is zero.
-        :rtype: float
         """
 
         width_coefficients = self.border_group.get_width_coefficients()
         if width_coefficients[0] > 0.0 and all(
             coeff == 0.0 for coeff in width_coefficients[1:]
         ):
             # this is not correct as it should be an interval
             return [0, self.length]
         # but useful because only start and end of ParametricLane should be considered
 
         # get roots of derivative
-        roots = P.polyroots(P.polyder(width_coefficients))
+        roots = polynomial.polyroots(polynomial.polyder(width_coefficients))
         real_roots = roots[(np.isreal(roots)) & (roots >= 0) & (roots <= self.length)]
         if self.reverse:
             real_roots[:] = [self.length - x for x in real_roots]
         return real_roots
 
     def maximum_width(self, reverse: bool = False) -> Tuple[float, float]:
         """Get position and value of maximum width.
         Position is the distance of the maximum to the start or end
         of ParametricLane (end if reverse==True).
 
         :param reverse: If True and there are two equal maxima, take maxima closer to the end of the ParametricLane.
                         Default is False.
-        :type reverse: bool
         :return: (pos, max) tuple of position and value of maximum
-        :rtype: Tuple[float, float]
         """
         width_coefficients = self.border_group.get_width_coefficients()
-        width_derivative = P.polyder(width_coefficients)
+        width_derivative = polynomial.polyder(width_coefficients)
         # width_second_derivative = P.polyder(width_derivative)
-        roots = P.polyroots(width_derivative)
+        roots = polynomial.polyroots(width_derivative)
         # is_local_maximum = P.polyval(roots, width_second_derivative) < 0
         restricted_roots = roots[
             (np.isreal(roots))
             & (roots >= 0)
             # & (is_local_maximum)
             & (roots <= self.length)
         ]
 
         # append start and end of ParametricLane because maximum could be there, too
         restricted_roots = np.append(restricted_roots, [0, self.length])
 
         # calculate maximum values
-        max_values = P.polyval(restricted_roots, width_coefficients)
+        max_values = polynomial.polyval(restricted_roots, width_coefficients)
 
         # width of one ParametricLane is either always positive or negative
         max_values = abs(max_values)
         pos_and_val = np.column_stack((restricted_roots, max_values))
         if self.reverse:
             pos_and_val = np.array([[self.length - x[0], x[1]] for x in pos_and_val])
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane_group.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/plane_group.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import warnings
 from typing import Tuple, Optional, List
 import math
 import numpy as np
 import copy
+from pyproj import Transformer
 
 from crdesigner.map_conversion.common.conversion_lanelet import ConversionLanelet
 from crdesigner.map_conversion.opendrive.opendrive_conversion.plane_elements.plane import ParametricLane
 from commonroad.scenario.lanelet import LineMarking
 
 
 class ParametricLaneGroup:
     """A group of parametric_lanes can be converted to a
     lanelet just like a single parametric_lane.
     """
 
     def __init__(
         self,
-        id_=None,
+        id_: str = None,
         parametric_lanes=None,
         inner_neighbour=None,
         inner_neighbour_same_direction=True,
         outer_neighbour=None,
     ):
         """Initializes a ParametricLaneGroup object.
 
@@ -46,20 +47,19 @@
 
         if parametric_lanes is not None:
             if isinstance(parametric_lanes, list):
                 self.extend(parametric_lanes)
             else:
                 self.append(parametric_lanes)
 
-    def append(self, parametric_lane):
-        """Append lane to start or end of interal list of ParametricLane objects. If the parametric_lane is reverse,
+    def append(self, parametric_lane: ParametricLane):
+        """Append lane to start or end of internal list of ParametricLane objects. If the parametric_lane is reverse,
         it is inserted at the start.
 
         :param parametric_lane: Lane to be inserted either at beginning or end of list.
-        :type parametric_lane: :class:`ParametricLane`
         """
         if parametric_lane.reverse:
             self.parametric_lanes.insert(0, parametric_lane)
         else:
             self.parametric_lanes.append(parametric_lane)
 
         self._add_geo_length(parametric_lane.length, parametric_lane.reverse)
@@ -77,17 +77,15 @@
     def _add_geo_length(self, length: float, reverse: bool = False):
         """Add length of a ParametricLane to the array which keeps track
         at which position which ParametricLane is placed.
         This array is used for quickly accessing
         the proper ParametricLane for calculating a position.
 
         :param length: Length of ParametricLane to be added.
-        :type length: float
         :param reverse: Whether the lane is reversed. Default is False.
-        :type reverse: bool
         """
         if reverse:
             self._geo_lengths = np.insert(self._geo_lengths, 1, length)
             self._geo_lengths[2:] = [
                 x + length for i, x in enumerate(self._geo_lengths) if i > 1
             ]
         else:
@@ -96,24 +94,22 @@
             )
 
     @property
     def type(self) -> str:
         """Get type of ParametricLaneGroup.
 
         :return: Type of first ParametricLane in this group.
-        :rtype: str
         """
         return self.parametric_lanes[0].type_
 
     @property
     def length(self) -> float:
         """Length of all ParametricLanes which are collected in this ParametricLaneGroup.
 
         :return: Accumulated length of ParametricLaneGroup
-        :rtype: float
         """
 
         return sum([x.length for x in self.parametric_lanes])
 
     @property
     def access(self):
         """Access restrictions of the first ParametricLane in this ParametricLaneGroup.
@@ -123,37 +119,34 @@
         """
         return self.parametric_lanes[0].access
 
     def has_zero_width_everywhere(self) -> bool:
         """Checks if width is zero at every point of this ParametricLaneGroup.
 
         :return: True if every ParametricLane has width_coefficients equal to only zero
-        :rtype: bool
         """
         return all(
             [plane.has_zero_width_everywhere() for plane in self.parametric_lanes]
         )
 
-    def to_lanelet(self, error_tolerance, min_delta_s) -> ConversionLanelet:
+    def to_lanelet(self, error_tolerance, min_delta_s, transformer: Transformer) -> ConversionLanelet:
         """Convert a ParametricLaneGroup to a Lanelet.
 
         :param error_tolerance: Max. error between reference geometry and polyline of vertices.
-        :type error_tolerance: float
         :param min_delta_s: Min. step length between two sampling positions on the reference geometry
-        :type min_delta_s: float
+        :param transformer: Coordinate projection transformer.
         :return: Created Lanelet.
-        :rtype: 'class'`ConversionLanelet`
         """
         left_vertices, right_vertices = np.array([]), np.array([])
         line_marking_left_vertices = LineMarking.UNKNOWN
         line_marking_right_vertices = LineMarking.UNKNOWN
 
         for parametric_lane in self.parametric_lanes:
             local_left_vertices, local_right_vertices = parametric_lane.calc_vertices(
-                error_tolerance=error_tolerance, min_delta_s=min_delta_s
+                error_tolerance=error_tolerance, min_delta_s=min_delta_s, transformer=transformer
             )
             # check whether parametric lane cannot be used,
             # e.g., if to small it is possible that no vertices are generated
             if local_left_vertices is None or len(local_left_vertices) == 0:
                 continue
 
             if len(left_vertices) > 0:  # check for first iteration
@@ -268,27 +261,23 @@
                                         user_one_way=users)
 
         # Adjacent lanes
         self._set_adjacent_lanes(lanelet)
 
         return lanelet
 
-    def calc_border(self, border: str, s_pos: float, width_offset: float = 0.0, compute_curvature=True):
+    def calc_border(self, border: str, s_pos: float, width_offset: float = 0.0, compute_curvature: bool = True) \
+            -> Tuple[Tuple[float, float], float, float, float]:
         """Calc vertices point of inner or outer Border.
 
         :param border: Which border to calculate (inner or outer)
-        :type border: str
         :param s_pos: Position of parameter ds where to calc the cartesian coordinates
-        :type s_pos: float
         :param width_offset: Offset to add to calculated width in reference to the reference border. Default is 0.0.
-        :type width_offset: float
         :param compute_curvature: Whether to computer curvature. Default is True.
-        :type compute_curvature: bool
         :return: Cartesian coordinates of point on inner border and tangential direction.
-        :rtype: Tuple[Tuple[float, float], float, float, float]
         """
         try:
             # get index of geometry which is at s_pos
             mask = self._geo_lengths > s_pos
             sub_idx = np.argmin(self._geo_lengths[mask] - s_pos)
             plane_idx = np.arange(self._geo_lengths.shape[0])[mask][sub_idx] - 1
         except ValueError:
@@ -308,31 +297,27 @@
     def to_lanelet_with_mirroring(
         self,
         mirror_border: str,
         distance: Tuple[float, float],
         mirror_interval: Tuple[float, float],
         adjacent_lanelet: ConversionLanelet,
         precision: float = 0.5,
+        transformer: Optional[Transformer] = None
     ):
         """Convert a ParametricLaneGroup to a Lanelet with mirroring one of the borders.
 
         :param mirror_border: Which lane to mirror, if performing merging or splitting of lanes.
-        :type mirror_border: str
         :param distance: Distance at start and end of lanelet, which mirroring lane should have from the other lane it
                         mirrors
-        :type distance: Tuple[float, float]
         :param mirror_interval: Position at start and end of mirroring
-        :type mirror_interval: Tuple[float, float]
         :param adjacent_lanelet: The adjacent lanelet.
-        :type adjacent_lanelet: :class:`opendrive.opendrive_conversion.conversion_lanelet.ConversionLanelet`
         :param precision: Number which indicates at which space interval (in curve parameter ds) the coordinates of the
                         boundaries should be calculated. Default is 0.5.
-        :type precision: float
+        :param transformer: Coordinate projection transformer.
         :return: Created Lanelet.
-        :rtype: :class:`opendrive.opendrive_conversion.conversion_lanelet.ConversionLanelet`
         """
         linear_distance_poly = np.polyfit(mirror_interval, distance, 1)
         distance_poly1d = np.poly1d(linear_distance_poly)
         global_distance = distance_poly1d([0, self.length])
 
         if self.parametric_lanes[0].reverse:
             global_distance[:] = [-x for x in global_distance]
@@ -346,16 +331,20 @@
             outer_pos = self.calc_border("outer", pos)[0]
             original_width = np.linalg.norm(inner_pos - outer_pos)
 
             # if not mirroring lane or outside of range
             if (
                 pos < mirror_interval[0] or pos > mirror_interval[1]
             ) and not np.isclose(pos, mirror_interval[1]):
-                left_vertices.append(inner_pos)
-                right_vertices.append(outer_pos)
+                if transformer is not None:
+                    left_vertices.append(transformer.transform(inner_pos[0], inner_pos[1]))
+                    right_vertices.append(transformer.transform(outer_pos[0], outer_pos[1]))
+                else:
+                    left_vertices.append(inner_pos)
+                    right_vertices.append(outer_pos)
                 last_width_difference = 0
 
             else:
                 # calculate positions of adjacent lanelet because new width of lanelet
                 # cannot be more than width of adjacent lanelet and original width
                 adj_inner_pos = adjacent_lanelet.calc_border("inner", pos)[0]
                 adj_outer_pos = adjacent_lanelet.calc_border("outer", pos)[0]
@@ -370,44 +359,66 @@
 
                     # change width s.t. it does not mirror inner border but instead
                     # outer border
                     local_width_offset = (
                         math.copysign(1, local_width_offset) * last_width_difference
                     )
                     if modified_width < original_width:
-                        right_vertices.append(
-                            self.calc_border("outer", pos, local_width_offset)[0]
-                        )
+                        new_vertex = self.calc_border("outer", pos, local_width_offset)[0]
+                        if transformer is not None:
+                            right_vertices.append(transformer.transform(new_vertex[0], new_vertex[1]))
+                        else:
+                            right_vertices.append(new_vertex)
                     elif modified_width > original_width + adjacent_width:
-                        right_vertices.append(adj_outer_pos)
+                        if transformer is not None:
+                            right_vertices.append(transformer.transform(adj_outer_pos[0], adj_outer_pos[1]))
+                        else:
+                            right_vertices.append(adj_outer_pos)
                     else:
-                        right_vertices.append(new_outer_pos)
+                        if transformer is not None:
+                            right_vertices.append(transformer.transform(new_outer_pos[0], new_outer_pos[1]))
+                        else:
+                            right_vertices.append(new_outer_pos)
                         last_width_difference = abs(modified_width - original_width)
 
-                    left_vertices.append(inner_pos)
+                    if transformer is not None:
+                        left_vertices.append(transformer.transform(inner_pos[0], inner_pos[1]))
+                    else:
+                        left_vertices.append(inner_pos)
                 elif mirror_border == "right":
                     new_inner_pos = self.calc_border("outer", pos, local_width_offset)[
                         0
                     ]
                     modified_width = np.linalg.norm(new_inner_pos - outer_pos)
 
                     local_width_offset = (
                         math.copysign(1, local_width_offset) * last_width_difference
                     )
                     if modified_width < original_width:
-                        left_vertices.append(
-                            self.calc_border("inner", pos, local_width_offset)[0]
-                        )
+                        new_vertex = self.calc_border("inner", pos, local_width_offset)[0]
+                        if transformer is not None:
+                            left_vertices.append(transformer.transform(new_vertex[0], new_vertex[1]))
+                        else:
+                            left_vertices.append(new_vertex)
                     elif modified_width > original_width + adjacent_width:
-                        left_vertices.append(adj_inner_pos)
+                        if transformer is not None:
+                            left_vertices.append(transformer.transform(adj_inner_pos[0], adj_inner_pos[1]))
+                        else:
+                            left_vertices.append(adj_inner_pos)
                     else:
-                        left_vertices.append(new_inner_pos)
+                        if transformer is not None:
+                            left_vertices.append(transformer.transform(new_inner_pos[0], new_inner_pos[1]))
+                        else:
+                            left_vertices.append(new_inner_pos)
                         last_width_difference = abs(modified_width - original_width)
 
-                    right_vertices.append(outer_pos)
+                    if transformer is not None:
+                        right_vertices.append(transformer.transform(outer_pos[0], outer_pos[1]))
+                    else:
+                        right_vertices.append(outer_pos)
 
         left_vertices, right_vertices = (
             np.array(left_vertices),
             np.array(right_vertices),
         )
         # right_vertices = np.array(right_vertices)
 
@@ -425,17 +436,15 @@
 
     def _calc_border_positions(self, precision: float) -> np.ndarray:
         """Determine the positions along the border where the coordinates
         of the border should be calculated.
 
         :param precision: Number which indicates at which space interval (in curve parameter ds)
                         the coordinates of the boundaries should be calculated.
-        :type precision: float
         :return: Array with the ordered positions.
-        :rtype: np.ndarray
         """
         poses = np.array([])
         for i, parametric_lane in enumerate(self.parametric_lanes):
             num_steps = int(max(2, np.ceil(parametric_lane.length / float(precision))))
             if not i:
                 idx = 0
             else:
@@ -446,32 +455,32 @@
                 np.linspace(0, parametric_lane.length, num_steps)[idx::]
                 + self._geo_lengths[i],
             )
 
         return poses
 
     def _set_adjacent_lanes(self, lanelet: ConversionLanelet):
-        """While converting a ParametricLaneGroup to a Lanelet, set
+        """
+        While converting a ParametricLaneGroup to a Lanelet, set
         the proper attributes relating to adjacent lanes.
+
         :param lanelet: The lanelet which is created from the ParametricLaneGroup
-        :type lanelet: :class:`ConversionLanelet`
         """
         if self.inner_neighbour is not None:
             lanelet.adj_left = self.inner_neighbour
             lanelet.adj_left_same_direction = self.inner_neighbour_same_direction
 
         if self.outer_neighbour is not None:
             lanelet.adj_right = self.outer_neighbour
             lanelet.adj_right_same_direction = True
 
     def maximum_width(self) -> float:
         """Get the maximum width of the lanelet.
 
         :return: Maximum width of all ParametricLanes in this group.
-        :rtype: float
         """
         total_maximum = 0
 
         for plane in self.parametric_lanes:
             _, maximum = plane.maximum_width()
             if maximum > total_maximum:
                 total_maximum = maximum
@@ -480,20 +489,17 @@
 
     def first_zero_width_change_position(
         self, reverse: bool = False, reference_width: float = 0.0
     ) -> Tuple[Optional[float], Optional[float]]:
         """Get the earliest point of the ParametricLaneGroup where the width change is zero.
 
         :param reverse: True if checking should start from end of lanelet. Default is False
-        :type reverse: bool
         :param reference_width: Width for which width at zero width change position has
                             to be greater as. Default is 0.0.
-        :type reference_width: float
         :return: Position of ParametricLaneGroup (in curve parameter ds) where width change is zero.
-        :rtype: Tuple[Optional[float], Optional[float]]
         """
         s_pos = 0
         positions = []
 
         # total_maximum = self.maximum_width()
 
         for plane in self.parametric_lanes:
@@ -508,10 +514,10 @@
         # if lanelet has zero width change and its width
         # is either near the maximum or it is greater than the reference width
         # the position can be used
         for pos, val in positions:
             if val > 0.9 * reference_width or val > 0.9 * self.maximum_width():
                 if (pos == 0.0 and not reverse) or (pos == self.length and reverse):
                     continue
-                return (pos, val)
+                return pos, val
 
-        return (None, None)
+        return None, None
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/traffic_signals.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/plane_elements/traffic_signals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-import iso3166
 import numpy as np
-import warnings
+import logging
 import enum
 from crdesigner.map_conversion.opendrive.opendrive_conversion import utils
 from typing import Union, Tuple, List
 
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.road import Road
 from crdesigner.map_conversion.common.utils import generate_unique_id
+from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadLanes import LaneSection
+from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadSignal import Signal
 
 from commonroad.scenario.traffic_sign import TrafficSign, TrafficLight, TrafficSignElement, TrafficSignIDZamunda, \
     TrafficSignIDGermany, TrafficSignIDUsa, TrafficSignIDChina, TrafficSignIDSpain, TrafficSignIDRussia
 from commonroad.scenario.lanelet import StopLine, LineMarking
 
 
 def extract_traffic_element_id(signal_type: str, signal_subtype: str, traffic_sign_enum: enum) \
         -> Union[TrafficSignIDZamunda, TrafficSignIDGermany, TrafficSignIDUsa, TrafficSignIDChina,
                  TrafficSignIDSpain, TrafficSignIDRussia]:
     """Extract the traffic element id from the signal type and subtype string.
 
     :param signal_type: Signal type of the traffic element
-    :type signal_type: str
     :param signal_subtype: Subtype of the traffic element
-    :type signal_subtype: str
     :param traffic_sign_enum: Enumeration of country-specific traffic signs
-    :type traffic_sign_enum: enum
     :return: The extracted traffic element id.
-    :rtype: Union[TrafficSignIDZamunda, TrafficSignIDGermany, TrafficSignIDUsa, TrafficSignIDChina,
-                 TrafficSignIDSpain, TrafficSignIDRussia]
     """
     if signal_type in set(item.value for item in traffic_sign_enum):
         element_id = traffic_sign_enum(signal_type)
     elif signal_type + "-" + signal_subtype in set(item.value for item in traffic_sign_enum):
         element_id = traffic_sign_enum(signal_type + "-" + str(signal_subtype))
+    elif (traffic_sign_enum is TrafficSignIDGermany or traffic_sign_enum is TrafficSignIDZamunda) \
+            and signal_type == "252":  # traffic sign ID 252 is replaced by 260
+        element_id = traffic_sign_enum("260")
     else:
-        warnings.warn("OpenDRIVE/traffic_signals.py: Unknown {}"
-                      " of ID {} of subtype {}!".format(traffic_sign_enum.__name__, signal_type, signal_subtype))
+        logging.warning("OpenDRIVE/traffic_signals.py: Unknown {} of ID {} of subtype {}!".format(
+                traffic_sign_enum.__name__, signal_type, signal_subtype))
         element_id = traffic_sign_enum.UNKNOWN
 
     return element_id
 
 
 def get_traffic_signals(road: Road) -> Tuple[List[TrafficLight], List[TrafficSign], List[StopLine]]:
     """Extracts traffic_lights, traffic_signs, stop_lines from a road.
 
     :param road: The road object from which to extract signals.
-    :type road: :class:`Road`
     :return: lists of traffic_lights, traffic_signs, stop_lines
-    :rtype: tuple[list[TrafficLight], list[TrafficSign], list[StopLine]]
     """
     traffic_signs = []
     traffic_lights = []
     stop_lines = []
 
     # TODO: Stop lines are created and appended to the list for DEU and OpenDrive format.
     # This has been replicated for other countries but has not been tested with a test case
@@ -169,28 +166,24 @@
                 traffic_lights.append(traffic_light)
             else:
                 continue
 
     return traffic_lights, traffic_signs, stop_lines
 
 
-def calculate_stop_line_position(lane_sections, signal, position, tangent) -> Tuple[np.ndarray, np.ndarray]:
+def calculate_stop_line_position(lane_sections: List[LaneSection], signal: Signal, position: np.ndarray,
+                                 tangent: float) -> Tuple[np.ndarray, np.ndarray]:
     """Function to calculate the 2 points that define the stop line which
     is a straight line from one edge of the road to the other.
 
     :param lane_sections: Opendrive lane_sections list containing the lane_section parsed lane_section class
-    :type lane_sections: list
     :param signal: Signal object, in this case the stop line.
-    :type signal: :class:`StopLine`
     :param position: initial position as calculated in the get_traffic_signals function
-    :type position: np.ndarray
     :param tangent: tangent value as calculated in the get_traffic_signals function
-    :type tangent: float
     :return: Positions of the stop line
-    :rtype: tuple[np.ndarray, np.ndarray]
     """
     total_width = 0
     for lane_section in lane_sections:
         for lane in lane_section.allLanes:
             # Stop line width only depends on drivable lanes
             if lane.id != 0 and lane.type in ["driving", "onRamp", "offRamp", "exit", "entry"]:
                 for width in lane.widths:
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_conversion/utils.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_conversion/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 import iso3166
 from dataclasses import dataclass
 from typing import Union
 from commonroad.scenario.traffic_sign import TrafficSignIDZamunda, TrafficSignIDGermany, TrafficSignIDUsa, \
     TrafficSignIDChina, TrafficSignIDSpain, TrafficSignIDRussia, TrafficSignIDArgentina, TrafficSignIDBelgium, \
     TrafficSignIDFrance, TrafficSignIDGreece, TrafficSignIDCroatia, TrafficSignIDItaly, TrafficSignIDPuertoRico
 
-@dataclass
-class CustomDefaultLaneletType:
-    general_lanelet_type_activ: bool  # activates whether certain lanelet type should be added to all lanelets
-    general_lanelet_type: str  # lanelet type which is added to every lanelet (if activated)
-    driving_default_lanelet_type: str  # mapping of OpenDRIVE driveway lane type to a CommonRoad lanelet type
-    lanelet_types_backwards_compatible: bool # if active, converts OpenDRIVE lane types only to CommonRoad lanelet
-    # types compatible with commonroad-io==2022.1 (probably also even older ones)
-
 
 def encode_road_section_lane_width_id(road_id, section_id, lane_id, width_id) -> str:
     """Encodes a road section lane width with an ID.
 
     :param road_id: ID of road.
     :type road_id: int
     :param section_id: ID of RoadSection.
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/eulerspiral.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/eulerspiral.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,29 +21,29 @@
         :param kappa0: curvature at the starting point
         :return: The new curvature at position s and the magnitude by which the curvature
             changes with s in the form of (new curvature, magnitude of change)
         """
         return self._gamma * s + kappa0, self._gamma
 
     @staticmethod
-    def createFromLengthAndCurvature(length: float, curvStart: float, curvEnd: float) -> EulerSpiral:
+    def create_from_length_and_curvature(length: float, curv_start: float, curv_end: float) -> EulerSpiral:
         """
         Create an EulerSpiral from a given length with curveStart
         and curvEnd. This is how the OpenDrive format specifies
         EulerSpirals.
 
         :param length: Length of EulerSpiral
-        :param curvStart: Curvature at start of EulerSpiral
-        :param curvEnd: Curvature at end of EulerSpiral
-        :return: EulerSpiral - a new Clothoid
+        :param curv_start: Curvature at start of EulerSpiral
+        :param curv_end: Curvature at end of EulerSpiral
+        :return: EulerSpiral - a new clothoid
         """
         # if length is zero, assume zero curvature
         if length == 0:
             return EulerSpiral(0)
-        return EulerSpiral(1 * (curvEnd - curvStart) / length)
+        return EulerSpiral(1 * (curv_end - curv_start) / length)
 
     def calc(self, s: float, x0: float = 0, y0: float = 0, kappa0: float = 0, theta0: float = 0)\
             -> Tuple[float, float, float, Tuple[float, float]]:
         """
         Calculates x and y position, angle of the tangent and the curvature at position s.
         The position is described in complex representation with x being the real part of the
         number and y the imaginary part. The angle of the tangent is measured w.r.t.
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/geometry.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         :param curv_start: curvature at the start of the spiral
         :param curv_end: curvature at the end of the spiral
         """
         self._curv_start = curv_start
         self._curv_end = curv_end
 
         super().__init__(start_position=start_position, heading=heading, length=length)
-        self._spiral = EulerSpiral.createFromLengthAndCurvature(
+        self._spiral = EulerSpiral.create_from_length_and_curvature(
             self.length, self._curv_start, self._curv_end
         )
 
     def calc_position(self, s_pos:float, compute_curvature: bool = True) \
             -> Tuple[np.ndarray, float, Tuple[float, float]]:
         """
         Calculates x and y coordinates at position s along the line and returns additionally the orientation and
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/junction.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/junction.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/opendrive.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/opendrive.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,7 +156,8 @@
         self.date = date
         self.north = north
         self.south = south
         self.east = east
         self.west = west
         self.vendor = vendor
         self.geo_reference = None
+        self.offset = {"x": "0.0", "y": "0.0", "z": "0.0", "hdg":  "0.0"}
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadElevationProfile.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadElevationProfile.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLanes.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLanes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from typing import Union
 from typing import TYPE_CHECKING
+import logging
 if TYPE_CHECKING:
     from crdesigner.map_conversion.opendrive.opendrive_parser.elements.road import Road
 
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.road_record import RoadRecord
 import warnings
 
 
@@ -573,15 +574,15 @@
     :ivar _lane_change: Allows a lane change in the indicated direction, taking into account that lanes are numbered
         in ascending order from right to left. If the attribute is missing, “both” is used as default.
     :ivar _height: height of the road mark
     """
     def __init__(self):
         self._SOffset = None
         self._type = None
-        self._weight = None
+        self._weight = "standard"
         self._color = None
         self._material = None
         self._width = None
         self._lane_change = None
         self._height = None
 
     @property
@@ -636,75 +637,76 @@
     @weight.setter
     def weight(self, value: str):
         """
         Setter of the weight of the road mark.
         :param value: Value the weight is set to
         """
         if value is None:
-            warnings.warn("Parser could not find value for road_mark.weight, standard is used per default.")
+            logging.warning(
+                    "RoadMark::weight: Parser could not find value for road_mark.weight, standard is used per default.")
             value = "standard"
         self._weight = str(value)
 
     @property
     def color(self) -> str:
         """
         Color of the road mark.
 
         :getter: returns the color of the road mark
         :setter: sets the color of the road mark
         :type: string
         """
-        warnings.warn("Attribute color is not used for conversion!", DeprecationWarning)
+        logging.warning("RoadMark::color: Attribute color is not used for conversion!", DeprecationWarning)
         return self._color
 
     @color.setter
     def color(self, value):
         self._color = str(value)
 
     @property
     def material(self):
         """
         Material of the road mark.
 
         :getter: returns material of the road mark
         :type: string
         """
-        warnings.warn("Attribute material is not used for conversion!", DeprecationWarning)
+        logging.warning("RoadMark::material: Attribute material is not used for conversion!", DeprecationWarning)
         return self._material
 
     @property
     def width(self):
         """
         Width of the road mark.
 
         :getter: returns the width of the road mark
         :type:
         """
-        warnings.warn("Attribute width is not used for conversion!", DeprecationWarning)
+        logging.warning("RoadMark::width: Attribute width is not used for conversion!", DeprecationWarning)
         return self._width
 
     @property
     def lane_change(self):
         """
         Allows lane change according to value.
 
         :getter: returns allowed lane change
         :setter: sets lane_change
         :type: string
         """
-        warnings.warn("Attribute lane_change is not used for conversion", DeprecationWarning)
+        logging.warning("RoadMark::lane_change: Attribute lane_change is not used for conversion", DeprecationWarning)
         return self._lane_change
 
     @lane_change.setter
     def lane_change(self, value):
         self._lane_change = value
 
     @property
     def height(self):
         """
         Height of the road mark.
 
         :getter: returns the height of the road mark
         :type:
         """
-        warnings.warn("Attribute height is not used for conversion!", DeprecationWarning)
+        logging.warning("RoadMark::height: Attribute height is not used for conversion!", DeprecationWarning)
         return self._height
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLateralProfile.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLateralProfile.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLink.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadLink.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadObject.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,25 @@
         :setter: sets type of object
         :type: string
         """
         return self._type
 
     @type.setter
     def type(self, value):
-        road_types = ['barrier', 'bike', 'building', 'bus', 'car', 'crosswalk', 'gantry', 'motorbike', 'none',
-                      'obstacle', 'parkingSpace', 'patch', 'pedestrian', 'pole', 'railing', 'roadMark', 'soundBarrier',
-                      'streetLamp', 'trafficIsland', 'trailer', 'train', 'tram', 'tree', 'van', 'vegetation', 'wind']
+        road_types = ['barrier', 'bike', 'building', 'bus', 'car', 'crosswalk', 'ZebraCrossing', 'gantry', 'motorbike',
+                      'none', 'obstacle', 'parkingSpace', 'patch', 'pedestrian', 'pole', 'RoadSignPole', 'railing',
+                      'roadMark', 'roadmark', 'soundBarrier', 'streetLamp', 'Streetlamp', 'trafficIsland', 'trailer',
+                      'train', 'tram', 'tree', 'van', 'vegetation', 'wind', 'Guidepost']
         customs = ['permanentDelineator', 'emergencyCallBox', 'tunnel', 'arrowStraight', 'arrowRight', 'arrowMergeLeft',
-                   'arrowLeft', 'arrowLeftRight', 'arrowStraightLeft', 'arrowMergeRight', 'island', 'guidepost']
+                   'arrowLeft', 'arrowLeftRight', 'arrowStraightLeft', 'arrowMergeRight', 'island', 'guidepost',
+                   'roadpainting']
         if value == "-1":
             value = "none"
         if value not in road_types and value not in customs:
-            raise AttributeError("Value is not a valid object type!")
+            raise AttributeError("Value is not a supported object type!")
         self._type = str(value)
 
     @property
     def name(self) -> str:
         """
         Name of object.
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadPlanView.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadPlanView.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadSignal.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadSignal.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road_record.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/road_record.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadtype.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/elements/roadtype.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/opendrive/opendrive_parser/parser.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/opendrive/opendrive_parser/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import logging
 import warnings
-
+from typing import Optional, Dict
 import numpy as np
 from lxml import etree
 
 from crdesigner.map_conversion.common.utils import generate_unique_id
-
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.opendrive import OpenDrive, Header
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.road import Road
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadLink import Predecessor as RoadLinkPredecessor, \
     Successor as RoadLinkSuccessor, Neighbor as RoadLinkNeighbor
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadtype import RoadType, Speed as RoadTypeSpeed
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadElevationProfile import \
     ElevationRecord as RoadElevationProfile
@@ -20,15 +20,14 @@
     LaneBorder as RoadLaneSectionLaneBorder, RoadMark as RoadLaneRoadMark
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.junction import Junction, \
     Connection as JunctionConnection, LaneLink as JunctionConnectionLaneLink
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadSignal import Signal as RoadSignal, \
     SignalReference
 from crdesigner.map_conversion.opendrive.opendrive_parser.elements.roadObject import Object as RoadObject, \
     ObjectOutlineCorner
-from typing import Optional, TypeVar
 
 
 def parse_opendrive(file_path: str) -> OpenDrive:
     """
     Tries to parse XML tree, returns OpenDRIVE object
 
     :param file_path: path to opendrive
@@ -117,48 +116,47 @@
     if val is None:
         warnings.warn("Parser could not find value for " + name + ", " + default + " is used per default.")
         return default
     else:
         return val
 
 
-def parse_opendrive_road_geometry(new_road: Road, road_geometry: etree.ElementTree):
+def parse_opendrive_road_geometry(new_road: Road, road_geometry: etree.ElementTree, offset: Dict[str, str]):
     """
     Parse OpenDRIVE road geometry and appends it to road object.
 
     :param new_road: Road to append the parsed road geometry
     :param road_geometry: XML element which contains the information
+    :param offset: Offset defined in OpenDRIVE.
     """
-    start_coord = [float(road_geometry.get("x")), float(road_geometry.get("y"))]
+    start_coord = np.array([float(road_geometry.get("x")) - float(offset["x"]),
+                            float(road_geometry.get("y")) - float(offset["y"])])
 
     if road_geometry.find("line") is not None:
-        new_road.planView.add_line(start_coord, float(road_geometry.get("hdg")), float(road_geometry.get("length")), )
+        new_road.planView.add_line(start_coord, float(road_geometry.get("hdg")) - float(offset["hdg"]),
+                                   float(road_geometry.get("length")))
 
     elif road_geometry.find("spiral") is not None:
         curv_start = float(defaultval(road_geometry.find("spiral").get("curvStart"), "spiral.curvStart"))
         curv_end = float(defaultval(road_geometry.find("spiral").get("curvEnd"), "spiral.curvEnd"))
         if np.isclose(curv_start, curv_end):
             raise AttributeError("Curvature at the start and at the end of a spiral must be different")
-        new_road.planView.add_spiral(start_coord, float(road_geometry.get("hdg")), float(road_geometry.get("length")),
-                                     curv_start,
-                                     curv_end,)
+        new_road.planView.add_spiral(start_coord, float(road_geometry.get("hdg")) - float(offset["hdg"]),
+                                     float(road_geometry.get("length")), curv_start, curv_end,)
     elif road_geometry.find("arc") is not None:
-        new_road.planView.add_arc(start_coord, float(road_geometry.get("hdg")), float(road_geometry.get("length")),
+        new_road.planView.add_arc(start_coord, float(road_geometry.get("hdg")) - float(offset["hdg"]),
+                                  float(road_geometry.get("length")),
                                   float(road_geometry.find("arc").get("curvature")),)
 
     elif road_geometry.find("poly3") is not None:
         new_road.planView.add_poly3(start_coord, float(road_geometry.get("hdg")), float(road_geometry.get("length")),
-                                    float(
-                                            defaultval(road_geometry.find("poly3").get("a"), "poly3.a")),
-                                    float(
-                                            defaultval(road_geometry.find("poly3").get("b"), "poly3.b")),
-                                    float(
-                                            defaultval(road_geometry.find("poly3").get("c"), "poly3.c")),
-                                    float(
-                                            defaultval(road_geometry.find("poly3").get("d"), "poly3.d")),)# raise
+                                    float(defaultval(road_geometry.find("poly3").get("a"), "poly3.a")),
+                                    float(defaultval(road_geometry.find("poly3").get("b"), "poly3.b")),
+                                    float(defaultval(road_geometry.find("poly3").get("c"), "poly3.c")),
+                                    float(defaultval(road_geometry.find("poly3").get("d"), "poly3.d")),)
         # NotImplementedError()
 
     elif road_geometry.find("paramPoly3") is not None:
         if road_geometry.find("paramPoly3").get("pRange"):
 
             if road_geometry.find("paramPoly3").get("pRange") == "arcLength":
                 p_max = float(road_geometry.get("length"))
@@ -339,15 +337,16 @@
                 new_lane.has_border_record = True
 
             # Road Marks
             for mark in lane.findall("roadMark"):
                 road_mark = RoadLaneRoadMark()
 
                 road_mark.type = mark.get("type")
-                road_mark.weight = mark.get("weight")
+                if mark.get("weight") is not None:
+                    road_mark.weight = mark.get("weight")
                 road_mark.SOffset = mark.get("sOffset")
 
                 new_lane.road_mark.append(road_mark)
 
             # Material and Rules are not implemented in CommonRoad -> no need
 
             # Visiblility -> not part of ASAM OpenDRIVE 1.7.0 anymore
@@ -445,15 +444,15 @@
 
     # Type
     for opendrive_xml_road_type in road.findall("type"):
         parse_opendrive_road_type(new_road, opendrive_xml_road_type)
 
     # Plan view
     for road_geometry in road.find("planView").findall("geometry"):
-        parse_opendrive_road_geometry(new_road, road_geometry)
+        parse_opendrive_road_geometry(new_road, road_geometry, opendrive.header.offset)
     # Elevation profile
     road_elevation_profile = road.find("elevationProfile")
     if road_elevation_profile is not None:
         parse_opendrive_road_elevation_profile(new_road, road_elevation_profile)
 
     # Lateral profile
     road_lateral_profile = road.find("lateralProfile")
@@ -545,15 +544,16 @@
         if obj.get("pitch") is not None:
             road_object.pitch = obj.get("pitch")
         if obj.get("roll") is not None:
             road_object.roll = obj.get("roll")
 
         road_object.outline = corners
     except:
-        print("Error during parsing of road objects.")
+        logging.error("parse_opendrive_road_object: Error during parsing of road objects. "
+                      "Object id {}".format(obj.attrib.get("id")))
 
     new_road.addObject(road_object)
 
 
 def calculate_lane_section_lengths(new_road: Road):
     """
     Calculates lane section length for OpenDRIVE road.
@@ -595,14 +595,18 @@
                            header.get("date"), header.get("north"), header.get("south"), header.get("east"),
                            header.get("west"), header.get("vendor"), )
 
     # Reference
     if header.find("geoReference") is not None:
         parsed_header.geo_reference = header.find("geoReference").text
 
+    # offset {x: , y: , z: , hdg:}
+    if header.find("offset") is not None:
+        parsed_header.offset = header.find("offset").attrib
+
     opendrive.header = parsed_header
 
 
 def parse_opendrive_junction(opendrive: OpenDrive, junction: etree.ElementTree):
     """
     Parse OpenDRIVE junction and appends it to OpenDRIVE object.
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/config.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/config.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/converter.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/converter.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/cleanup.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/cleanup.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/export.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/cr_operations/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import utm
 
 from crdesigner.map_conversion.osm2cr import config
 from crdesigner.map_conversion.osm2cr.converter_modules.graph_operations import road_graph as rg
 from crdesigner.map_conversion.osm2cr.converter_modules.intermediate_operations.intermediate_format import \
     IntermediateFormat
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.osm2cr.converter_modules.utility.idgenerator import get_id
 from crdesigner.map_conversion.osm2cr.converter_modules.utility.geonamesID import get_geonamesID
 from crdesigner.map_conversion.osm2cr.converter_modules.cr_operations.cleanup import sanitize
 
 # CommonRoad python tools are imported
 from commonroad.visualization.mp_renderer import MPRenderer
 from commonroad.common.file_writer import CommonRoadFileWriter, OverwriteExistingFile
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/intersection_merger.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/intersection_merger.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/lane_linker.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/lane_linker.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/mapillary.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/mapillary.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/offsetter.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/offsetter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module provides a method to offset roads at certain occasions to smooth the course of consecutive lanes.
 """
 from crdesigner.map_conversion.osm2cr.converter_modules.graph_operations import road_graph as rg, lane_linker
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.osm2cr import config
 
 
 def offset_graph(graph: rg.Graph) -> None:
     """
     performs an offset on roads in the graph to keep passing lanes straight
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/restrictions.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/restrictions.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import logging
 from typing import List, Set, Tuple, Optional
 from ordered_set import OrderedSet
 import numpy as np
 
 from crdesigner.map_conversion.osm2cr import config
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 
 from ._graph_node import GraphNode
 from ._graph_edge import GraphEdge
 from ._graph_traffic_light import GraphTrafficLight
 from ._graph_traffic_sign import GraphTrafficSign
 from ._graph_lane import Lane
 from ._graph_functions import (
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_edge.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import math
 from typing import List, Set, Tuple, Optional
 from ordered_set import OrderedSet
 import numpy as np
 
 from crdesigner.map_conversion.osm2cr import config
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.osm2cr.converter_modules.utility.custom_types import (
     Road_info,
     Assumption_info,
 )
 
 from ._graph_node import GraphNode
 from ._graph_lane import Lane
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_functions.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from queue import Queue
 from typing import List, Set, Tuple
 import numpy as np
 
 from crdesigner.map_conversion.osm2cr import config
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 
 
 def graph_search(center_node: "GraphNode") -> Tuple[Set["GraphNode"], Set["GraphEdge"]]:
     """
     searches all elements connected to center_node from a graph and returns them
 
     :param center_node: the node to search from
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_lane.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_lane.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 """
 
 import math
 from typing import List, Set, Optional
 import numpy as np
 
 from commonroad.geometry.shape import Polygon
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry, idgenerator
+from crdesigner.map_conversion.osm2cr.converter_modules.utility import idgenerator
+from crdesigner.map_conversion.common import geometry
 
 from ._graph_node import GraphNode
 from ._graph_traffic_light import GraphTrafficLight
 from ._graph_traffic_sign import GraphTrafficSign
 
 
 class Lane:
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_node.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 GraphNode class
 """
 
 from typing import Set
 import numpy as np
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 
 
 class GraphNode:
     """
     Class that represents a node in the graph
 
     """
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_light.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_light.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_sign.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_graph_traffic_sign.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_sublayered_graph.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/road_graph/_sublayered_graph.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/segment_clusters.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/segment_clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This module holds all methods necessary to cluster segments at intersections.
 """
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.osm2cr.converter_modules.graph_operations import road_graph as rg
 from crdesigner.map_conversion.osm2cr import config
 
 import numpy as np
 from typing import Set, Dict, List, Tuple
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/traffic_sign_parser.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/graph_operations/traffic_sign_parser.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_edge.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_edge.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_format.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from commonroad.scenario.state import CustomState, InitialState
 from commonroad.planning.goal import GoalRegion
 from commonroad.common.util import Interval
 from commonroad.geometry.shape import Rectangle, Circle
 
 from crdesigner.map_conversion.osm2cr.converter_modules.graph_operations.road_graph import Graph
 from crdesigner.map_conversion.osm2cr import config
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry, idgenerator
+from crdesigner.map_conversion.osm2cr.converter_modules.utility import idgenerator
+from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.osm2cr.converter_modules.intermediate_operations.intersection_enhancement import \
     intersection_enhancement
 
 
 from ._intermediate_node import Node
 from ._intermediate_edge import Edge
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_node.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intermediate_format/_intermediate_node.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module holds the classes required for the intermediate format
 """
 
 __author__ = "Behtarin Ferdousi"
 
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 
 
 class Node:
     """
     Class to represent the nodes in the intermediate format
     """
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intersection_enhancement.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/intersection_enhancement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module is used to enhance intersections with traffic lights.
 """
 
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry, idgenerator
+from crdesigner.map_conversion.osm2cr.converter_modules.utility import idgenerator
+from crdesigner.map_conversion.common import geometry
 from crdesigner.map_conversion.osm2cr.converter_modules.intermediate_operations.traffic_light_generator import \
     TrafficLightGenerator
 
 
 def intersection_enhancement(intermediate_format):
     """
     Enhance intersections with traffic lights.
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/traffic_light_generator.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/intermediate_operations/traffic_light_generator.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/downloader.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/downloader.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/info_deduction.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/info_deduction.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/osm_parser.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/osm_operations/osm_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from crdesigner.map_conversion.osm2cr import config
 from crdesigner.map_conversion.osm2cr.converter_modules.graph_operations import road_graph as rg
 from crdesigner.map_conversion.osm2cr.converter_modules.graph_operations.restrictions import Restriction
 from crdesigner.map_conversion.osm2cr.converter_modules.osm_operations import info_deduction as i_d
 from crdesigner.map_conversion.osm2cr.converter_modules.utility import idgenerator
 from crdesigner.map_conversion.osm2cr.converter_modules.utility.custom_types import Road_info
-from crdesigner.map_conversion.osm2cr.converter_modules.utility.geometry import (
+from crdesigner.map_conversion.common.geometry import (
     Point,
     is_corner,
     Area,
     lon_lat_to_cartesian,
 )
 
 # type def
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/geometry.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/common/geometry.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/geonamesID.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/geonamesID.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/graph_analysis.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/idgenerator.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/idgenerator.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/converter_modules/utility/plots.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/converter_modules/utility/plots.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/osm2cr/main.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/osm2cr/main.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/config.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/config.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/converter.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/converter.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/mapping.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/mapping.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_light.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_light.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_sign.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/cr2sumo/traffic_sign.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/merge.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/merge.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/sumo2cr.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/sumo2cr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import subprocess
 
 from commonroad.scenario.scenario import Scenario
 from crdesigner.map_conversion.opendrive.opendrive_conversion.network import Network
 from crdesigner.map_conversion.opendrive.opendrive_parser.parser import parse_opendrive
-from crdesigner.configurations.get_configs import get_configs
 from lxml import etree
 
 from PyQt5.QtWidgets import QMessageBox
 
 
 def convert_net_to_cr(net_file: str, verbose: bool = False) -> Scenario:
     """
@@ -38,16 +37,15 @@
         print('converted to OpenDrive (.xodr)')
 
     # convert to commonroad using opendrive2lanelet
     # import, parse and convert OpenDRIVE file
     with open(opendrive_file, "r") as fi:
         open_drive = parse_opendrive(etree.parse(fi).getroot())
 
-    config = get_configs().opendrive
-    road_network = Network(config)
+    road_network = Network()
     road_network.load_opendrive(open_drive)
     scenario = road_network.export_commonroad_scenario()
     if verbose:
         print('converted to Commonroad (.cr.xml)')
 
     return scenario
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/sumolib_net.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/sumolib_net.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/DEU.typ.xml` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/DEU.typ.xml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/README.md` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/README.md`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/USA.typ.xml` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/USA.typ.xml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/ZAM.typ.xml` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/ZAM.typ.xml`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/templates/default.sumo.cfg` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/templates/default.sumo.cfg`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/map_conversion/sumo_map/util.py` & `commonroad_scenario_designer-0.7.1/crdesigner/map_conversion/sumo_map/util.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/start_gui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/start_gui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/cli/command_line.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/cli/command_line.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import argparse
 import sys
 
 from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.common.file_writer import CommonRoadFileWriter, OverwriteExistingFile
 from commonroad.scenario.scenario import Tag
 
+from crdesigner.config.config import Lanelet2ConversionParams, GeneralParams
 from crdesigner.start_gui import start_gui_new as start_gui
 from crdesigner.map_conversion.map_conversion_interface import commonroad_to_lanelet, lanelet_to_commonroad, \
     opendrive_to_commonroad, osm_to_commonroad, commonroad_to_sumo, sumo_to_commonroad
 
 
 def get_args() -> argparse.Namespace:
     """
@@ -29,14 +30,16 @@
     parser.add_argument('-c', '--source_commonroad', default=False, action='store_true',
                         help='indicator whether a conversion from CommonRoad to the other format should be performed, '
                              'default=False')
     parser.add_argument("-f", "--force-overwrite", action="store_true", help="overwrite existing file if it has same "
                                                                              "name as converted file")
     parser.add_argument("-t", "--tags", nargs="+", help="tags for the created scenario", default=set())
     parser.add_argument("--proj", help="proj-string to specify conversion for lanelet/lanelet2 format")
+    parser.add_argument("--autoware", help="create autoware-compatible lanelet2 map")
+    parser.add_argument("--local_coordinates", help="use local coordinates for lanelet2 map")
     parser.add_argument("--adjacencies", action="store_true", help="detect left and right adjacencies of "
                                                                    "lanelets if they do not share a common way "
                                                                    "(this is only used for lanelet/lanelet2 "
                                                                    "conversion)")
     parser.add_argument("--left-driving", action="store_true", help="set to true if map describes a left driving "
                                                                     "system, e.g., in Great Britain "
                                                                     "(this is only used for lanelet/lanelet2 "
@@ -87,26 +90,41 @@
                 "Not converting because file exists and option 'force-overwrite' not active",
                 file=sys.stderr,
             )
             sys.exit(-1)
 
         if args.source_commonroad:
             if args.mode == "map-convert-lanelet":
-                commonroad_to_lanelet(input_file, output_file, args.proj)
+                config = Lanelet2ConversionParams()
+                if args.proj:
+                    config.proj_string = args.proj
+                if args.autoware:
+                    config.autoware = args.autoware
+                if args.local_coordinates:
+                    config.local_coordinates = args.local_coordinates
+                commonroad_to_lanelet(input_file, output_file, config)
             if args.mode == "map-convert-sumo":
                 commonroad_to_sumo(input_file, output_file)
         else:
             if args.mode == "map-convert-osm":
                 scenario = osm_to_commonroad(input_file)
             elif args.mode == "map-convert-opendrive":
                 scenario = opendrive_to_commonroad(input_file)
             elif args.mode == "map-convert-sumo":
                 scenario = sumo_to_commonroad(input_file)
             elif args.mode == "map-convert-lanelet":
-                scenario = lanelet_to_commonroad(input_file, args.proj, args.left_driving, args.adjacencies)
+                config_lanelet2 = Lanelet2ConversionParams()
+                config_general = GeneralParams()
+                if args.proj:
+                    config_lanelet2.proj_string = args.proj
+                if args.adjacencies:
+                    config_lanelet2.adjacencies = args.adjacencies
+                if args.left_driving:
+                    config_lanelet2.left_driving = args.left_driving
+                scenario = lanelet_to_commonroad(input_file, config_general)
             else:
                 return
             tags = set([Tag(t) for t in args.tags])
             writer = CommonRoadFileWriter(
                 scenario=scenario,
                 planning_problem_set=PlanningProblemSet(),
                 author=args.author,
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/animated_viewer_wrapper.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/animated_viewer_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/animated_viewer.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/animated_viewer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import List, Optional, Union
 import numpy as np
 
 from PyQt5.QtWidgets import QFileDialog, QMessageBox
 from commonroad.planning.planning_problem import PlanningProblemSet
 
 from commonroad.scenario.intersection import Intersection
 from commonroad.scenario.scenario import Scenario
@@ -19,14 +19,41 @@
 
 from matplotlib.animation import FuncAnimation
 
 from .dynamic_canvas import DynamicCanvas
 from .helper import draw_lanelet_polygon
 
 
+def extract_plot_limits(lanelet_network: LaneletNetwork) -> Optional[List[float]]:
+    """
+    Extracts plot limits from a lanelet network
+
+    :param lanelet_network: CommonRoad lanelet network.
+    :return: Plot limits or none if lanelet network is empty.
+    """
+    margin = 50
+    if len(lanelet_network.lanelets) > 0:
+        x_lanelet_left = [point[0] for lanelet in lanelet_network.lanelets for point in
+                          lanelet.left_vertices]
+        y_lanelet_left = [point[1] for lanelet in lanelet_network.lanelets for point in
+                          lanelet.left_vertices]
+        x_lanelet_right = [point[0] for lanelet in lanelet_network.lanelets for point in
+                           lanelet.right_vertices]
+        y_lanelet_right = [point[1] for lanelet in lanelet_network.lanelets for point in
+                           lanelet.right_vertices]
+
+        x_min = min(x_lanelet_left + x_lanelet_right) - margin
+        y_min = min(y_lanelet_left + y_lanelet_right) - margin
+        x_max = max(x_lanelet_left + x_lanelet_right) + margin
+        y_max = max(y_lanelet_left + y_lanelet_right) + margin
+        return [x_min, x_max, y_min, y_max]
+    else:
+        return None
+
+
 class AnimatedViewer:
     def __init__(self, parent, callback_function):
 
         self.current_scenario = None
         self.current_pps = None
         self.parent = parent
         self.dynamic = DynamicCanvas(parent, width=5, height=10, dpi=100, animated_viewer=self)
@@ -71,20 +98,22 @@
             if not self._config:
                 def set_config(conf):
                     self._config = conf
                     self._calc_max_timestep()
                 config.subscribe(set_config)
             self._config = config.value
 
+        plot_limits = extract_plot_limits(scenario.lanelet_network)
+
         self._calc_max_timestep()
         if self.animation:
             self.time_step.value = 0
             self.animation.event_source.stop()
             self.animation = None
-        self.update_plot(clear_artists=True, new_file_added=new_file_added)
+        self.update_plot(clear_artists=True, new_file_added=new_file_added, plot_limits=plot_limits)
 
     def _init_animation(self):
         if not self.current_scenario:
             return
 
         print('init animation')
         scenario = self.current_scenario
@@ -205,20 +234,22 @@
 
     def update_plot(self,
                     sel_lanelets: Lanelet = None,
                     sel_intersection: Intersection = None,
                     time_step_changed: bool = False,
                     time_step: int = 0,
                     clear_artists: bool = False,
-                    new_file_added: bool = False):
+                    new_file_added: bool = False,
+                    plot_limits: Optional[List[float]] = None):
         """ Update the plot accordingly to the selection of scenario elements
         :param new_file_added: if a new cr file was created or added
         :param sel_lanelets: selected lanelet, defaults to None
         :param sel_intersection: selected intersection, defaults to None
         :param clear_artists: deletes artists from renderer (only required when opening new scenarios)
+        :param plot_limits: plot limits (area of axis) which should be visualized
         """
         if not isinstance(sel_lanelets, list) and sel_lanelets:
             sel_lanelets = [sel_lanelets]
 
         x_lim = self.dynamic.get_axes().get_xlim()
         y_lim = self.dynamic.get_axes().get_ylim()
 
@@ -248,18 +279,20 @@
             self.draw_lanelet_vertices(lanelet, ax)
 
         handles, labels = ax.get_legend_handles_labels()
         if sel_lanelets != None and config.LEGEND:
             legend = ax.legend(handles, labels)
             legend.set_zorder(50)
 
-        if new_file_added:
+        if new_file_added and plot_limits is None:
             # initialise the axis to a bigger range
             self.dynamic.set_limits([-50, 50, -50, 50])
             self.dynamic.draw_idle()
+        elif new_file_added:
+            self.dynamic.set_limits(plot_limits)
         # otherwise keep previous limits (persist zoom)
         else:
             self.dynamic.set_limits([x_lim[0], x_lim[1], y_lim[0], y_lim[1]])
             self.dynamic.draw_idle()
 
         self.dynamic.drawer.tight_layout()
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/dynamic_canvas.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/dynamic_canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 import copy
 from typing import List, Union
-from pygeodesy import flatLocal
 
 import PyQt5
+import numpy as np
+from PyQt5 import QtCore
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import QSizePolicy
-from PyQt5 import QtCore
-
-import numpy as np
-from matplotlib.backend_bases import MouseButton
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
-from matplotlib.figure import Figure
-from utm import from_latlon
-
-from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.common.util import Interval
-from commonroad.scenario.scenario import Scenario
-from commonroad.visualization.mp_renderer import MPRenderer
-from commonroad.visualization.draw_params import StaticObstacleParams, DynamicObstacleParams
 from commonroad.geometry.shape import Circle
-from commonroad.scenario.obstacle import StaticObstacle, DynamicObstacle
+from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.scenario.lanelet import Lanelet, LaneletType
+from commonroad.scenario.obstacle import StaticObstacle, DynamicObstacle
+from commonroad.scenario.scenario import Scenario
+from commonroad.visualization.draw_params import StaticObstacleParams, DynamicObstacleParams
+from commonroad.visualization.mp_renderer import MPRenderer
+from matplotlib.backend_bases import MouseButton
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from matplotlib.figure import Figure
 
-from crdesigner.ui.gui.mwindow.toolboxes.toolbox_ui import PosB
 from crdesigner.ui.gui.mwindow.animated_viewer_wrapper.commonroad_viewer.service_layer.draw_params_updater import \
     DrawParamsCustom
+from crdesigner.ui.gui.mwindow.service_layer import config
+from crdesigner.ui.gui.mwindow.service_layer.aerial_data import get_aerial_image_bing, get_aerial_image_ldbv, \
+    get_aerial_image_limits
+from crdesigner.ui.gui.mwindow.toolboxes.toolbox_ui import PosB
 from .helper import _merge_dict, calculate_closest_vertices, calculate_euclidean_distance, angle_between
-from .service_layer import update_draw_params_dynamic_only_based_on_zoom
-from .service_layer import update_draw_params_based_on_zoom
+from .service_layer import resize_lanelet_network
 from .service_layer import update_draw_params_based_on_scenario
+from .service_layer import update_draw_params_based_on_zoom
 from .service_layer import update_draw_params_dynamic_based_on_scenario
-from .service_layer import resize_lanelet_network
-from crdesigner.ui.gui.mwindow.service_layer import config
-
+from .service_layer import update_draw_params_dynamic_only_based_on_zoom
 from ...service_layer.map_creator import MapCreator
-from crdesigner.ui.gui.mwindow.service_layer.aerial_data import get_aerial_image_bing, get_aerial_image_ldbv
 
 ZOOM_FACTOR = 1.2
 
 
 class DynamicCanvas(FigureCanvas):
     """
     This canvas provides zoom with the mouse wheel.
@@ -85,15 +81,15 @@
         self.draw_lanelet_preview = None
         self.draw_append_lanelet_preview = None
         self.add_to_selected_preview = None
         self.add_to_selected = None
 
         self.draw_temporary_points = {}
         self.num_lanelets = 0
-        self.aerial_map_bounds = [48.263864, 11.655410, 48.261424, 11.660930]
+        self.aerial_map_bounds = (48.263864, 11.655410, 48.261424, 11.660930)
         self.show_aerial = False
 
         super().__init__(self.drawer)
 
         self._parent = parent
         self.setParent(parent)
         self.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
@@ -864,85 +860,48 @@
         self.draw_idle()
         self.num_lanelets = len(self.animated_viewer.current_scenario.lanelet_network.lanelets)
 
     def show_aerial_image(self):
         """
         shows the current (previously loaded) aerial image in the plot as a background
         """
-        self.ax.imshow(self.current_aerial_image, aspect='auto', extent=self.image_limits, alpha=0.75)
+        self.ax.imshow(self.current_aerial_image, aspect='equal', extent=self.image_limits, alpha=0.75)
+        self.ax.set_xlim(self.image_limits[0], self.image_limits[1])
+        self.ax.set_ylim(self.image_limits[2], self.image_limits[3])
 
-    def activate_aerial_image(self, bing: bool, lat1: float, lon1: float, lat2: float, lon2: float,
-                              center_at_zero: bool):
+    def activate_aerial_image(self, bing: bool, lat1: float, lon1: float, lat2: float, lon2: float):
         """
-        loads the aerial image with the following gps coordinates
+        loads the aerial image with the following gps coordinates...
+        :param bing: whether image should be loaded from bing
         :param lat1: northern bound
         :param lon1: western bound
         :param lat2: southern bound
         :param lon2: eastern bound
-        :param center_at_zero: Boolean indicating whether image should be centered at origin.
-        and gets the corresponding plot limits for the image
+        ...and gets the corresponding plot limits for the image
         and activates its showing in the background by setting show_aerial on True
         """
         self.update_aerial_image(lat1, lon1, lat2, lon2)
+        extent = self.aerial_map_bounds
         if bing:
-            self.current_aerial_image, extent = \
-                get_aerial_image_bing(self.aerial_map_bounds[0], self.aerial_map_bounds[1], self.aerial_map_bounds[2],
-                                      self.aerial_map_bounds[3])
-        else:
-            self.current_aerial_image = \
-                get_aerial_image_ldbv(self.aerial_map_bounds[0], self.aerial_map_bounds[1], self.aerial_map_bounds[2],
-                                      self.aerial_map_bounds[3])
-        self.image_limits = \
-            self.get_aerial_image_limits(self.aerial_map_bounds[0], self.aerial_map_bounds[1],
-                                         self.aerial_map_bounds[2], self.aerial_map_bounds[3], center_at_zero)
+            self.current_aerial_image, extent = get_aerial_image_bing(self.aerial_map_bounds)
+        else:
+            self.current_aerial_image = get_aerial_image_ldbv(self.aerial_map_bounds)
+        self.image_limits = get_aerial_image_limits(extent, self.scenario)
 
         self.show_aerial = True
 
     def update_aerial_image(self, lat1: float, lon1: float, lat2: float, lon2: float):
         """
         updates the gps coordinates of the aerial image to be loaded then shown
         :param lat1: northern bound
         :param lon1: western bound
         :param lat2: southern bound
         :param lon2: eastern bound
         """
-        self.aerial_map_bounds[0] = lat1
-        self.aerial_map_bounds[1] = lon1
-        self.aerial_map_bounds[2] = lat2
-        self.aerial_map_bounds[3] = lon2
-
-    def get_aerial_image_limits(self, lat1: float, lon1: float, lat2: float, lon2: float, center_at_zero: bool) \
-            -> List[float]:
-        """
-        converts the gps coordinates to limits array [0, dist width, 0, dist height] where dist is the measurement
-        in meters for the side of the rectangle containing the area bound by these coordinates
-        :param lat1: northern bound
-        :param lon1: western bound
-        :param lat2: southern bound
-        :param lon2: eastern bound
-        :param center_at_zero: Boolean indicating whether image should be centered at origin.
-        :return: 2. limits of image (in meters)
-        """
-
-        # compute height out of distance between left upper (north-west) and left lower (south-west) vertex
-        height = flatLocal(lat1, lon1, lat2, lon1)
-        # compute width out of distance between right lower (south-east) and left lower (south-west) vertex
-        width = flatLocal(lat2, lon1, lat2, lon2)
-
-        if not center_at_zero:
-            # compute UTM coordinates for lower left point
-            lower_lat = lat2 + (lat2 - lat1) / 2
-            left_lon = lon1 + (lon2 - lon1) / 2
-
-            (coord1, coord2, zone_num, zone_let) = from_latlon(lower_lat, left_lon)
-            print(coord1, coord2)
-        else:
-            coord1 = 0
-            coord2 = 0
-        return [coord1, coord1 + width, coord2, coord2 + height]
+        self.aerial_map_bounds = lat1, lon1, lat2, lon2
 
     def deactivate_aerial_image(self):
         """
         deactivate the showing of the aerial image, called when user clicks on Remove button in road network toolbox
         """
         self.show_aerial = False
         self._update_map()
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/helper.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/helper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/draw_params_updater.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/draw_params_updater.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/general_services.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/general_services.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/scenario_resizer.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/commonroad_viewer/service_layer/scenario_resizer.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/gui_sumo_simulation.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/animated_viewer_wrapper/gui_sumo_simulation.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/crdesigner_console_wrapper.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/crdesigner_console_wrapper/crdesigner_console_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/mwindow.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/mwindow.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/aerial_data.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/aerial_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 This module provides methods to download and use aerial images from Bing Maps
 """
 import json
 import os
-import requests
-from requests.auth import HTTPBasicAuth
 from io import BytesIO
 from queue import Queue
 from threading import Thread
 from typing import List, Tuple
 from typing import Optional
 from urllib.request import urlopen, HTTPBasicAuthHandler, build_opener, install_opener
 
 import mercantile
+import requests
 from PIL import Image
 from PIL.JpegImagePlugin import JpegImageFile
+from commonroad.scenario.scenario import Scenario
+from pyproj import Proj
 
+from crdesigner.config.config import ProjectionMethods
 from crdesigner.map_conversion.osm2cr import config
 from crdesigner.ui.gui.mwindow.service_layer import config as config_settings
 
 IMAGE_RESOLUTION = 256
 
 bing_maps_api_response = None
 
@@ -96,14 +98,15 @@
 
         # get data
         data = s.get(request, headers=headers).json()
         if data['authenticationResultCode'] == 'ValidCredentials':
             return True
     return False
 
+
 def validate_ldbv_credentials() -> bool:
     url = "https://geoservices.bayern.de/wms/v2/ogc_dop20.cgi?service=wms&request=GetMap&version=1.1.1&bbox=11.65541,48.26142,11.66093,48.26386&width=100&height=100&layers=by_dop20c&format=image/jpeg&srs=EPSG:4326"
     ldbv_username = config_settings.LDBV_USERNAME
     ldbv_password = config_settings.LDBV_PASSWORD
 
     try:
         auth_handler = HTTPBasicAuthHandler()
@@ -112,14 +115,15 @@
         opener = build_opener(auth_handler)
         install_opener(opener)
         urlopen(url).read()
     except:
         return False
     return True
 
+
 def get_tile(quadkey: str) -> JpegImageFile:
     """
     takes a quadkey, downloads the corresponding tile if not present and converts it to an image
 
     :param quadkey: quadkey of tile
     :return: image
     """
@@ -144,15 +148,15 @@
             store_tile(quadkey, image)
         except:
             return get_tile(quadkey)
     return image
 
 
 def get_required_quadkeys(west: float, south: float, east: float, north: float, zoom: int) -> Tuple[
-    List[str], int, int, List[float]]:
+    List[str], int, int, Tuple[float, float, float, float]]:
     """
     gets quadkeys for all tiles in a region sorted by their x and y value
     returns also the number of different x and y values
 
     :param west: west end of the region
     :param south: south end of the region
     :param east: east end of the region
@@ -186,23 +190,24 @@
     for y, count in y_counts.items():
         assert count == y_length
 
     tiles = sorted(tiles, key=lambda x: (x.x, x.y))
     quadkeys = [mercantile.quadkey(tile) for tile in tiles]
 
     lnglat_top_left = mercantile.ul(tiles[0])
+
     horizontal_min = lnglat_top_left.lng
     vertical_max = lnglat_top_left.lat
 
     bbox_lower_right = mercantile.xy_bounds(tiles[-1])
     lnglat_lower_right = mercantile.lnglat(bbox_lower_right.right, bbox_lower_right.bottom)
+
     horizontal_max = lnglat_lower_right.lng
     vertical_min = lnglat_lower_right.lat
-
-    extent = [horizontal_min, horizontal_max, vertical_min, vertical_max]
+    extent = (vertical_max, horizontal_min, vertical_min, horizontal_max)
     return quadkeys, x_length, y_length, extent
 
 
 def put_images_together(images: List[Image.Image], x_count: int, y_count: int) -> Image.Image:
     """
     puts tiles together to one image
 
@@ -257,45 +262,42 @@
     for t in threads:
         t.join()
 
     result = [images[quadkey] for quadkey in quadkeys]
     return result
 
 
-def get_aerial_image_bing(lat1: float, lon1: float, lat2: float, lon2: float, zoom: int = 19) -> Tuple[
-    Image.Image, List[float]]:
+def get_aerial_image_bing(bounds: Tuple[float, float, float, float], zoom: int = 19) -> Tuple[Image.Image,
+Tuple[float, float, float, float]]:
     """
-    gets the image and coordinates to a sepcified aera from bing
-
-    :param lat1: northern  bound
-    :param lon1: western bound
-    :param lat2: southern bound
-    :param lon2: eastern bound
+    gets the image and coordinates to a specified aera from bing
+    :param bounds: northern, western, southern and eastern bound
     :param zoom: zoom level
     :return: Tuple: 1. image, 2. extent of image
     """
     assert 1 <= zoom <= 23
 
+    lat1, lon1, lat2, lon2 = bounds
+
     keys, x_count, y_count, extent = get_required_quadkeys(lon1, lat2, lon2, lat1, zoom)
     print("loading {} tiles".format(len(keys)))
     # images = [get_tile(key) for key in keys]
     images = download_all_images(keys)
     image = put_images_together(images, x_count, y_count)
     return image, extent
 
-def get_aerial_image_ldbv(lat1: float, lon1: float, lat2: float, lon2: float) -> Image.Image:
+
+def get_aerial_image_ldbv(bounds: Tuple[float, float, float, float]) -> Image.Image:
     """
-    gets the image and coordinates to a sepcified aera from ldbv
+    gets the image and coordinates to a specified area from LDBV
 
-    :param lat1: northern  bound
-    :param lon1: western bound
-    :param lat2: southern bound
-    :param lon2: eastern bound
+    :param bounds: northern, western, southern and eastern bound
     :return: Image
     """
+    lat1, lon1, lat2, lon2 = bounds
     ldbv_username = config_settings.LDBV_USERNAME
     ldbv_password = config_settings.LDBV_PASSWORD
 
     lat_diff = lat1 - lat2
     lon_diff = lon2 - lon1
 
     # compute number of pixels of width and height based on coordinate limits (bigger side has always 4000 pixels)
@@ -304,19 +306,42 @@
         lon_pixels = int(onep * lon_diff)
         lat_pixels = 4000
     else:
         onep = 4000 / lon_diff
         lat_pixels = int(onep * lat_diff)
         lon_pixels = 4000
 
-    url = "https://geoservices.bayern.de/wms/v2/ogc_dop20.cgi?service=wms&request=GetMap&version=1.1.1&bbox={},{},{},{}&width={}&height={}&layers=by_dop20c&format=image/jpeg&srs=EPSG:4326".format(str(lon1), str(lat2), str(lon2), str(lat1), str(lat_pixels), str(lon_pixels))
+    # Reference system of the bbox-coordinates. We use WGS 84 (i.e. the "normal" geodetic system with
+    #   longitude and latitude);
+    #   for other options, see https://geodatenonline.bayern.de/geodatenonline/seiten/wms_dop20cm?36
+    ref_system = "EPSG:4326"
+    url = f"https://geoservices.bayern.de/wms/v2/ogc_dop20.cgi?service=wms&request=GetMap&version=1.1.1&bbox={str(lon1)},{str(lat2)},{str(lon2)},{str(lat1)}&width={str(lat_pixels)}&height={str(lon_pixels)}&layers=by_dop20c&format=image/jpeg&srs={ref_system}"
 
     auth_handler = HTTPBasicAuthHandler()
     auth_handler.add_password(realm='WMS DOP20', uri='https://geoservices.bayern.de/wms/v2/ogc_dop20.cgi', user=ldbv_username, passwd=ldbv_password)
     opener = build_opener(auth_handler)
     install_opener(opener)
     tile = urlopen(url).read()
     image = Image.open(BytesIO(tile))
 
     return image
 
 
+def get_aerial_image_limits(bounds: Tuple[float, float, float, float], scenario: Scenario) -> Tuple[float, float,
+    float, float]:
+    """
+    :param bounds: bounds of the image region as latitude/longitude: (northern, western, southern, eastern)
+    :param scenario: CommonRoad scenario
+    :return bounds in scenario coordinates: (left, right, bottom, top)
+    """
+    lat1, lon1, lat2, lon2 = bounds
+    proj_string = None
+    loc = scenario.location
+    if loc is not None and loc.geo_transformation is not None:
+        proj_string = loc.geo_transformation.geo_reference
+    if proj_string is None:
+        proj_string = ProjectionMethods.pseudo_mercator.value
+    proj = Proj(proj_string)
+    lower_left = proj(longitude=lon1, latitude=lat2)
+    upper_right = proj(longitude=lon2, latitude=lat1)
+    return lower_left[0], upper_right[0], lower_left[1], upper_right[1]
+
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/config.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/config.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/converter_modules/opendrive_interface.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/opendrive_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 
 from PyQt5.QtWidgets import QFileDialog, QMessageBox
 
 from crdesigner.map_conversion.opendrive.opendrive_parser.parser import parse_opendrive
 from crdesigner.map_conversion.opendrive.opendrive_conversion.network import Network
 from crdesigner.ui.gui.mwindow.service_layer.converter_modules.converter_interface import ConverterInterface
-from crdesigner.configurations.get_configs import get_configs
 
 
 class OpenDRIVEInterface(ConverterInterface):
 
     def __init__(self, parent):
         self.cr_designer = parent
         self.loadedRoadNetwork = None
@@ -53,15 +52,15 @@
                 "OpenDRIVE error",
                 "There was an error during the loading of the selected OpenDRIVE file.\n\n{}"
                     .format(errorMsg),
                 QMessageBox.Ok,
             )
             return
 
-        self.loadedRoadNetwork = Network(get_configs().opendrive)
+        self.loadedRoadNetwork = Network()
         self.loadedRoadNetwork.load_opendrive(openDriveXml)
 
         self.cr_designer.text_browser.append(
             """Name: {}<br>Version: {}<br>Date: {}<br><br>OpenDRIVE
             Version {}.{}<br><br>Number of roads: {}<br>Total length
             of road network: {:.2f} meters""".format(
                 openDriveXml.header.name
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/converter_modules/osm_interface.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/converter_modules/osm_interface.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/errors.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/errors.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/general_services.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/general_services.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.ui` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/MainWindow.ui`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.ui` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/Sumo_simulate.ui`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/gui_settings_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/gui_settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/osm_settings_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/osm_settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/scenario_saving_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/settings_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_resources/sumo_settings_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_resources/sumo_settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_settings.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_settings.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.qrc` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/CR_Scenario_Designer.qrc`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/Groupe_6.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/Groupe_6.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_left.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_left.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_right.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_adjacent_right.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_lane.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/add_lane.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_redo.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_redo.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_undo.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/button_undo.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/close.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/close.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr.ico` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.ico` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr1.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr2.ico` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/cr2.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/drawing_mode.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/drawing_mode.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.ico` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/icon.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/merge_lanelet.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/merge_lanelet.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/new_file.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/new_file.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.svg` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/obstacle_toolbox.svg`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/open_file.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/open_file.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause_darkmode.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/pause_darkmode.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/play.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/play.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.svg` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/road_network_toolbox.svg`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/save.ico` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_file.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_file.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.svg` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/save_video.svg`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/split_lanelet.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/split_lanelet.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/target-darkmode.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/target-darkmode.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/target.png` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/target.png`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/gui_src/tools.ico` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/gui_src/tools.ico`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/help_actions.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/help_actions.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/map_creator.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/map_creator.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/osm_settings.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/osm_settings.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/osm_settings_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/osm_settings_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/services/config_default.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/config_default.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/services/plots_interactive.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/plots_interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 All plot functions in this module can plot in cartesian coordinates as well as in latitude and longitude.
 
 """
 from abc import ABC
 from typing import Tuple, List, Optional, Set, Dict, Union
 
 import numpy as np
-from PIL import Image
 from matplotlib.axes import Axes
 from matplotlib.collections import Collection, PathCollection
 from matplotlib.colors import to_rgba
 from matplotlib.lines import Line2D
 from matplotlib.patches import FancyArrow, Polygon, Patch, PathPatch
 from matplotlib.path import Path
 
 from crdesigner.map_conversion.osm2cr.converter_modules.graph_operations import road_graph as rg
-from crdesigner.map_conversion.osm2cr.converter_modules.utility import geometry
+from crdesigner.map_conversion.common import geometry
 
 PICKER_SIZE = 2
 LINE_WIDTH = 2.5
 SCATTER_SIZE = 200
 HIGHLIGHT_COLOR = "skyblue"
 STANDARD_COLOR = "black"
 POINT_COLOR = "dimgrey"
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/services/waitingspinnerwidget.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/services/waitingspinnerwidget.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/settings.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/settings.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/sumo_settings.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/sumo_settings.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/service_layer/util.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/service_layer/util.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/create_converter_toolbox.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/create_converter_toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 from crdesigner.ui.gui.mwindow.toolboxes.converter_toolbox.map_converter_toolbox import MapConversionToolbox
 from crdesigner.ui.gui.mwindow.toolboxes.service_layer.general_services import toolbox_callback
 
 
 def create_converter_toolbox(mwindow):
     """ Create the map converter toolbar_wrapper."""
     mwindow.map_converter_toolbox = MapConversionToolbox(mwindow.animated_viewer_wrapper.cr_viewer.current_scenario,
-                                                         lambda scenario: toolbox_callback(mwindow, scenario),
+                                                         lambda scenario: toolbox_callback(mwindow, scenario, True),
                                                          mwindow.crdesigner_console_wrapper.text_browser,
                                                          mwindow.obstacle_toolbox.sumo_simulation, mwindow)
     mwindow.addDockWidget(Qt.RightDockWidgetArea, mwindow.map_converter_toolbox)
     return mwindow.map_converter_toolbox  # for visibility
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,22 @@
 
 from crdesigner.map_conversion.osm2cr.converter_modules import converter
 from crdesigner.map_conversion.osm2cr.converter_modules.osm_operations.downloader import download_around_map
 from crdesigner.map_conversion.osm2cr import config
 from crdesigner.map_conversion.osm2cr.converter_modules.cr_operations.export import convert_to_scenario
 from crdesigner.map_conversion.osm2cr.converter_modules.graph_operations import road_graph as rg
 
-from crdesigner.ui.gui.mwindow.service_layer.converter_modules.osm_interface import OSMInterface
-
 from crdesigner.map_conversion.opendrive.opendrive_parser.parser import parse_opendrive
 from crdesigner.map_conversion.opendrive.opendrive_conversion.network import Network
 
 from crdesigner.map_conversion.lanelet2.lanelet2_parser import Lanelet2Parser
 from crdesigner.map_conversion.lanelet2.lanelet2cr import Lanelet2CRConverter
 from crdesigner.map_conversion.lanelet2.cr2lanelet import CR2LaneletConverter
 
-from crdesigner.configurations.get_configs import get_configs
-
+from crdesigner.ui.gui.mwindow.service_layer.converter_modules.osm_interface import OSMInterface
 from crdesigner.ui.gui.mwindow.animated_viewer_wrapper.gui_sumo_simulation import SUMO_AVAILABLE
 from crdesigner.ui.gui.mwindow.service_layer.services.waitingspinnerwidget import QtWaitingSpinner
 if SUMO_AVAILABLE:
     from crdesigner.ui.gui.mwindow.animated_viewer_wrapper.gui_sumo_simulation import SUMOSimulation
     from crdesigner.ui.gui.mwindow.service_layer.sumo_settings import SUMOSettings
     from crdesigner.map_conversion.sumo_map.sumo2cr import convert_net_to_cr
 
@@ -296,16 +293,15 @@
     def convert_open_drive_to_cr(self):
         """
         Starts the OpenDRIVE conversion process by picking a file and converting it without showing a spinner.
         """
         if self.open_drive_file is None:
             return
 
-        config = get_configs().opendrive
-        open_drive_network = Network(config)
+        open_drive_network = Network()
         open_drive_network.load_opendrive(self.open_drive_file)
 
         self.text_browser.append(
             """Name: {}<br>Version: {}<br>Date: {}<br><br>OpenDRIVE
             Version {}.{}""".format(
                 self.open_drive_file.header.name if self.open_drive_file.header.name else "<i>unset</i>",
                 self.open_drive_file.header.version,
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/converter_toolbox/map_converter_toolbox_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/create_obstacle_toolbox.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/create_obstacle_toolbox.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/obstacle_toolbox/obstacle_toolbox_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/create_road_network_toolbox.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/create_road_network_toolbox.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     def __init__(self, fun, roadNetworkToolbox):
         QRunnable.__init__(self)
         self.fun = fun
         self.roadNetworkToolbox = roadNetworkToolbox
 
     def run(self):
         self.fun()
-        QMetaObject.invokeMethod(self.roadNetworkToolbox, "stopSpinner",
-                                Qt.QueuedConnection,
-                                Q_ARG(str, "Conversion Ended"))
+        QMetaObject.invokeMethod(self.roadNetworkToolbox, "stopSpinner", Qt.QueuedConnection,
+                                 Q_ARG(str, "Conversion Ended"))
+
 
 class RoadNetworkToolbox(QDockWidget, ):
     def __init__(self, current_scenario: Scenario, text_browser, callback, tmp_folder: str, selection_changed_callback,
                  mwindow):
         super().__init__("Road Network Toolbox")
         self.road_network_toolbox_ui = RoadNetworkToolboxUI(mwindow)
         self.adjust_ui()
@@ -78,23 +78,23 @@
         # Lanelet buttons
         self.road_network_toolbox_ui.button_remove_lanelet.clicked.connect(lambda: self.remove_lanelet())
         self.road_network_toolbox_ui.button_attach_to_other_lanelet.clicked.connect(
                 lambda: self.attach_to_other_lanelet())
 
         # connect radiobuttons for adding to the adjust_add_sections function which shows and hides choices
         self.road_network_toolbox_ui.place_at_position.clicked.connect(
-            lambda: self.road_network_toolbox_ui.adjust_add_sections())
+                lambda: self.road_network_toolbox_ui.adjust_add_sections())
         self.road_network_toolbox_ui.connect_to_previous_selection.clicked.connect(
-            lambda: self.road_network_toolbox_ui.adjust_add_sections())
+                lambda: self.road_network_toolbox_ui.adjust_add_sections())
         self.road_network_toolbox_ui.connect_to_predecessors_selection.clicked.connect(
-            lambda: self.road_network_toolbox_ui.adjust_add_sections())
+                lambda: self.road_network_toolbox_ui.adjust_add_sections())
         self.road_network_toolbox_ui.connect_to_successors_selection.clicked.connect(
-            lambda: self.road_network_toolbox_ui.adjust_add_sections())
+                lambda: self.road_network_toolbox_ui.adjust_add_sections())
         self.road_network_toolbox_ui.connecting_radio_button_group.buttonClicked.connect(
-            lambda: self.initialize_basic_lanelet_information())
+                lambda: self.initialize_basic_lanelet_information())
 
         self.road_network_toolbox_ui.button_create_adjacent.clicked.connect(lambda: self.create_adjacent())
         self.road_network_toolbox_ui.button_connect_lanelets.clicked.connect(lambda: self.connect_lanelets())
         self.road_network_toolbox_ui.button_rotate_lanelet.clicked.connect(lambda: self.rotate_lanelet())
         self.road_network_toolbox_ui.button_translate_lanelet.clicked.connect(lambda: self.translate_lanelet())
         self.road_network_toolbox_ui.button_merge_lanelets.clicked.connect(lambda: self.merge_with_successor())
 
@@ -130,15 +130,14 @@
         self.road_network_toolbox_ui.button_add_intersection.clicked.connect(lambda: self.add_intersection())
         self.road_network_toolbox_ui.button_remove_intersection.clicked.connect(lambda: self.remove_intersection())
         self.road_network_toolbox_ui.button_update_intersection.clicked.connect(lambda: self.update_intersection())
         # Aerial Image buttons
         self.road_network_toolbox_ui.button_add_aerial_image.clicked.connect(lambda: self.show_aerial_image())
         self.road_network_toolbox_ui.button_remove_aerial_image.clicked.connect(lambda: self.remove_aerial_image())
 
-
     def refresh_toolbox(self, scenario: Scenario):
         self.current_scenario = scenario
         # refresh toolboxes based on the scenario
         self.set_default_road_network_list_information()
 
     def lanelet_selection_changed(self):
         selected_lanelet = self.selected_lanelet()
@@ -156,71 +155,81 @@
     def get_x_position_lanelet_start(self, update=False) -> float:
         """
         Extracts lanelet x-position of first center vertex.
 
         @return: x-position [m]
         """
         if not update:
-            if self.road_network_toolbox_ui.place_at_position.isChecked() and self.road_network_toolbox_ui.lanelet_start_position_x.text() and self.road_network_toolbox_ui.lanelet_start_position_x.text() != "-":
+            if self.road_network_toolbox_ui.place_at_position.isChecked() and \
+                    self.road_network_toolbox_ui.lanelet_start_position_x.text() and \
+self.road_network_toolbox_ui.lanelet_start_position_x.text() != "-":
                 return float(self.road_network_toolbox_ui.lanelet_start_position_x.text().replace(",", "."))
             else:
                 return 0
         else:
-            if self.road_network_toolbox_ui.selected_lanelet_start_position_x.text() and self.road_network_toolbox_ui.selected_lanelet_start_position_x.text() != "-":
+            if self.road_network_toolbox_ui.selected_lanelet_start_position_x.text() and \
+                    self.road_network_toolbox_ui.selected_lanelet_start_position_x.text() != "-":
                 return float(self.road_network_toolbox_ui.selected_lanelet_start_position_x.text().replace(",", "."))
             else:
                 return 0
 
     def get_y_position_lanelet_start(self, update=False) -> float:
         """
         Extracts lanelet y-position of first center vertex.
 
         @return: y-position [m]
         """
         if not update:
-            if self.road_network_toolbox_ui.place_at_position.isChecked() and self.road_network_toolbox_ui.lanelet_start_position_y.text() and self.road_network_toolbox_ui.lanelet_start_position_y.text() != "-":
+            if self.road_network_toolbox_ui.place_at_position.isChecked() and \
+self.road_network_toolbox_ui.lanelet_start_position_y.text() and \
+self.road_network_toolbox_ui.lanelet_start_position_y.text() != "-":
                 return float(self.road_network_toolbox_ui.lanelet_start_position_y.text().replace(",", "."))
             else:
                 return 0
         else:
-            if self.road_network_toolbox_ui.selected_lanelet_start_position_y.text() and self.road_network_toolbox_ui.selected_lanelet_start_position_y.text() != "-":
+            if self.road_network_toolbox_ui.selected_lanelet_start_position_y.text() and \
+self.road_network_toolbox_ui.selected_lanelet_start_position_y.text() != "-":
                 return float(self.road_network_toolbox_ui.selected_lanelet_start_position_y.text().replace(",", "."))
             else:
                 return 0
 
     def get_x_position_lanelet_end(self, update=False) -> float:
         """
         Extracts lanelet x-position of last center vertex.
 
         @return: x-position [m]
         """
         if not update:
-            if self.road_network_toolbox_ui.lanelet_end_position_x.text() and self.road_network_toolbox_ui.lanelet_end_position_x.text() != "-":
+            if self.road_network_toolbox_ui.lanelet_end_position_x.text() and \
+                    self.road_network_toolbox_ui.lanelet_end_position_x.text() != "-":
                 return float(self.road_network_toolbox_ui.lanelet_end_position_x.text().replace(",", "."))
             else:
                 return 0
         else:
-            if self.road_network_toolbox_ui.selected_lanelet_end_position_x.text() and self.road_network_toolbox_ui.selected_lanelet_end_position_x.text() != "-":
+            if self.road_network_toolbox_ui.selected_lanelet_end_position_x.text() and \
+                    self.road_network_toolbox_ui.selected_lanelet_end_position_x.text() != "-":
                 return float(self.road_network_toolbox_ui.selected_lanelet_end_position_x.text().replace(",", "."))
             else:
                 return 0
 
     def get_y_position_lanelet_end(self, update=False) -> float:
         """
         Extracts lanelet y-position of last center vertex.
 
         @return: y-position [m]
         """
         if not update:
-            if self.road_network_toolbox_ui.lanelet_end_position_y.text() and self.road_network_toolbox_ui.lanelet_end_position_y.text() != "-":
+            if self.road_network_toolbox_ui.lanelet_end_position_y.text() and \
+                    self.road_network_toolbox_ui.lanelet_end_position_y.text() != "-":
                 return float(self.road_network_toolbox_ui.lanelet_end_position_y.text().replace(",", "."))
             else:
                 return 0
         else:
-            if self.road_network_toolbox_ui.selected_lanelet_end_position_y.text() and self.road_network_toolbox_ui.selected_lanelet_end_position_y.text() != "-":
+            if self.road_network_toolbox_ui.selected_lanelet_end_position_y.text() and \
+                    self.road_network_toolbox_ui.selected_lanelet_end_position_y.text() != "-":
                 return float(self.road_network_toolbox_ui.selected_lanelet_end_position_y.text().replace(",", "."))
             else:
                 return 0
 
     def get_float(self, str) -> float:
         """
         Validates number and replace , with . to be able to insert german floats
@@ -285,35 +294,39 @@
         return lanelets
 
     def initialize_basic_lanelet_information(self):
         """
         Initializes lanelet GUI elements with lanelet information.
         """
 
-        if not self.road_network_toolbox_ui.place_at_position.isChecked() and not self.road_network_toolbox_ui.connect_to_previous_selection.isChecked() and not self.road_network_toolbox_ui.connect_to_predecessors_selection.isChecked() and not self.road_network_toolbox_ui.connect_to_successors_selection.isChecked():
+        if not self.road_network_toolbox_ui.place_at_position.isChecked() and not \
+self.road_network_toolbox_ui.connect_to_previous_selection.isChecked() and not \
+        self.road_network_toolbox_ui.connect_to_predecessors_selection.isChecked() and not \
+        self.road_network_toolbox_ui.connect_to_successors_selection.isChecked():
             self.road_network_toolbox_ui.adding_method = ""
             return
 
         if self.road_network_toolbox_ui.connect_to_predecessors_selection.isChecked():
             self.road_network_toolbox_ui.predecessors.view().pressed.connect(
-                self.initialize_predecessor_and_successor_fields)
+                    self.initialize_predecessor_and_successor_fields)
         elif self.road_network_toolbox_ui.connect_to_successors_selection.isChecked():
             self.road_network_toolbox_ui.successors.view().pressed.connect(
-                self.initialize_predecessor_and_successor_fields)
+                    self.initialize_predecessor_and_successor_fields)
 
         # Line marking fields
         line_markings = [e.value for e in LineMarking]
         self.road_network_toolbox_ui.line_marking_right.addItems(line_markings)
         self.road_network_toolbox_ui.line_marking_left.addItems(line_markings)
 
         # Advanced
         road_user_list = [r.value for r in RoadUser]
         lanelet_type_list = [e.value for e in LaneletType]
 
-        # When connect to previous is selected and the last added lanelet is not none, then initialize all fields with the value of the last lanelet
+        # When connect to previous is selected and the last added lanelet is not none, then initialize all fields
+        # with the value of the last lanelet
         if self.road_network_toolbox_ui.connect_to_previous_selection.isChecked():
             if self.last_added_lanelet_id is not None:
                 last_lanelet = self.current_scenario.lanelet_network.find_lanelet_by_id(self.last_added_lanelet_id)
                 self.road_network_toolbox_ui.previous_lanelet.addItem(str(last_lanelet.lanelet_id))
 
                 self.road_network_toolbox_ui.lanelet_length.setText(self.get_length(last_lanelet))
                 self.road_network_toolbox_ui.lanelet_width.setText(self.get_width(last_lanelet))
@@ -387,48 +400,50 @@
         line_markings_stop_line = [e.value for e in LineMarking if
                                    e.value not in [LineMarking.UNKNOWN.value, LineMarking.NO_MARKING.value]]
         self.road_network_toolbox_ui.line_marking_stop_line.addItems(line_markings_stop_line)
 
         # Neighboring fields
         self.road_network_toolbox_ui.predecessors.clear()
         self.road_network_toolbox_ui.predecessors.addItems(
-            ["None"] + [str(item) for item in self.collect_lanelet_ids()])
+                ["None"] + [str(item) for item in self.collect_lanelet_ids()])
         self.road_network_toolbox_ui.predecessors.setCurrentIndex(0)
 
         self.road_network_toolbox_ui.successors.clear()
         self.road_network_toolbox_ui.successors.addItems(["None"] + [str(item) for item in self.collect_lanelet_ids()])
         self.road_network_toolbox_ui.successors.setCurrentIndex(0)
 
         self.road_network_toolbox_ui.adjacent_right.clear()
         self.road_network_toolbox_ui.adjacent_right.addItems(
-            ["None"] + [str(item) for item in self.collect_lanelet_ids()])
+                ["None"] + [str(item) for item in self.collect_lanelet_ids()])
         self.road_network_toolbox_ui.adjacent_right.setCurrentIndex(0)
 
         self.road_network_toolbox_ui.adjacent_left.clear()
         self.road_network_toolbox_ui.adjacent_left.addItems(
-            ["None"] + [str(item) for item in self.collect_lanelet_ids()])
+                ["None"] + [str(item) for item in self.collect_lanelet_ids()])
         self.road_network_toolbox_ui.adjacent_left.setCurrentIndex(0)
 
         # Advanced
         self.road_network_toolbox_ui.lanelet_referenced_traffic_sign_ids.clear()
         self.road_network_toolbox_ui.lanelet_referenced_traffic_sign_ids.addItems(
-            ["None"] + [str(item) for item in self.collect_traffic_sign_ids()])
+                ["None"] + [str(item) for item in self.collect_traffic_sign_ids()])
         self.road_network_toolbox_ui.lanelet_referenced_traffic_sign_ids.setCurrentIndex(0)
 
         self.road_network_toolbox_ui.lanelet_referenced_traffic_light_ids.clear()
         self.road_network_toolbox_ui.lanelet_referenced_traffic_light_ids.addItems(
-            ["None"] + [str(item) for item in self.collect_traffic_light_ids()])
+                ["None"] + [str(item) for item in self.collect_traffic_light_ids()])
         self.road_network_toolbox_ui.lanelet_referenced_traffic_light_ids.setCurrentIndex(0)
 
     def initialize_predecessor_and_successor_fields(self):
         """
-        Initializes lanelet information fields according to the selected predecessor / successor when connect to predecessor / successor is selected
+        Initializes lanelet information fields according to the selected predecessor / successor when connect to
+        predecessor / successor is selected
         selects always the first in the list of predecessors / successors
         """
-        if len(self.road_network_toolbox_ui.predecessors.get_checked_items()) == 0 and len(self.road_network_toolbox_ui.successors.get_checked_items()) == 0:
+        if len(self.road_network_toolbox_ui.predecessors.get_checked_items()) == 0 and len(
+                self.road_network_toolbox_ui.successors.get_checked_items()) == 0:
             return
         if self.road_network_toolbox_ui.connect_to_predecessors_selection.isChecked():
             pred = self.road_network_toolbox_ui.predecessors.get_checked_items()[0]
             if not pred.isdigit():
                 return
             lanelet = self.current_scenario.lanelet_network.find_lanelet_by_id(int(pred))
         elif self.road_network_toolbox_ui.connect_to_successors_selection.isChecked():
@@ -610,15 +625,18 @@
         @param left_vertices: Left boundary of lanelet which should be updated.
         @param right_vertices: Right boundary of lanelet which should be updated.
         """
         if self.current_scenario is None:
             self.text_browser.append("Please create first a new scenario.")
             return
 
-        if not self.road_network_toolbox_ui.place_at_position.isChecked() and not self.road_network_toolbox_ui.connect_to_previous_selection.isChecked() and not self.road_network_toolbox_ui.connect_to_successors_selection.isChecked() and not self.road_network_toolbox_ui.connect_to_predecessors_selection.isChecked():
+        if not self.road_network_toolbox_ui.place_at_position.isChecked() and not \
+        self.road_network_toolbox_ui.connect_to_previous_selection.isChecked() and not \
+                self.road_network_toolbox_ui.connect_to_successors_selection.isChecked() and not \
+                self.road_network_toolbox_ui.connect_to_predecessors_selection.isChecked():
             self.text_browser.append("Please select an adding option.")
             return
 
         predecessors = [int(pre) for pre in self.road_network_toolbox_ui.predecessors.get_checked_items()]
         successors = [int(suc) for suc in self.road_network_toolbox_ui.successors.get_checked_items()]
 
         place_at_position = self.road_network_toolbox_ui.place_at_position.isChecked()
@@ -641,17 +659,19 @@
         lanelet_start_pos_y = self.get_y_position_lanelet_start(False)
 
         lanelet_width = self.get_float(self.road_network_toolbox_ui.lanelet_width)
         line_marking_left = LineMarking(self.road_network_toolbox_ui.line_marking_left.currentText())
         line_marking_right = LineMarking(self.road_network_toolbox_ui.line_marking_right.currentText())
         num_vertices = int(self.road_network_toolbox_ui.number_vertices.text())
         adjacent_left = int(
-            self.road_network_toolbox_ui.adjacent_left.currentText()) if self.road_network_toolbox_ui.adjacent_left.currentText() != "None" else None
+                self.road_network_toolbox_ui.adjacent_left.currentText()) if \
+                self.road_network_toolbox_ui.adjacent_left.currentText() != "None" else None
         adjacent_right = int(
-            self.road_network_toolbox_ui.adjacent_right.currentText()) if self.road_network_toolbox_ui.adjacent_right.currentText() != "None" else None
+                self.road_network_toolbox_ui.adjacent_right.currentText()) if \
+                self.road_network_toolbox_ui.adjacent_right.currentText() != "None" else None
         adjacent_left_same_direction = self.road_network_toolbox_ui.adjacent_left_same_direction.isChecked()
         adjacent_right_same_direction = self.road_network_toolbox_ui.adjacent_right_same_direction.isChecked()
         lanelet_type = {LaneletType(ty) for ty in self.road_network_toolbox_ui.lanelet_type.get_checked_items() if
                         ty != "None"}
         user_one_way = {RoadUser(user) for user in self.road_network_toolbox_ui.road_user_oneway.get_checked_items() if
                         user != "None"}
         user_bidirectional = {RoadUser(user) for user in
@@ -698,15 +718,15 @@
                                                  user_one_way, user_bidirectional, line_marking_left,
                                                  line_marking_right, stop_line, traffic_signs, traffic_lights,
                                                  stop_line_at_end, stop_line_at_beginning)
 
         if connect_to_last_selection:
             last_lanelet = self.current_scenario.lanelet_network.find_lanelet_by_id(self.last_added_lanelet_id)
             lanelet.translate_rotate(
-                np.array([last_lanelet.center_vertices[-1][0], last_lanelet.center_vertices[-1][1]]), 0)
+                    np.array([last_lanelet.center_vertices[-1][0], last_lanelet.center_vertices[-1][1]]), 0)
             MapCreator.fit_to_predecessor(last_lanelet, lanelet)
         elif connect_to_predecessors_selection:
             if len(predecessors) > 0:
                 predecessor = self.current_scenario.lanelet_network.find_lanelet_by_id(predecessors[0])
                 lanelet.translate_rotate(
                         np.array([predecessor.center_vertices[-1][0], predecessor.center_vertices[-1][1]]), 0)
                 MapCreator.fit_to_predecessor(predecessor, lanelet)
@@ -720,15 +740,15 @@
                 lanelet.translate_rotate(np.array([x_start, y_start]), 0)
                 MapCreator.fit_to_successor(successor, lanelet)
         elif place_at_position:
             lanelet.translate_rotate(np.array([lanelet_start_pos_x, lanelet_start_pos_y]), 0)
             if not self.road_network_toolbox_ui.horizontal.isChecked():
                 if self.road_network_toolbox_ui.select_end_position.isChecked():
                     rotation_angle = math.degrees(
-                        math.asin((self.get_y_position_lanelet_end() - lanelet_start_pos_y) / lanelet_length))
+                            math.asin((self.get_y_position_lanelet_end() - lanelet_start_pos_y) / lanelet_length))
                     # convert rotation_angle to positive angle since translate_rotate function only expects positive
                     # angle
                     if self.get_x_position_lanelet_end() < lanelet_start_pos_x:
                         rotation_angle = 180 - rotation_angle
                     if rotation_angle < 0:
                         rotation_angle = 360 + rotation_angle
                 elif self.road_network_toolbox_ui.rotate.isChecked():
@@ -833,51 +853,54 @@
         lanelet_end_pos_y = self.get_y_position_lanelet_end(True)
 
         lanelet_width = self.get_float(self.road_network_toolbox_ui.selected_lanelet_width)
         line_marking_left = LineMarking(self.road_network_toolbox_ui.selected_line_marking_left.currentText())
         line_marking_right = LineMarking(self.road_network_toolbox_ui.selected_line_marking_right.currentText())
         num_vertices = int(self.road_network_toolbox_ui.selected_number_vertices.text())
         adjacent_left = int(
-                self.road_network_toolbox_ui.selected_adjacent_left.currentText()) if self.road_network_toolbox_ui.selected_adjacent_left.currentText() != "None" else None
+                self.road_network_toolbox_ui.selected_adjacent_left.currentText()) if \
+                self.road_network_toolbox_ui.selected_adjacent_left.currentText() != "None" else None
         adjacent_right = int(
-                self.road_network_toolbox_ui.selected_adjacent_right.currentText()) if self.road_network_toolbox_ui.selected_adjacent_right.currentText() != "None" else None
+                self.road_network_toolbox_ui.selected_adjacent_right.currentText()) if \
+                self.road_network_toolbox_ui.selected_adjacent_right.currentText() != "None" else None
         adjacent_left_same_direction = self.road_network_toolbox_ui.selected_adjacent_left_same_direction.isChecked()
         adjacent_right_same_direction = self.road_network_toolbox_ui.selected_adjacent_right_same_direction.isChecked()
         lanelet_type = {LaneletType(ty) for ty in self.road_network_toolbox_ui.selected_lanelet_type.get_checked_items()
                         if ty != "None"}
         user_one_way = {RoadUser(user) for user in
                         self.road_network_toolbox_ui.selected_road_user_oneway.get_checked_items() if user != "None"}
         user_bidirectional = {RoadUser(user) for user in
                               self.road_network_toolbox_ui.selected_road_user_bidirectional.get_checked_items() if
                               user != "None"}
 
         traffic_signs = {int(sign) for sign in
                          self.road_network_toolbox_ui.selected_lanelet_referenced_traffic_sign_ids.get_checked_items()}
         traffic_lights = {int(light) for light in
-                          self.road_network_toolbox_ui.selected_lanelet_referenced_traffic_light_ids.get_checked_items()}
+                          self.road_network_toolbox_ui.selected_lanelet_referenced_traffic_light_ids
+                          .get_checked_items()}
         if self.road_network_toolbox_ui.selected_stop_line_box.isChecked():
             if self.road_network_toolbox_ui.selected_stop_line_beginning.isChecked():
                 stop_line_at_end = False
                 stop_line_at_beginning = True
                 stop_line_marking = LineMarking(
-                    self.road_network_toolbox_ui.selected_line_marking_stop_line.currentText())
+                        self.road_network_toolbox_ui.selected_line_marking_stop_line.currentText())
                 stop_line = StopLine(np.array([0, 0]), np.array([0, 0]), stop_line_marking, set(), set())
             elif self.road_network_toolbox_ui.selected_stop_line_end.isChecked():
                 stop_line_at_end = True
                 stop_line_at_beginning = False
                 stop_line_marking = LineMarking(
-                    self.road_network_toolbox_ui.selected_line_marking_stop_line.currentText())
+                        self.road_network_toolbox_ui.selected_line_marking_stop_line.currentText())
                 stop_line = StopLine(np.array([0, 0]), np.array([0, 0]), stop_line_marking, set(), set())
             else:
                 stop_line_start_x = self.get_float(self.road_network_toolbox_ui.selected_stop_line_start_x)
                 stop_line_end_x = self.get_float(self.road_network_toolbox_ui.selected_stop_line_end_x)
                 stop_line_start_y = self.get_float(self.road_network_toolbox_ui.selected_stop_line_start_y)
                 stop_line_end_y = self.get_float(self.road_network_toolbox_ui.selected_stop_line_end_y)
                 stop_line_marking = LineMarking(
-                    self.road_network_toolbox_ui.selected_line_marking_stop_line.currentText())
+                        self.road_network_toolbox_ui.selected_line_marking_stop_line.currentText())
                 stop_line_at_end = False
                 stop_line_at_beginning = False
                 stop_line = StopLine(np.array([stop_line_start_x, stop_line_start_y]),
                                      np.array([stop_line_end_x, stop_line_end_y]), stop_line_marking, set(), set())
         else:
             stop_line_at_end = False
             stop_line_at_beginning = False
@@ -917,15 +940,16 @@
         if rotation_angle < 0:
             rotation_angle = 360 + rotation_angle
 
         initial_vertex = lanelet.center_vertices[0]
         lanelet.translate_rotate(np.array([0, 0]), np.deg2rad(rotation_angle))
         lanelet.translate_rotate(initial_vertex - lanelet.center_vertices[0], 0.0)
 
-        # rotation destroys position of stop line therefore save stop line position and afterwards set stop line position again to right value
+        # rotation destroys position of stop line therefore save stop line position and afterwards set stop line
+        # position again to right value
         if stop_line is not None and not stop_line_at_end and not stop_line_at_beginning:
             lanelet.stop_line.start = stop_line_start
             lanelet.stop_line.end = stop_line_end
 
         self.last_added_lanelet_id = lanelet_id
 
         self.current_scenario.add_objects(lanelet)
@@ -936,15 +960,15 @@
         """
         Calculates length of the lanelet.
 
         @param lanelet: Lanelet of which the length should be calculated.
         @return: length of lanelet
         """
         return str(
-            np.linalg.norm(lanelet.center_vertices[0] - lanelet.center_vertices[len(lanelet.center_vertices) - 1]))
+                np.linalg.norm(lanelet.center_vertices[0] - lanelet.center_vertices[len(lanelet.center_vertices) - 1]))
 
     def get_width(self, lanelet: Lanelet = None):
         """
         Calculates width of the lanelet.
 
         @param lanelet: Lanelet of which the width should be calculated.
         @return: width of lanelet
@@ -977,25 +1001,24 @@
             self.road_network_toolbox_ui.predecessors.set_checked_items([str(lanelet.lanelet_id)])
             self.initialize_predecessor_and_successor_fields()
         elif self.road_network_toolbox_ui.connect_to_successors_selection.isChecked():
             self.road_network_toolbox_ui.successors.setCurrentIndex(lanelet.lanelet_id)
             self.road_network_toolbox_ui.successors.set_checked_items([str(lanelet.lanelet_id)])
             self.initialize_predecessor_and_successor_fields()
 
-
         self.road_network_toolbox_ui.selected_lanelet_start_position_x.setText(
-            str(0.0 if lanelet.center_vertices[0][0] == 1.0e-16 else lanelet.center_vertices[0][0]))
+                str(0.0 if lanelet.center_vertices[0][0] == 1.0e-16 else lanelet.center_vertices[0][0]))
         self.road_network_toolbox_ui.selected_lanelet_start_position_y.setText(
-            str(0.0 if lanelet.center_vertices[0][1] == 1.0e-16 else lanelet.center_vertices[0][1]))
+                str(0.0 if lanelet.center_vertices[0][1] == 1.0e-16 else lanelet.center_vertices[0][1]))
         self.road_network_toolbox_ui.selected_lanelet_end_position_x.setText(
-            str(0.0 if lanelet.center_vertices[len(lanelet.center_vertices) - 1][0] == 1.0e-16 else
-                lanelet.center_vertices[len(lanelet.center_vertices) - 1][0]))
+                str(0.0 if lanelet.center_vertices[len(lanelet.center_vertices) - 1][0] == 1.0e-16 else
+                    lanelet.center_vertices[len(lanelet.center_vertices) - 1][0]))
         self.road_network_toolbox_ui.selected_lanelet_end_position_y.setText(
-            str(0.0 if lanelet.center_vertices[len(lanelet.center_vertices) - 1][1] == 1.0e-16 else
-                lanelet.center_vertices[len(lanelet.center_vertices) - 1][1]))
+                str(0.0 if lanelet.center_vertices[len(lanelet.center_vertices) - 1][1] == 1.0e-16 else
+                    lanelet.center_vertices[len(lanelet.center_vertices) - 1][1]))
         self.road_network_toolbox_ui.selected_lanelet_width.setText(self.get_width(lanelet))
         self.road_network_toolbox_ui.selected_lanelet_length.setText(self.get_length(lanelet))
 
         # curved lanelet attributes
         if not self.lanelet_is_straight(lanelet):
             self.road_network_toolbox_ui.selected_curved_checkbox.setChecked(True)
             self.road_network_toolbox_ui.selected_curved_checkbox.box.setMaximumSize(0, 0)
@@ -1008,15 +1031,15 @@
         self.road_network_toolbox_ui.selected_lanelet_radius.setText("10.0")
         self.road_network_toolbox_ui.selected_lanelet_angle.setText("90.0")
 
         self.road_network_toolbox_ui.selected_number_vertices.setText(str(len(lanelet.center_vertices)))
 
         self.road_network_toolbox_ui.selected_line_marking_left.setCurrentText(lanelet.line_marking_left_vertices.value)
         self.road_network_toolbox_ui.selected_line_marking_right.setCurrentText(
-            lanelet.line_marking_right_vertices.value)
+                lanelet.line_marking_right_vertices.value)
 
         self.road_network_toolbox_ui.selected_predecessors.set_checked_items([str(pre) for pre in lanelet.predecessor])
         self.road_network_toolbox_ui.selected_successors.set_checked_items([str(suc) for suc in lanelet.successor])
 
         self.road_network_toolbox_ui.selected_adjacent_left.setCurrentText(str(lanelet.adj_left))
         self.road_network_toolbox_ui.selected_adjacent_right.setCurrentText(str(lanelet.adj_right))
         self.road_network_toolbox_ui.selected_adjacent_left_same_direction.setChecked(
@@ -1052,15 +1075,15 @@
                 self.road_network_toolbox_ui.selected_stop_line_select_position.setChecked(True)
                 self.road_network_toolbox_ui.adjust_selected_stop_line_position()
                 self.road_network_toolbox_ui.selected_stop_line_start_x.setText(str(lanelet.stop_line.start[0]))
                 self.road_network_toolbox_ui.selected_stop_line_start_y.setText(str(lanelet.stop_line.start[1]))
                 self.road_network_toolbox_ui.selected_stop_line_end_x.setText(str(lanelet.stop_line.end[0]))
                 self.road_network_toolbox_ui.selected_stop_line_end_y.setText(str(lanelet.stop_line.end[1]))
             self.road_network_toolbox_ui.selected_line_marking_stop_line.setCurrentText(
-                str(lanelet.stop_line.line_marking.value))
+                    str(lanelet.stop_line.line_marking.value))
         else:
             self.road_network_toolbox_ui.selected_stop_line_box.setChecked(True)
             self.road_network_toolbox_ui.selected_stop_line_beginning.setChecked(True)
             self.road_network_toolbox_ui.adjust_selected_stop_line_position()
             self.road_network_toolbox_ui.selected_stop_line_box.setChecked(False)
 
     def create_adjacent(self):
@@ -1169,16 +1192,16 @@
         incoming_length = int(self.road_network_toolbox_ui.intersection_incoming_length.text())
         add_traffic_signs = self.road_network_toolbox_ui.intersection_with_traffic_signs.isChecked()
         add_traffic_lights = self.road_network_toolbox_ui.intersection_with_traffic_lights.isChecked()
         country_signs = globals()["TrafficSignID" + SupportedTrafficSignCountry(
                 self.current_scenario.scenario_id.country_id).name.capitalize()]
 
         intersection, new_traffic_signs, new_traffic_lights, new_lanelets = MapCreator.create_four_way_intersection(
-            width, diameter, incoming_length, self.current_scenario, add_traffic_signs, add_traffic_lights,
-            country_signs)
+                width, diameter, incoming_length, self.current_scenario, add_traffic_signs, add_traffic_lights,
+                country_signs)
         self.current_scenario.add_objects(intersection)
         self.current_scenario.add_objects(new_lanelets)
         self.current_scenario.add_objects(new_traffic_signs)
         self.current_scenario.add_objects(new_traffic_lights)
         self.set_default_road_network_list_information()
         self.callback(self.current_scenario)
 
@@ -1194,16 +1217,16 @@
         incoming_length = int(self.road_network_toolbox_ui.intersection_incoming_length.text())
         add_traffic_signs = self.road_network_toolbox_ui.intersection_with_traffic_signs.isChecked()
         add_traffic_lights = self.road_network_toolbox_ui.intersection_with_traffic_lights.isChecked()
         country_signs = globals()["TrafficSignID" + SupportedTrafficSignCountry(
                 self.current_scenario.scenario_id.country_id).name.capitalize()]
 
         intersection, new_traffic_signs, new_traffic_lights, new_lanelets = MapCreator.create_three_way_intersection(
-            width, diameter, incoming_length, self.current_scenario, add_traffic_signs, add_traffic_lights,
-            country_signs)
+                width, diameter, incoming_length, self.current_scenario, add_traffic_signs, add_traffic_lights,
+                country_signs)
 
         self.current_scenario.add_objects(intersection)
         self.current_scenario.add_objects(new_lanelets)
         self.current_scenario.add_objects(new_traffic_signs)
         self.current_scenario.add_objects(new_traffic_lights)
         self.set_default_road_network_list_information()
         self.callback(self.current_scenario)
@@ -1225,15 +1248,15 @@
         if self.current_scenario is None:
             self.text_browser.append("_Warning:_ Create a new file")
             return
         num_rows = self.road_network_toolbox_ui.traffic_sign_element_table.rowCount()
         self.road_network_toolbox_ui.traffic_sign_element_table.insertRow(num_rows)
         combo_box = QComboBox()
         combo_box.addItems([elem.name for elem in globals()["TrafficSignID" + SupportedTrafficSignCountry(
-            self.current_scenario.scenario_id.country_id).name.capitalize()]])
+                self.current_scenario.scenario_id.country_id).name.capitalize()]])
         self.road_network_toolbox_ui.traffic_sign_element_table.setCellWidget(num_rows, 0, combo_box)
 
     def remove_traffic_sign_element(self):
         """
         Removes last entry in traffic sign element table of a traffic sign.
         """
         num_rows = self.road_network_toolbox_ui.traffic_sign_element_table.rowCount()
@@ -1354,21 +1377,21 @@
             self.road_network_toolbox_ui.x_position_traffic_sign.setText(str(traffic_sign.position[0]))
             self.road_network_toolbox_ui.y_position_traffic_sign.setText(str(traffic_sign.position[1]))
             self.road_network_toolbox_ui.traffic_sign_element_table.setRowCount(0)
             for elem in traffic_sign.traffic_sign_elements:
                 self.add_traffic_sign_element()
                 num_rows = self.road_network_toolbox_ui.traffic_sign_element_table.rowCount()
                 self.road_network_toolbox_ui.traffic_sign_element_table.cellWidget(num_rows - 1, 0).setCurrentText(
-                    country_signs(elem.traffic_sign_element_id).name)
+                        country_signs(elem.traffic_sign_element_id).name)
                 if len(elem.additional_values) > 0:
-                    self.road_network_toolbox_ui.traffic_sign_element_table.setItem(
-                        num_rows - 1, 1, QTableWidgetItem(str(elem.additional_values[0])))
+                    self.road_network_toolbox_ui.traffic_sign_element_table.setItem(num_rows - 1, 1,
+                            QTableWidgetItem(str(elem.additional_values[0])))
                 else:
-                    self.road_network_toolbox_ui.traffic_sign_element_table.setItem(
-                        num_rows - 1, 1, QTableWidgetItem(""))
+                    self.road_network_toolbox_ui.traffic_sign_element_table.setItem(num_rows - 1, 1,
+                            QTableWidgetItem(""))
         else:
             self.road_network_toolbox_ui.traffic_sign_virtual_selection.setChecked(False)
             self.road_network_toolbox_ui.x_position_traffic_sign.setText("0.0")
             self.road_network_toolbox_ui.y_position_traffic_sign.setText("0.0")
             self.road_network_toolbox_ui.traffic_sign_element_table.setRowCount(0)
 
     def add_traffic_light(self, traffic_light_id: int = None):
@@ -1380,33 +1403,34 @@
         if self.current_scenario is None:
             self.text_browser.append("_Warning:_ Create a new file")
             return
         if len(self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()) == 0:
             self.text_browser.append("_Warning:_ Add Referenced Lanelets")
             return
         # Check if only 'None' is selected - if yes -> Warning
-        if 'None' in self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items() and len(self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()) == 1:
+        if 'None' in self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items() and len(
+                self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()) == 1:
             self.text_browser.append("_Warning:_ Add Referenced Lanelets")
             return
         # Check if 'None' is and other items are selected -> Uncheck 'None'
         elif 'None' in self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items():
             self.road_network_toolbox_ui.referenced_lanelets_traffic_light.uncheck_items('None')
-        referenced_lanelets = \
-            {int(la) for la in self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()}
+        referenced_lanelets = {int(la) for la in
+                               self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()}
         if self.road_network_toolbox_ui.x_position_traffic_light.text():
             x_position = self.get_float(self.road_network_toolbox_ui.x_position_traffic_light)
         else:
             x_position = 0
         if self.road_network_toolbox_ui.y_position_traffic_light.text():
             y_position = self.get_float(self.road_network_toolbox_ui.y_position_traffic_light)
         else:
             y_position = 0
 
-        traffic_light_direction = \
-            TrafficLightDirection(self.road_network_toolbox_ui.traffic_light_directions.currentText())
+        traffic_light_direction = TrafficLightDirection(
+            self.road_network_toolbox_ui.traffic_light_directions.currentText())
         time_offset = int(self.road_network_toolbox_ui.time_offset.text())
         time_red = int(self.road_network_toolbox_ui.time_red.text())
         time_green = int(self.road_network_toolbox_ui.time_green.text())
         time_yellow = int(self.road_network_toolbox_ui.time_yellow.text())
         time_red_yellow = int(self.road_network_toolbox_ui.time_red_yellow.text())
         time_inactive = int(self.road_network_toolbox_ui.time_inactive.text())
         traffic_light_active = self.road_network_toolbox_ui.traffic_light_active.isChecked()
@@ -1424,17 +1448,16 @@
                 traffic_light_cycle.append(TrafficLightCycleElement(TrafficLightState.YELLOW, time_yellow))
             elif elem == "in" and time_inactive > 0:
                 traffic_light_cycle.append(TrafficLightCycleElement(TrafficLightState.INACTIVE, time_inactive))
 
         if traffic_light_id is None:
             traffic_light_id = self.current_scenario.generate_object_id()
 
-        new_traffic_light = TrafficLight(traffic_light_id, traffic_light_cycle,
-                                         np.array([x_position, y_position]), time_offset, traffic_light_direction,
-                                         traffic_light_active)
+        new_traffic_light = TrafficLight(traffic_light_id, traffic_light_cycle, np.array([x_position, y_position]),
+                                         time_offset, traffic_light_direction, traffic_light_active)
 
         self.current_scenario.add_objects(new_traffic_light, referenced_lanelets)
         self.set_default_road_network_list_information()
         self.callback(self.current_scenario)
 
     def remove_traffic_light(self):
         """
@@ -1443,16 +1466,15 @@
         if self.current_scenario is None:
             self.text_browser.append("_Warning:_ Create a new file")
             return
         if self.road_network_toolbox_ui.selected_traffic_light.currentText() not in ["", "None"]:
             selected_traffic_light_id = int(self.road_network_toolbox_ui.selected_traffic_light.currentText())
         else:
             return
-        traffic_light = \
-            self.current_scenario.lanelet_network.find_traffic_light_by_id(selected_traffic_light_id)
+        traffic_light = self.current_scenario.lanelet_network.find_traffic_light_by_id(selected_traffic_light_id)
         self.current_scenario.remove_traffic_light(traffic_light)
         self.set_default_road_network_list_information()
         self.callback(self.current_scenario)
 
     def update_traffic_light(self):
         """
         Updates a traffic light from the scenario based on the user selection.
@@ -1460,38 +1482,37 @@
         if self.current_scenario is None:
             self.text_browser.append("_Warning:_ Create a new file")
             return
         if len(self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()) == 0:
             self.text_browser.append("_Warning:_ Add Referenced Lanelets")
             return
         # Check if only 'None' is selected - if yes -> Warning
-        if 'None' in self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items() and len(self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()) == 1:
+        if 'None' in self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items() and len(
+                self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()) == 1:
             self.text_browser.append("_Warning:_ Add Referenced Lanelets")
-            return # Check if 'None' is and other items are selected -> Uncheck 'None'
+            return  # Check if 'None' is and other items are selected -> Uncheck 'None'
         elif 'None' in self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items():
             self.road_network_toolbox_ui.referenced_lanelets_traffic_light.uncheck_items('None')
         if self.road_network_toolbox_ui.selected_traffic_light.currentText() not in ["", "None"]:
             selected_traffic_light_id = int(self.road_network_toolbox_ui.selected_traffic_light.currentText())
         else:
             return
-        traffic_light = \
-            self.current_scenario.lanelet_network.find_traffic_light_by_id(selected_traffic_light_id)
+        traffic_light = self.current_scenario.lanelet_network.find_traffic_light_by_id(selected_traffic_light_id)
         self.current_scenario.remove_traffic_light(traffic_light)
         self.add_traffic_light(selected_traffic_light_id)
         self.set_default_road_network_list_information()
         self.callback(self.current_scenario)
 
     def update_traffic_light_information(self):
         """
         Updates information of traffic light widget based on traffic light ID selected by the user.
         """
         if self.road_network_toolbox_ui.selected_traffic_light.currentText() not in ["", "None"]:
             selected_traffic_light_id = int(self.road_network_toolbox_ui.selected_traffic_light.currentText())
-            traffic_light = \
-                self.current_scenario.lanelet_network.find_traffic_light_by_id(selected_traffic_light_id)
+            traffic_light = self.current_scenario.lanelet_network.find_traffic_light_by_id(selected_traffic_light_id)
 
             self.road_network_toolbox_ui.x_position_traffic_light.setText(str(traffic_light.position[0]))
             self.road_network_toolbox_ui.y_position_traffic_light.setText(str(traffic_light.position[1]))
             self.road_network_toolbox_ui.time_offset.setText(str(traffic_light.time_offset))
             self.road_network_toolbox_ui.traffic_light_active.setChecked(True)
 
             cycle_order = ""
@@ -1512,55 +1533,52 @@
                     cycle_order += "in-"
                     self.road_network_toolbox_ui.time_inactive.setText(str(elem.duration))
             cycle_order = cycle_order[:-1]
             self.road_network_toolbox_ui.traffic_light_cycle_order.setCurrentText(cycle_order)
 
             self.road_network_toolbox_ui.traffic_light_directions.setCurrentText(str(traffic_light.direction.value))
 
-            referenced_lanelets = [str(la.lanelet_id) for la in
-                                   self.current_scenario.lanelet_network.lanelets
-                                   if selected_traffic_light_id in la.traffic_lights]
+            referenced_lanelets = [str(la.lanelet_id) for la in self.current_scenario.lanelet_network.lanelets if
+                                   selected_traffic_light_id in la.traffic_lights]
             self.road_network_toolbox_ui.referenced_lanelets_traffic_light.set_checked_items(referenced_lanelets)
 
     def create_traffic_lights(self):
         if not SUMO_AVAILABLE:
             self.text_browser.append("SUMO is not installed correctly!")
             return
         lanelet_ids = [int(lanelet_id) for lanelet_id in
                        self.road_network_toolbox_ui.referenced_lanelets_traffic_light.get_checked_items()]
         if not lanelet_ids:
             return
         self.road_network_toolbox_ui.referenced_lanelets_traffic_light.clear()
-        converter = CR2SumoMapConverter(self.current_scenario,
-                                        SumoConfig.from_scenario(self.current_scenario))
+        converter = CR2SumoMapConverter(self.current_scenario, SumoConfig.from_scenario(self.current_scenario))
         converter.create_sumo_files(self.tmp_folder)
         oks = []
         dt = self.current_scenario.dt
         offset = int(self.road_network_toolbox_ui.time_offset.text())
         red = int(self.road_network_toolbox_ui.time_red.text())
         red_yellow = int(self.road_network_toolbox_ui.time_red_yellow.text())
         green = int(self.road_network_toolbox_ui.time_green.text())
         yellow = int(self.road_network_toolbox_ui.time_yellow.text())
         total = red + red_yellow + green + yellow
 
         for lanelet_id in lanelet_ids:
             try:
-                ok = converter.auto_generate_traffic_light_system(lanelet_id,
-                                                                  green_time=int(green * dt),
-                                                                  yellow_time=int(yellow * dt),
-                                                                  all_red_time=0,
+                ok = converter.auto_generate_traffic_light_system(lanelet_id, green_time=int(green * dt),
+                                                                  yellow_time=int(yellow * dt), all_red_time=0,
                                                                   left_green_time=math.ceil(0.06 * total * dt),
                                                                   crossing_min_time=math.ceil(0.1 * total * dt),
                                                                   crossing_clearance_time=math.ceil(0.15 * total * dt),
                                                                   time_offset=int(offset * dt))
             except Exception:
                 ok = False
             oks.append(ok)
-            self.text_browser.append(
-                ("Created" if ok else "ERROR: Could not create") + f" traffic light system for lanelet {lanelet_id}")
+            self.text_browser.append((
+                                         "Created" if ok else "ERROR: Could not create") + f" traffic light system "
+                                                                                           f"for lanelet {lanelet_id}")
 
         if any(oks):
             # update lanelet_network and boradcast change
             self.current_scenario.replace_lanelet_network(converter.lanelet_network)
             self.callback(self.current_scenario)
 
     def add_incoming_to_table(self, new_incoming: bool = True, incoming_ids: List[str] = None):
@@ -1575,16 +1593,16 @@
             self.text_browser.append("_Warning:_ Create a new file")
             return
 
         num_rows = self.road_network_toolbox_ui.intersection_incomings_table.rowCount()
         self.road_network_toolbox_ui.intersection_incomings_table.insertRow(num_rows)
         lanelet_ids = [str(la_id) for la_id in self.collect_lanelet_ids()]
         if new_incoming:
-            self.road_network_toolbox_ui.intersection_incomings_table.setItem(
-                num_rows, 0, QTableWidgetItem(str(self.current_scenario.generate_object_id())))
+            self.road_network_toolbox_ui.intersection_incomings_table.setItem(num_rows, 0,
+                    QTableWidgetItem(str(self.current_scenario.generate_object_id())))
         combo_box_lanelets = CheckableComboBox()
         combo_box_lanelets.addItems(lanelet_ids)
         self.road_network_toolbox_ui.intersection_incomings_table.setCellWidget(num_rows, 1, combo_box_lanelets)
         combo_box_successors_left = CheckableComboBox()
         combo_box_successors_left.addItems(lanelet_ids)
         self.road_network_toolbox_ui.intersection_incomings_table.setCellWidget(num_rows, 2, combo_box_successors_left)
         combo_box_successors_straight = CheckableComboBox()
@@ -1599,23 +1617,23 @@
     def update_left_of_combobox(self, incoming_ids: List[str] = None):
         """
         Collects all incoming IDs in incoming table and updates left of combobox
 
         @param incoming_ids: List of available incoming IDs.
         """
         if incoming_ids is None:
-            incoming_ids = [self.road_network_toolbox_ui.intersection_incomings_table.item(row, 0).text()
-                            for row in range(self.road_network_toolbox_ui.intersection_incomings_table.rowCount())]
+            incoming_ids = [self.road_network_toolbox_ui.intersection_incomings_table.item(row, 0).text() for row in
+                            range(self.road_network_toolbox_ui.intersection_incomings_table.rowCount())]
         for row in range(self.road_network_toolbox_ui.intersection_incomings_table.rowCount()):
             combo_box_left_of = QComboBox()
             combo_box_left_of.addItems(incoming_ids)
             if row != self.road_network_toolbox_ui.intersection_incomings_table.rowCount() - 1:
                 index = self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row, 5).findText(
-                    self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row, 5).currentText(),
-                    Qt.MatchFixedString)
+                        self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row, 5).currentText(),
+                        Qt.MatchFixedString)
             else:
                 index = -1
             self.road_network_toolbox_ui.intersection_incomings_table.setCellWidget(row, 5, combo_box_left_of)
             if index >= 0:
                 self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row, 5).setCurrentIndex(index)
 
     def remove_intersection(self):
@@ -1624,32 +1642,30 @@
         """
         if self.current_scenario is None:
             self.text_browser.append("_Warning:_ Create a new file")
             return
 
         if self.road_network_toolbox_ui.selected_intersection.currentText() not in ["", "None"]:
             selected_intersection_id = int(self.road_network_toolbox_ui.selected_intersection.currentText())
-            intersection = \
-                self.current_scenario.lanelet_network.find_intersection_by_id(selected_intersection_id)
+            intersection = self.current_scenario.lanelet_network.find_intersection_by_id(selected_intersection_id)
             self.current_scenario.remove_intersection(intersection)
             self.set_default_road_network_list_information()
             self.callback(self.current_scenario)
 
     def update_intersection(self):
         """
         Updates a selected intersection from the scenario.
         """
         if self.current_scenario is None:
             self.text_browser.append("_Warning:_ Create a new file")
             return
 
         if self.road_network_toolbox_ui.selected_intersection.currentText() not in ["", "None"]:
             selected_intersection_id = int(self.road_network_toolbox_ui.selected_intersection.currentText())
-            intersection = \
-                self.current_scenario.lanelet_network.find_intersection_by_id(selected_intersection_id)
+            intersection = self.current_scenario.lanelet_network.find_intersection_by_id(selected_intersection_id)
             self.current_scenario.remove_intersection(intersection)
             self.add_intersection(selected_intersection_id)
             self.set_default_road_network_list_information()
             self.callback(self.current_scenario)
 
     def add_intersection(self, intersection_id: int = None):
         """
@@ -1660,38 +1676,39 @@
             return
 
         if intersection_id is None:
             intersection_id = self.current_scenario.generate_object_id()
         incomings = []
         for row in range(self.road_network_toolbox_ui.intersection_incomings_table.rowCount()):
             incoming_id = int(self.road_network_toolbox_ui.intersection_incomings_table.item(row, 0).text())
-            incoming_lanelets = \
-                {int(item) for item in
-                 self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row, 1).get_checked_items()}
+            incoming_lanelets = {int(item) for item in
+                                 self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row,
+                                                                                                      1).get_checked_items()}
             if len(incoming_lanelets) < 1:
                 self.text_browser.append("_Warning:_ An incoming must consist at least of one lanelet.")
                 print("road_network_toolbox.py/add_intersection: An incoming must consist at least of one lanelet.")
                 return
             successor_left = {int(item) for item in
-                              self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                row, 2).get_checked_items()}
+                              self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row,
+                                      2).get_checked_items()}
             successor_straight = {int(item) for item in
-                                  self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                                      row, 3).get_checked_items()}
+                                  self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row,
+                                          3).get_checked_items()}
             successor_right = {int(item) for item in
-                               self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                                       row, 4).get_checked_items()}
+                               self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row,
+                                       4).get_checked_items()}
             if len(successor_left) + len(successor_right) + len(successor_straight) < 1:
                 print("An incoming must consist at least of one successor")
                 return
-            left_of = int(self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row, 5).currentText()) \
-                if self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row, 5).currentText() != "" \
-                else None
-            incoming = IntersectionIncomingElement(incoming_id, incoming_lanelets, successor_right,
-                                                   successor_straight, successor_left, left_of)
+            left_of = int(self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(row,
+                                                                                               5).currentText()) if \
+                                                                                               self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
+                row, 5).currentText() != "" else None
+            incoming = IntersectionIncomingElement(incoming_id, incoming_lanelets, successor_right, successor_straight,
+                                                   successor_left, left_of)
             incomings.append(incoming)
         crossings = {int(item) for item in self.road_network_toolbox_ui.intersection_crossings.get_checked_items()}
 
         if len(incomings) > 1:
             intersection = Intersection(intersection_id, incomings, crossings)
             self.current_scenario.add_objects(intersection)
 
@@ -1711,53 +1728,52 @@
 
     def update_intersection_information(self):
         """
         Updates information of intersection widget based on intersection ID selected by the user.
         """
         if self.road_network_toolbox_ui.selected_intersection.currentText() not in ["", "None"]:
             selected_intersection_id = int(self.road_network_toolbox_ui.selected_intersection.currentText())
-            intersection = \
-                self.current_scenario.lanelet_network.find_intersection_by_id(selected_intersection_id)
+            intersection = self.current_scenario.lanelet_network.find_intersection_by_id(selected_intersection_id)
             self.road_network_toolbox_ui.intersection_incomings_table.setRowCount(0)
             incoming_ids = [str(inc.incoming_id) for inc in intersection.incomings]
             for incoming in intersection.incomings:
                 self.add_incoming_to_table(False, incoming_ids)
                 num_rows = self.road_network_toolbox_ui.intersection_incomings_table.rowCount()
-                self.road_network_toolbox_ui.intersection_incomings_table.setItem(
-                    num_rows - 1, 0, QTableWidgetItem(str(incoming.incoming_id)))
-                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                    num_rows - 1, 1).set_checked_items([str(la_id) for la_id in incoming.incoming_lanelets])
-                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                    num_rows - 1, 2).set_checked_items([str(la_id) for la_id in incoming.successors_left])
-                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                    num_rows - 1, 3).set_checked_items([str(la_id) for la_id in incoming.successors_straight])
-                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                    num_rows - 1, 4).set_checked_items([str(la_id) for la_id in incoming.successors_right])
-                index = self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                    num_rows - 1, 5).findText(str(incoming.left_of))
-                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(
-                    num_rows - 1, 5).setCurrentIndex(index)
+                self.road_network_toolbox_ui.intersection_incomings_table.setItem(num_rows - 1, 0,
+                        QTableWidgetItem(str(incoming.incoming_id)))
+                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(num_rows - 1, 1).set_checked_items(
+                        [str(la_id) for la_id in incoming.incoming_lanelets])
+                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(num_rows - 1, 2).set_checked_items(
+                        [str(la_id) for la_id in incoming.successors_left])
+                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(num_rows - 1, 3).set_checked_items(
+                        [str(la_id) for la_id in incoming.successors_straight])
+                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(num_rows - 1, 4).set_checked_items(
+                        [str(la_id) for la_id in incoming.successors_right])
+                index = self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(num_rows - 1, 5).findText(
+                    str(incoming.left_of))
+                self.road_network_toolbox_ui.intersection_incomings_table.cellWidget(num_rows - 1, 5).setCurrentIndex(
+                    index)
             self.road_network_toolbox_ui.intersection_crossings.set_checked_items(
-                [str(cr) for cr in intersection.crossings])
+                    [str(cr) for cr in intersection.crossings])
 
             self.road_network_toolbox_ui.intersection_lanelet_to_fit.clear()
             self.road_network_toolbox_ui.intersection_lanelet_to_fit.addItems(
-                ["None"] + [str(item) for item in self.collect_incoming_lanelet_ids_from_intersection()])
+                    ["None"] + [str(item) for item in self.collect_incoming_lanelet_ids_from_intersection()])
             self.road_network_toolbox_ui.intersection_lanelet_to_fit.setCurrentIndex(0)
 
     def connect_lanelets(self):
         """
         Connects two lanelets by adding a new lanelet using cubic spline interpolation.
         """
         selected_lanelet_one = self.selected_lanelet()
         if selected_lanelet_one is None:
             return
         if self.road_network_toolbox_ui.selected_lanelet_two.currentText() != "None":
             selected_lanelet_two = self.current_scenario.lanelet_network.find_lanelet_by_id(
-                int(self.road_network_toolbox_ui.selected_lanelet_two.currentText()))
+                    int(self.road_network_toolbox_ui.selected_lanelet_two.currentText()))
         else:
             self.text_browser.append("No lanelet selected for [2].")
             return
 
         connected_lanelet = MapCreator.connect_lanelets(selected_lanelet_one, selected_lanelet_two,
                                                         self.current_scenario.generate_object_id())
         self.last_added_lanelet_id = connected_lanelet.lanelet_id
@@ -1771,15 +1787,15 @@
         @return:
         """
         selected_lanelet_one = self.selected_lanelet()
         if selected_lanelet_one is None:
             return
         if self.road_network_toolbox_ui.selected_lanelet_two.currentText() != "None":
             selected_lanelet_two = self.current_scenario.lanelet_network.find_lanelet_by_id(
-                int(self.road_network_toolbox_ui.selected_lanelet_two.currentText()))
+                    int(self.road_network_toolbox_ui.selected_lanelet_two.currentText()))
         else:
             self.text_browser.append("No lanelet selected for [2].")
             return
 
         MapCreator.fit_to_predecessor(selected_lanelet_two, selected_lanelet_one)
         self.callback(self.current_scenario)
 
@@ -1832,17 +1848,18 @@
                 self.current_scenario.lanelet_network.find_lanelet_by_id(pred).add_successor(suc)
         self.callback(self.current_scenario)
 
     def fit_intersection(self):
         """
         Rotates and translates a complete intersection so that it is attached to a user-defined lanelet.
         """
-        if self.road_network_toolbox_ui.selected_intersection.currentText() not in ["", "None"] \
-            and self.road_network_toolbox_ui.other_lanelet_to_fit.currentText() not in ["", "None"] \
-                and self.road_network_toolbox_ui.intersection_lanelet_to_fit.currentText() not in ["", "None"]:
+        if self.road_network_toolbox_ui.selected_intersection.currentText() not in ["",
+                                                                                    "None"] and \
+                                                                                    self.road_network_toolbox_ui.other_lanelet_to_fit.currentText() not in [
+            "", "None"] and self.road_network_toolbox_ui.intersection_lanelet_to_fit.currentText() not in ["", "None"]:
             selected_intersection_id = int(self.road_network_toolbox_ui.selected_intersection.currentText())
             intersection = self.current_scenario.lanelet_network.find_intersection_by_id(selected_intersection_id)
 
             predecessor_id = int(self.road_network_toolbox_ui.other_lanelet_to_fit.currentText())
             lanelet_predecessor = self.current_scenario.lanelet_network.find_lanelet_by_id(predecessor_id)
 
             successor_id = int(self.road_network_toolbox_ui.intersection_lanelet_to_fit.currentText())
@@ -1852,74 +1869,86 @@
                                                        self.current_scenario.lanelet_network)
             self.callback(self.current_scenario)
 
     def show_aerial_image(self):
         if self.current_scenario is None:
             self.text_browser.append("Please create first a new scenario.")
             return
-        if float(self.road_network_toolbox_ui.northern_bound.text()) > 90 or float(self.road_network_toolbox_ui.northern_bound.text()) < -90:
+        if float(self.road_network_toolbox_ui.northern_bound.text()) > 90 or float(
+                self.road_network_toolbox_ui.northern_bound.text()) < -90:
             self.text_browser.append("Invalid northern bound. Latitude has to be between -90 and 90.")
             return
-        if float(self.road_network_toolbox_ui.southern_bound.text()) > 90 or float(self.road_network_toolbox_ui.southern_bound.text()) < -90:
+        if float(self.road_network_toolbox_ui.southern_bound.text()) > 90 or float(
+                self.road_network_toolbox_ui.southern_bound.text()) < -90:
             self.text_browser.append("Invalid southern bound. Latitude has to be between -90 and 90.")
             return
-        if float(self.road_network_toolbox_ui.western_bound.text()) > 180 or float(self.road_network_toolbox_ui.western_bound.text()) < -180:
+        if float(self.road_network_toolbox_ui.western_bound.text()) > 180 or float(
+                self.road_network_toolbox_ui.western_bound.text()) < -180:
             self.text_browser.append("Invalid western bound. Longitude has to be between -180 and 180.")
             return
-        if float(self.road_network_toolbox_ui.eastern_bound.text()) > 180 or float(self.road_network_toolbox_ui.eastern_bound.text()) < -180:
+        if float(self.road_network_toolbox_ui.eastern_bound.text()) > 180 or float(
+                self.road_network_toolbox_ui.eastern_bound.text()) < -180:
             self.text_browser.append("Invalid eastern bound. Longitude has to be between -180 and 180.")
             return
-        if float(self.road_network_toolbox_ui.southern_bound.text()) >= float(self.road_network_toolbox_ui.northern_bound.text()) \
-                or float(self.road_network_toolbox_ui.western_bound.text()) >= float(self.road_network_toolbox_ui.eastern_bound.text()):
+        if float(self.road_network_toolbox_ui.southern_bound.text()) >= float(
+                self.road_network_toolbox_ui.northern_bound.text()) or float(
+                self.road_network_toolbox_ui.western_bound.text()) >= float(
+                self.road_network_toolbox_ui.eastern_bound.text()):
             self.text_browser.append("Invalid coordinate limits.")
             return
 
         if self.road_network_toolbox_ui.bing_selection.isChecked():
             if config_settings.BING_MAPS_KEY == "":
                 print("_Warning__: No Bing Maps key specified. Go to settings and set password.")
                 warning_dialog = QMessageBox()
-                warning_dialog.warning(None, "Warning", "No Bing Maps key specified. Go to settings and set password.", QMessageBox.Ok,
-                                   QMessageBox.Ok)
+                warning_dialog.warning(None, "Warning", "No Bing Maps key specified. Go to settings and set password.",
+                                       QMessageBox.Ok, QMessageBox.Ok)
                 warning_dialog.close()
                 return
         elif self.road_network_toolbox_ui.ldbv_selection.isChecked():
             if config_settings.LDBV_USERNAME == "" or config_settings.LDBV_PASSWORD == "":
                 print("_Warning__: LDBV username and password not specified. Go to settings and set them.")
                 warning_dialog = QMessageBox()
-                warning_dialog.warning(None, "Warning", "LDBV username and password not specified. Go to settings and set them.",
+                warning_dialog.warning(None, "Warning",
+                                       "LDBV username and password not specified. Go to settings and set them.",
                                        QMessageBox.Ok, QMessageBox.Ok)
                 warning_dialog.close()
                 return
-            if float(self.road_network_toolbox_ui.southern_bound.text()) > 50.6 or float(self.road_network_toolbox_ui.southern_bound.text()) < 47.2 \
-                    or float(self.road_network_toolbox_ui.northern_bound.text()) > 50.6 or float(self.road_network_toolbox_ui.northern_bound.text()) < 47.2 \
-                    or float(self.road_network_toolbox_ui.western_bound.text()) > 13.9 or float(self.road_network_toolbox_ui.western_bound.text()) < 8.9 \
-                    or float(self.road_network_toolbox_ui.eastern_bound.text()) > 13.9 or float(self.road_network_toolbox_ui.eastern_bound.text()) < 8.9:
-                self.text_browser.append("Coordinates are outside Bavaria. This tool works only for coordinates inside Bavaria.")
+            if float(self.road_network_toolbox_ui.southern_bound.text()) > 50.6 or float(
+                    self.road_network_toolbox_ui.southern_bound.text()) < 47.2 or float(
+                    self.road_network_toolbox_ui.northern_bound.text()) > 50.6 or float(
+                    self.road_network_toolbox_ui.northern_bound.text()) < 47.2 or float(
+                    self.road_network_toolbox_ui.western_bound.text()) > 13.9 or float(
+                    self.road_network_toolbox_ui.western_bound.text()) < 8.9 or float(
+                    self.road_network_toolbox_ui.eastern_bound.text()) > 13.9 or float(
+                    self.road_network_toolbox_ui.eastern_bound.text()) < 8.9:
+                self.text_browser.append(
+                    "Coordinates are outside Bavaria. This tool works only for coordinates inside Bavaria.")
                 return
 
         self.startSpinner(self.road_network_toolbox_ui.Spinner)
         runnable = RequestRunnable(self.activate_aerial_image, self)
         QThreadPool.globalInstance().start(runnable)
 
-
     def activate_aerial_image(self):
-        self.mwindow.animated_viewer_wrapper.cr_viewer.dynamic.activate_aerial_image(self.road_network_toolbox_ui.bing_selection.isChecked(),
-                                                                                 float(self.road_network_toolbox_ui.northern_bound.text()),
-                                                                                 float(self.road_network_toolbox_ui.western_bound.text()),
-                                                                                 float(self.road_network_toolbox_ui.southern_bound.text()),
-                                                                                 float(self.road_network_toolbox_ui.eastern_bound.text()),
-                                                                                     self.road_network_toolbox_ui.center_at_zero.isChecked())
+        self.mwindow.animated_viewer_wrapper.cr_viewer.dynamic.activate_aerial_image(
+            self.road_network_toolbox_ui.bing_selection.isChecked(),
+            float(self.road_network_toolbox_ui.northern_bound.text()),
+            float(self.road_network_toolbox_ui.western_bound.text()),
+            float(self.road_network_toolbox_ui.southern_bound.text()),
+            float(self.road_network_toolbox_ui.eastern_bound.text()))
         self.mwindow.animated_viewer_wrapper.cr_viewer.dynamic.show_aerial_image()
+
     def remove_aerial_image(self):
         self.mwindow.animated_viewer_wrapper.cr_viewer.dynamic.deactivate_aerial_image()
         self.callback(self.current_scenario)
 
     @pyqtSlot(str)
     def stopSpinner(self, data):
         print(data)
         self.callback(self.current_scenario)
         self.road_network_toolbox_ui.Spinner.stop()
 
     def startSpinner(self, spinner: QtWaitingSpinner):
         if (spinner.isSpinning()):
             spinner.stop()
-        spinner.start()
+        spinner.start()
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/road_network_toolbox/road_network_toolbox_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,18 +108,14 @@
 
         # probably move the next 4 lines to init_aerial_widget or something
         self.northern_bound.setText("48.263864")
         self.western_bound.setText("11.655410")
         self.southern_bound.setText("48.261424")
         self.eastern_bound.setText("11.660930")
 
-        self.center_at_zero = QCheckBox("Center at origin")
-        self.center_at_zero.setChecked(True)
-        self.layout_aerial_image_groupbox.addRow(self.center_at_zero)
-
         self.Spinner = QtWaitingSpinner(self, centerOnParent=True)
         self.Spinner.setInnerRadius(7)
         self.Spinner.setNumberOfLines(10)
         self.Spinner.setLineLength(7)
         self.Spinner.setLineWidth(2)
 
         self.layout_aerial_image_groupbox.addRow(self.button_add_aerial_image)
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/toolboxes/toolbox_ui.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/toolboxes/toolbox_ui.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/menu_bar_wrapper.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/menu_bar_wrapper/menu_bar_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/file_actions.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/file_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
     mwindow.filename = filename
     if SUMO_AVAILABLE:
         mwindow.animated_viewer_wrapper.cr_viewer.open_scenario(new_scenario,
                                                                 mwindow.obstacle_toolbox.sumo_simulation.config,
                                                                 planning_problem_set=pps, new_file_added=True)
         mwindow.obstacle_toolbox.sumo_simulation.scenario = mwindow.animated_viewer_wrapper.cr_viewer.current_scenario
     else:
-        mwindow.animated_viewer_wrapper.cr_viewer.open_scenario(new_scenario, planning_problem_set=pps, new_file_added=True)
-    mwindow.animated_viewer_wrapper.update_view(new_file_added=True)
+        mwindow.animated_viewer_wrapper.cr_viewer.open_scenario(new_scenario, planning_problem_set=pps,
+                                                                new_file_added=True)
     mwindow.store_scenario()
     mwindow.update_toolbox_scenarios()
     update_to_new_scenario(mwindow)
 
 
 def update_to_new_scenario(mwindow):
     """"""
```

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/general_services.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/general_services.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/setting_actions.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/service_layer/setting_actions.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/toolbar_wrapper.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/toolbar_wrapper/toolbar_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/crdesigner/ui/gui/mwindow/top_bar_wrapper/top_bar_wrapper.py` & `commonroad_scenario_designer-0.7.1/crdesigner/ui/gui/mwindow/top_bar_wrapper/top_bar_wrapper.py`

 * *Files identical despite different names*

### Comparing `commonroad_scenario_designer-0.7.0/pyproject.toml` & `commonroad_scenario_designer-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "commonroad-scenario-designer"
-version = "0.7.0"
+version = "0.7.1"
 description = "Toolbox for Map Conversion and Scenario Creation for Autonomous Vehicles"
 authors = ["Cyber-Physical Systems Group, Technical University of Munich <commonroad@lists.lrz.de>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 keywords= ["autonomous", "automated", "vehicles", "driving", "motion", "planning", "simulation", "map", "scenario"]
 classifiers = [
     "Programming Language :: Python :: 3.8",
@@ -23,29 +23,30 @@
 Documentation = "https://commonroad-scenario-designer.readthedocs.io/en/latest/"
 Forum = "https://commonroad.in.tum.de/forum/c/scenario-designer/"
 Source = "https://gitlab.lrz.de/tum-cps/commonroad-scenario-designer"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 commonroad-io = "2023.1"
-pyqt5 = ">=5.12.2"
-matplotlib = ">=3.5,<3.6"
+pyqt5 = ">=5.15.9"
+matplotlib = ">=3.6.0"
 numpy = "^1.24.2"
 lxml = "^4.9.2"
 pyproj = "^3.4.1"
 utm = "^0.7.0"
 shapely = ">=2.0.1"
 ordered-set = "^4.1.0"
 sumocr = "2023.1"
 iso3166 = "^2.1.1"
 networkx = "^3.0"
 omegaconf = "^2.3.0"
 pyyaml = "6.0"
 pygeodesy = "^23.3.23"
 mercantile = "^1.2.1"
+urllib3 = "^2.0.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 ipython = "^8.11.0"
 sphinx = ">=2.2.1"
```

### Comparing `commonroad_scenario_designer-0.7.0/PKG-INFO` & `commonroad_scenario_designer-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-scenario-designer
-Version: 0.7.0
+Version: 0.7.1
 Summary: Toolbox for Map Conversion and Scenario Creation for Autonomous Vehicles
 Home-page: https://commonroad.in.tum.de
 License: GPL-3.0-or-later
 Keywords: autonomous,automated,vehicles,driving,motion,planning,simulation,map,scenario
 Author: Cyber-Physical Systems Group, Technical University of Munich
 Author-email: commonroad@lists.lrz.de
 Requires-Python: >=3.8,<4.0
@@ -13,33 +13,30 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: commonroad-io (==2023.1)
 Requires-Dist: iso3166 (>=2.1.1,<3.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: matplotlib (>=3.5,<3.6)
+Requires-Dist: matplotlib (>=3.6.0)
 Requires-Dist: mercantile (>=1.2.1,<2.0.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: pygeodesy (>=23.3.23,<24.0.0)
 Requires-Dist: pyproj (>=3.4.1,<4.0.0)
-Requires-Dist: pyqt5 (>=5.12.2)
+Requires-Dist: pyqt5 (>=5.15.9)
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: shapely (>=2.0.1)
 Requires-Dist: sumocr (==2023.1)
+Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Requires-Dist: utm (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://commonroad-scenario-designer.readthedocs.io/en/latest/
 Project-URL: Forum, https://commonroad.in.tum.de/forum/c/scenario-designer/
 Project-URL: Source, https://gitlab.lrz.de/tum-cps/commonroad-scenario-designer
 Description-Content-Type: text/markdown
 
 # CommonRoad Scenario Designer
@@ -47,15 +44,14 @@
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)  
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)  
 [![PyPI version fury.io](https://badge.fury.io/py/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)
 [![PyPI download week](https://img.shields.io/pypi/dw/commonroad-scenario-designer.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-scenario-designer/) 
 [![PyPI download month](https://img.shields.io/pypi/dm/commonroad-scenario-designer.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-scenario-designer/)  
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-scenario-designer.svg)](https://pypi.python.org/pypi/commonroad-scenario-designer/)
-[![Documentation Status](https://readthedocs.org/projects/commonroad-scenario-designer/badge/?version=latest)](http://commonroad-scenario-designer.readthedocs.io/?badge=latest) 
 
 This toolbox provides map converters for [OpenStreetMap](https://www.openstreetmap.de/karte.html) (OSM), 
 [Lanelet](https://www.mrt.kit.edu/software/libLanelet/libLanelet.html) / [Lanelet2](https://github.com/fzi-forschungszentrum-informatik/Lanelet2), 
 [OpenDRIVE](https://www.asam.net/standards/detail/opendrive/), and [SUMO](https://sumo.dlr.de/docs/index.html) to the [CommonRoad](https://commonroad.in.tum.de/) 
 (CR) format and for some formats vice versa.  
 Additionally, a graphical user interface (GUI) is included, which allows one to efficiently create and manipulate 
 CommonRoad maps and scenarios.
@@ -183,15 +179,15 @@
 The titles of module pages have to be set manually!  
 The full documentation of the API and introducing examples can also be found [here](https://commonroad-scenario-designer.readthedocs.io/en/latest/).
 
 ## Changelog
 A detailed overview about the changes in each version is provided in the [Changelog](https://gitlab.lrz.de/tum-cps/commonroad-scenario-designer/-/blob/main/CHANGELOG.md).
 
 ## Bug and feature reporting
-This release (v0.7.0) is still a BETA version.  
+This release (v0.7.1) is still a BETA version.  
 In case you detect a bug or you want to suggest a new feature, please report it in our [forum](https://commonroad.in.tum.de/forum/c/scenario-designer/18).   
 If you want to contribute to the toolbox, you can also post it in the [forum](https://commonroad.in.tum.de/forum/c/scenario-designer/18) or contact [Sebastian Maierhofer](sebastian.maierhofer@tum.de).
 
 ## Authors
 
 Responsible: Sebastian Maierhofer, Sebastian Mair
 Contribution (in alphabetic order by last name): Daniel Asch, Hamza Begic, Florian Braunmiller, Tim Dang,
```

