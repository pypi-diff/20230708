# Comparing `tmp/aiovantage-0.5.0.tar.gz` & `tmp/aiovantage-0.6.0.tar.gz`

## Comparing `aiovantage-0.5.0.tar` & `aiovantage-0.6.0.tar`

### file list

```diff
@@ -1,156 +1,157 @@
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.pylintrc
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aiovantage-0.5.0/TODO
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 aiovantage-0.5.0/test.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.vscode/settings.json
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/dump_system.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/monitor_all.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/anemo_sensors/dump_anemo_sensors.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/anemo_sensors/monitor_anemo_sensors.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/areas/dump_areas.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/blind_groups/dump_blind_groups.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/blinds/dump_blinds.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/blinds/monitor_blinds.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/buttons/dump_buttons.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/buttons/monitor_buttons.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/command_client/event_log.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/command_client/status_load.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/config_client/dump_objects.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/config_client/get_version.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/dry_contacts/dump_dry_contacts.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/dry_contacts/monitor_dry_contacts.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/gmem/dump_gmem.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/gmem/monitor_gmem.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/gmem/set_gmem.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/light_sensors/dump_light_sensors.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/light_sensors/monitor_light_sensors.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/load_groups/dump_load_groups.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/control_load.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/dump_loads.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/monitor_loads.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/poll_on_loads.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/loads/toggle_load.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/omni_sensors/dump_omni_sensors.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/omni_sensors/monitor_omni_sensors.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/rgb_loads/dump_rgb_loads.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/rgb_loads/monitor_rgb_loads.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/stations/dump_stations.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/stations/jingle_bells.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/tasks/dump_tasks.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/tasks/run_task.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/temperature_sensors/dump_temperature_sensors.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.5.0/examples/temperature_sensors/monitor_temperature_sensors.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/__about__.py
--rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/connection.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/discovery.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/errors.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/events.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/py.typed
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/query.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/__init__.py
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/commands.py
--rw-r--r--   0        0        0    14769 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/events.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/utils.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/__init__.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/base.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/blind.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/button.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/color_temperature.py
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/gmem.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/introspection.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/light_sensor.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/load.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/object.py
--rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/rgb_load.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/sensor.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/sounder.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/task.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/command_client/interfaces/temperature.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/README.md
--rw-r--r--   0        0        0     7178 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/__init__.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/helpers.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/xml_dataclass.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/types.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/close_filter.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/get_object.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/open_filter.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/introspection/__init__.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/introspection/get_version.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/login/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/methods/login/login.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/__init__.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/anemo_sensor.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/area.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/blind.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/blind_group.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/button.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dc_power_profile.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/ddg_color_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dg_color_load.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dimmer.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dry_contact.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/dual_relay_station.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/eq_ctrl.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/eq_ux.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/gmem.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/keypad.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/light_sensor.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/load.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/load_group.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/location_object.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/master.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/module.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/module_gen2.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/omni_sensor.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/power_profile.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/pwm_power_profile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/qis_blind.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/qube_blind.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/relay_blind.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/rgb_load.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/scene_point_relay.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/sensor.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/station_bus.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/station_object.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/system_object.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/task.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/temperature.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/anemo_sensors.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/areas.py
--rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/base.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/blind_groups.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/blinds.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/buttons.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/dry_contacts.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/gmem.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/light_sensors.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/load_groups.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/loads.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/masters.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/modules.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/omni_sensors.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/rgb_loads.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/stations.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/tasks.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 aiovantage-0.5.0/src/aiovantage/controllers/temperature_sensors.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.5.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.5.0/LICENSE
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aiovantage-0.5.0/README.md
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 aiovantage-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 aiovantage-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.pylintrc
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 aiovantage-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 aiovantage-0.6.0/TODO
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/dump_system.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/monitor_all.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/anemo_sensors/dump_anemo_sensors.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/anemo_sensors/monitor_anemo_sensors.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/areas/dump_areas.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/blind_groups/dump_blind_groups.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/blinds/dump_blinds.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/blinds/monitor_blinds.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/buttons/dump_buttons.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/buttons/monitor_buttons.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/command_client/event_log.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/command_client/status_load.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/config_client/dump_objects.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/config_client/get_version.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/dry_contacts/dump_dry_contacts.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/dry_contacts/monitor_dry_contacts.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/gmem/dump_gmem.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/gmem/monitor_gmem.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/gmem/set_gmem.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/light_sensors/dump_light_sensors.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/light_sensors/monitor_light_sensors.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/load_groups/dump_load_groups.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/control_load.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/dump_loads.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/monitor_loads.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/poll_on_loads.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/loads/toggle_load.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/masters/dump_masters.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/masters/monitor_masters.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/omni_sensors/dump_omni_sensors.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/omni_sensors/monitor_omni_sensors.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/rgb_loads/dump_rgb_loads.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/rgb_loads/monitor_rgb_loads.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/stations/dump_stations.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/stations/jingle_bells.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/tasks/dump_tasks.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/tasks/run_task.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/temperature_sensors/dump_temperature_sensors.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aiovantage-0.6.0/examples/temperature_sensors/monitor_temperature_sensors.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/__about__.py
+-rw-r--r--   0        0        0     9851 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/connection.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/discovery.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/errors.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/events.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/py.typed
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/query.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/README.md
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/__init__.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/commands.py
+-rw-r--r--   0        0        0    15120 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/events.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/utils.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/__init__.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/anemo_sensor.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/base.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/blind.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/button.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/color_temperature.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/gmem.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/introspection.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/light_sensor.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/load.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/object.py
+-rw-r--r--   0        0        0     9652 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/rgb_load.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/sensor.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/sounder.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/task.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/command_client/interfaces/temperature.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/README.md
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/__init__.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/helpers.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/xml_dataclass.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/types.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/close_filter.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/get_object.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/open_filter.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/introspection/__init__.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/introspection/get_version.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/login/__init__.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/methods/login/login.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/anemo_sensor.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/area.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/blind.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/blind_group.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/button.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dc_power_profile.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/ddg_color_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dg_color_load.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dimmer.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dry_contact.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/dual_relay_station.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/eq_ctrl.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/eq_ux.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/gmem.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/keypad.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/light_sensor.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/load.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/load_group.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/location_object.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/master.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/module.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/module_gen2.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/omni_sensor.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/power_profile.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/pwm_power_profile.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/qis_blind.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/qube_blind.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/relay_blind.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/rgb_load.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/scene_point_relay.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/sensor.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/station_bus.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/station_object.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/system_object.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/task.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/temperature.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/somfy/rs485_group.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/somfy/rs485_shade.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/somfy/urtsi_2_group.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/config_client/objects/somfy/urtsi_2_shade.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/anemo_sensors.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/areas.py
+-rw-r--r--   0        0        0    12719 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/base.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/blind_groups.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/blinds.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/buttons.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/dry_contacts.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/gmem.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/light_sensors.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/load_groups.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/loads.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/masters.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/modules.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/omni_sensors.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/rgb_loads.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/stations.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/tasks.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 aiovantage-0.6.0/src/aiovantage/controllers/temperature_sensors.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aiovantage-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aiovantage-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aiovantage-0.6.0/README.md
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 aiovantage-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 aiovantage-0.6.0/PKG-INFO
```

### Comparing `aiovantage-0.5.0/.pre-commit-config.yaml` & `aiovantage-0.6.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 repos:
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.275
+    rev: v0.0.276
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: "v1.4.1"
     hooks:
```

### Comparing `aiovantage-0.5.0/CONTRIBUTING.md` & `aiovantage-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/.github/ISSUE_TEMPLATE/bug.yml` & `aiovantage-0.6.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `aiovantage-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/dump_system.py` & `aiovantage-0.6.0/examples/dump_system.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/monitor_all.py` & `aiovantage-0.6.0/examples/monitor_all.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/anemo_sensors/dump_anemo_sensors.py` & `aiovantage-0.6.0/examples/anemo_sensors/dump_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/anemo_sensors/monitor_anemo_sensors.py` & `aiovantage-0.6.0/examples/anemo_sensors/monitor_anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/areas/dump_areas.py` & `aiovantage-0.6.0/examples/areas/dump_areas.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/blind_groups/dump_blind_groups.py` & `aiovantage-0.6.0/examples/blind_groups/dump_blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/blinds/dump_blinds.py` & `aiovantage-0.6.0/examples/blinds/dump_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/blinds/monitor_blinds.py` & `aiovantage-0.6.0/examples/blinds/monitor_blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/buttons/dump_buttons.py` & `aiovantage-0.6.0/examples/buttons/dump_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/buttons/monitor_buttons.py` & `aiovantage-0.6.0/examples/buttons/monitor_buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/command_client/event_log.py` & `aiovantage-0.6.0/examples/command_client/event_log.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/command_client/status_load.py` & `aiovantage-0.6.0/examples/command_client/status_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/config_client/dump_objects.py` & `aiovantage-0.6.0/examples/config_client/dump_objects.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/config_client/get_version.py` & `aiovantage-0.6.0/examples/config_client/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/dry_contacts/dump_dry_contacts.py` & `aiovantage-0.6.0/examples/dry_contacts/dump_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/dry_contacts/monitor_dry_contacts.py` & `aiovantage-0.6.0/examples/dry_contacts/monitor_dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/gmem/dump_gmem.py` & `aiovantage-0.6.0/examples/gmem/dump_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/gmem/monitor_gmem.py` & `aiovantage-0.6.0/examples/gmem/monitor_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/gmem/set_gmem.py` & `aiovantage-0.6.0/examples/gmem/set_gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/light_sensors/dump_light_sensors.py` & `aiovantage-0.6.0/examples/light_sensors/dump_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/light_sensors/monitor_light_sensors.py` & `aiovantage-0.6.0/examples/light_sensors/monitor_light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/load_groups/dump_load_groups.py` & `aiovantage-0.6.0/examples/load_groups/dump_load_groups.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,13 +21,14 @@
     if args.debug:
         logging.basicConfig(level=logging.DEBUG)
 
     # Connect to the Vantage controller
     async with Vantage(args.host, args.username, args.password) as vantage:
         # Print out the id, name, and members of each load group
         async for load_group in vantage.load_groups:
-            print(load_group)
-            print(f"[{load_group.id}] '{load_group.name}' {load_group.load_ids}")
+            print(
+                f"[{load_group.id}] '{load_group.name}' loads={load_group.load_ids} level={load_group.level}%"
+            )
 
 
 with contextlib.suppress(KeyboardInterrupt):
     asyncio.run(main())
```

### Comparing `aiovantage-0.5.0/examples/loads/control_load.py` & `aiovantage-0.6.0/examples/loads/control_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/loads/dump_loads.py` & `aiovantage-0.6.0/examples/loads/dump_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/loads/monitor_loads.py` & `aiovantage-0.6.0/examples/loads/monitor_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/loads/poll_on_loads.py` & `aiovantage-0.6.0/examples/loads/poll_on_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/loads/toggle_load.py` & `aiovantage-0.6.0/examples/loads/toggle_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/omni_sensors/dump_omni_sensors.py` & `aiovantage-0.6.0/examples/omni_sensors/dump_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/omni_sensors/monitor_omni_sensors.py` & `aiovantage-0.6.0/examples/omni_sensors/monitor_omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/rgb_loads/dump_rgb_loads.py` & `aiovantage-0.6.0/examples/rgb_loads/dump_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/rgb_loads/monitor_rgb_loads.py` & `aiovantage-0.6.0/examples/rgb_loads/monitor_rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/stations/dump_stations.py` & `aiovantage-0.6.0/examples/stations/dump_stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/stations/jingle_bells.py` & `aiovantage-0.6.0/examples/stations/jingle_bells.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/tasks/dump_tasks.py` & `aiovantage-0.6.0/examples/tasks/dump_tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/tasks/run_task.py` & `aiovantage-0.6.0/examples/tasks/run_task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/temperature_sensors/dump_temperature_sensors.py` & `aiovantage-0.6.0/examples/temperature_sensors/dump_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/examples/temperature_sensors/monitor_temperature_sensors.py` & `aiovantage-0.6.0/examples/temperature_sensors/monitor_temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/__init__.py` & `aiovantage-0.6.0/src/aiovantage/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/connection.py` & `aiovantage-0.6.0/src/aiovantage/connection.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/errors.py` & `aiovantage-0.6.0/src/aiovantage/errors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/query.py` & `aiovantage-0.6.0/src/aiovantage/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,7 +137,16 @@
     async def aget(self, **kwargs: Any) -> Optional[T]:
         ...
 
     async def aget(self, *args: Any, **kwargs: Any) -> Optional[T]:
         """Asynchronously get the first object that matches the given filter."""
         await self.__populate()
         return self.get(*args, **kwargs)
+
+    def first(self) -> Optional[T]:
+        """Return the first object in the queryset."""
+        return next(iter(self), None)
+
+    async def afirst(self) -> Optional[T]:
+        """Asynchronously return the first object in the queryset."""
+        await self.__populate()
+        return self.first()
```

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/README.md` & `aiovantage-0.6.0/src/aiovantage/command_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/__init__.py` & `aiovantage-0.6.0/src/aiovantage/command_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/commands.py` & `aiovantage-0.6.0/src/aiovantage/command_client/commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,38 +21,42 @@
 
     default_port = 3001
     default_ssl_port = 3010
 
 
 @dataclass
 class CommandResponse:
-    """Wrapper for command responses from the Vantage Host Command service."""
+    """Wrapper for command responses."""
 
     command: str
-    """The command that was sent."""
-
     args: List[str]
-    """The arguments of the "R:" line of the response."""
-
     data: List[str]
-    """The data lines of the response, before the "R:" line."""
 
     def __init__(self, data: List[str]) -> None:
         """Initialize a CommandResponse."""
-        # Extract "data" lines from the response. These are any lines before the
-        # "R:" line, from commands such as "HELP" and "LISTSTATUS".
         self.data, return_line = data[:-1], data[-1]
-
-        # Split the "R:" line into the command and arguments
         command, *self.args = tokenize_response(return_line)
-
-        # Remove the "R:" prefix from the command
         self.command = command[2:]
 
 
+@dataclass
+class InvokeResponse:
+    """Wrapper for invoke command responses."""
+
+    vid: int
+    result: str
+    method: str
+    args: List[str]
+
+    def __init__(self, data: List[str]) -> None:
+        """Initialize an InvokeResponse."""
+        _, vid_str, self.result, self.method, *self.args = tokenize_response(data[0])
+        self.vid = int(vid_str)
+
+
 class CommandClient:
     """Client to send commands to the Vantage Host Command service."""
 
     def __init__(
         self,
         host: str,
         username: Optional[str] = None,
@@ -96,41 +100,84 @@
         command: str,
         *params: Union[str, int, float, Decimal],
         force_quotes: bool = False,
         connection: Optional[CommandConnection] = None,
     ) -> CommandResponse:
         """Send a command to the Host Command service and wait for a response.
 
-        Handles encoding the parameters correctly, and raises an exception if the
-        response line is R:ERROR.
-
         Args:
             command: The command to send, should be a single word string.
             params: The parameters to send with the command.
             force_quotes: Whether to force string params to be wrapped in double quotes.
             connection: The connection to use, if not the default.
 
         Returns:
             A CommandResponse instance.
         """
-        # Get a connection to the Host Command service
-        conn = connection or await self.get_connection()
-
-        # Build the request string, encoding the parameters if necessary
         if params:
             request = f"{command} {encode_params(*params, force_quotes=force_quotes)}"
         else:
             request = command
 
+        # Send the request and parse the response
+        raw_response = await self.raw_request(request, connection=connection)
+        return CommandResponse(raw_response)
+
+    async def invoke(
+        self,
+        vid: int,
+        method: str,
+        *params: Union[str, int, float, Decimal],
+        force_quotes: bool = False,
+        connection: Optional[CommandConnection] = None,
+    ) -> InvokeResponse:
+        """Invoke a method on an object, and wait for a response.
+
+        Args:
+            vid: The VID of the object to invoke the command on.
+            method: The method to invoke.
+            params: The parameters to send with the method.
+            force_quotes: Whether to force string params to be wrapped in double quotes.
+            connection: The connection to use, if not the default.
+
+        Returns:
+            A InvokeResponse instance.
+        """
+        if params:
+            request = f"INVOKE {vid} {method} {encode_params(*params, force_quotes=force_quotes)}"
+        else:
+            request = f"INVOKE {vid} {method}"
+
+        # Send the request and parse the response
+        raw_response = await self.raw_request(request, connection=connection)
+        return InvokeResponse(raw_response)
+
+    async def raw_request(
+        self, request: str, connection: Optional[CommandConnection] = None
+    ) -> List[str]:
+        """Send a raw command to the Host Command service and return all response lines.
+
+        Handles authentication if required, and raises an exception if the response line
+        contains R:ERROR.
+
+        Args:
+            request: The request to send.
+            connection: The connection to use, if not the default.
+
+        Returns:
+            The response lines received from the server.
+        """
+        conn = connection or await self.get_connection()
+
         # Send the command
         async with self._command_lock:
             self._logger.debug("Sending command: %s", request)
             await conn.write(f"{request}\n")
 
-            # Read the response
+            # Read all lines of the response
             response_lines = []
             while True:
                 response_line = await conn.readuntil(b"\r\n", self._read_timeout)
                 response_line = response_line.rstrip()
 
                 # Handle error codes
                 if response_line.startswith("R:ERROR"):
@@ -142,28 +189,27 @@
                     continue
 
                 # Return the response once we see the response line
                 response_lines.append(response_line)
                 if response_line.startswith("R:"):
                     break
 
-        response = CommandResponse(response_lines)
-        self._logger.debug("Received response: %s", response)
+        self._logger.debug("Received response: %s", "\n".join(response_lines))
 
-        return response
+        return response_lines
 
     async def get_connection(self) -> CommandConnection:
         """Get a connection to the Host Command service."""
         async with self._connection_lock:
             if self._connection.closed:
                 # Open a new connection
                 await self._connection.open()
 
                 # Authenticate the new connection if we have credentials
-                if self._username is not None and self._password is not None:
+                if self._username and self._password:
                     await self.command(
                         "LOGIN",
                         self._username,
                         self._password,
                         connection=self._connection,
                     )
```

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/events.py` & `aiovantage-0.6.0/src/aiovantage/command_client/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 class EventType(Enum):
     """Enumeration of event types."""
 
     CONNECTED = "connect"
     DISCONNECTED = "disconnect"
     RECONNECTED = "reconnect"
     STATUS = "status"
+    LOG = "log"
     ENHANCED_LOG = "enhanced_log"
 
 
 class ConnectEvent(TypedDict):
     """Event emitted when the connection is established."""
 
     type: Literal[EventType.CONNECTED]
@@ -160,15 +161,15 @@
         """Get a connection to the Host Command service."""
         async with self._connection_lock:
             if self._connection.closed:
                 # Open a new connection
                 await self._connection.open()
 
                 # Authenticate the new connection if we have credentials
-                if self._username is not None and self._password is not None:
+                if self._username and self._password:
                     await self._send(f"LOGIN {self._username} {self._password}")
 
             return self._connection
 
     def subscribe(
         self,
         callback: EventCallback,
@@ -364,26 +365,30 @@
         # Send a plaintext message to the Host Command service."""
         self._logger.debug("Sending message: %s", message)
         await self._connection.write(f"{message}\n")
 
     def _parse_message(self, message: str) -> None:
         # Parse a message from the Host Command service.
         if message.startswith("S:"):
-            # Parse a "Status" message
+            # Parse a "status" message, of the form "S:<type> <id> <args>"
+            # These messages are emitted when the state of an object changes after
+            # subscribing to updates via "STATUS <type>" or "ADDSTATUS <vid>".
             status_type, id_str, *args = tokenize_response(message)
             self.emit(
                 {
                     "type": EventType.STATUS,
                     "status_type": status_type[2:],
                     "id": int(id_str),
                     "args": args,
                 }
             )
         elif message.startswith("EL:"):
-            # Parse an "Enhanced Log" message
+            # Parse an "enhanced log" message, of the form "EL:<log>"
+            # These messages are emitted when an enhanced log is received after
+            # subscribing to updates via "ELLOG <type>".
             self.emit({"type": EventType.ENHANCED_LOG, "log": message[4:]})
         elif message.startswith("R:ERROR"):
             self._logger.error("Error message from EventStream: %s", message)
 
     def _queue_command(self, command: str) -> None:
         # Queue a command to be sent to the Host Command service.
         self._command_queue.put_nowait(command)
```

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/__init__.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/anemo_sensor.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/anemo_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/base.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/blind.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/button.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/color_temperature.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/color_temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/gmem.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/introspection.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/introspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,12 +18,12 @@
     async def get_firmware_version(self, vid: int, image: Firmware) -> str:
         """Get the firmware version.
 
         Args:
             vid: The Vantage ID of the controller.
             image: The firmware image to get the version of.
         """
-        # INVOKE <id> IntroSpection.GetFirmwareVersion <image>
-        # -> R:INVOKE <id> <rcode> IntroSpection.GetFirmwareVersion <image> <version>
-        response = await self.invoke(vid, "IntroSpection.GetFirmwareVersion", image)
+        # INVOKE <id> Introspection.GetFirmwareVersion <image>
+        # -> R:INVOKE <id> <rcode> Introspection.GetFirmwareVersion <image> <version>
+        response = await self.invoke(vid, "Introspection.GetFirmwareVersion", image)
 
         return response.args[4].rstrip()
```

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/light_sensor.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/light_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/load.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/rgb_load.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/rgb_load.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/sensor.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/sounder.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/sounder.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/task.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/task.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/command_client/interfaces/temperature.py` & `aiovantage-0.6.0/src/aiovantage/command_client/interfaces/temperature.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/README.md` & `aiovantage-0.6.0/src/aiovantage/config_client/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/__init__.py` & `aiovantage-0.6.0/src/aiovantage/config_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     async def get_connection(self) -> ConfigConnection:
         """Get a connection to the ACI service."""
         async with self._connection_lock:
             if self._connection.closed:
                 await self._connection.open()
 
                 # Ensure the connection is authenticated, if required
-                if self._username is not None and self._password is not None:
+                if self._username and self._password:
                     # Log in if we have credentials
                     success = await self.request(
                         Login,
                         Login.Params(self._username, self._password),
                         self._connection,
                     )
```

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/helpers.py` & `aiovantage-0.6.0/src/aiovantage/config_client/helpers.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/xml_dataclass.py` & `aiovantage-0.6.0/src/aiovantage/config_client/xml_dataclass.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/methods/types.py` & `aiovantage-0.6.0/src/aiovantage/config_client/methods/types.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py` & `aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/get_filter_results.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/get_object.py` & `aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/get_object.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/methods/configuration/open_filter.py` & `aiovantage-0.6.0/src/aiovantage/config_client/methods/configuration/open_filter.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/methods/introspection/get_version.py` & `aiovantage-0.6.0/src/aiovantage/config_client/methods/introspection/get_version.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/methods/login/login.py` & `aiovantage-0.6.0/src/aiovantage/config_client/methods/login/login.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/objects/__init__.py` & `aiovantage-0.6.0/src/aiovantage/config_client/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/objects/blind.py` & `aiovantage-0.6.0/src/aiovantage/config_client/objects/blind.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/objects/button.py` & `aiovantage-0.6.0/src/aiovantage/config_client/objects/button.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/objects/gmem.py` & `aiovantage-0.6.0/src/aiovantage/config_client/objects/gmem.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/objects/load.py` & `aiovantage-0.6.0/src/aiovantage/config_client/objects/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 @dataclass
 class Load(LocationObject):
     """Load object."""
 
     load_type: str = xml_element("LoadType")
+    parent_id: int = xml_element("Parent")
     power_profile_id: int = xml_element("PowerProfile")
 
     def __post_init__(self) -> None:
         """Declare state attributes in post init."""
         self.level: Optional[float] = None
 
     @property
```

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/objects/omni_sensor.py` & `aiovantage-0.6.0/src/aiovantage/config_client/objects/omni_sensor.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/objects/rgb_load.py` & `aiovantage-0.6.0/src/aiovantage/config_client/objects/rgb_load.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         HSIC = "HSIC"
         CCT = "CCT"
         COLOR_CHANNEL = "Color Channel"
 
     color_type: ColorType = xml_element("ColorType")
     min_temp: int = xml_element("MinTemp")
     max_temp: int = xml_element("MaxTemp")
+    parent_id: int = xml_element("Parent")
 
     def __post_init__(self) -> None:
         """Declare state attributes in post init."""
         self.hsl: Optional[Tuple[int, int, int]] = None
         self.rgb: Optional[Tuple[int, int, int]] = None
         self.rgbw: Optional[Tuple[int, int, int, int]] = None
         self.level: Optional[int] = None
```

### Comparing `aiovantage-0.5.0/src/aiovantage/config_client/objects/system_object.py` & `aiovantage-0.6.0/src/aiovantage/config_client/objects/system_object.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 class SystemObject:
     """Base class for all objects."""
 
     id: int = xml_attribute("VID")
     master_id: int = xml_attribute("Master")
     mtime: XmlDateTime = xml_attribute("MTime")
     name: str = xml_element("Name")
-    model: str = xml_element("Model")
     note: str = xml_element("Note")
+    model: str = xml_element("Model")
     display_name: str = xml_element("DName")
```

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/anemo_sensors.py` & `aiovantage-0.6.0/src/aiovantage/controllers/anemo_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/base.py` & `aiovantage-0.6.0/src/aiovantage/controllers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
             # Keep track of which objects we've seen
             cur_ids.add(obj.id)
 
         # Handle objects that were removed
         for vid in prev_ids - cur_ids:
             obj = self._items.pop(vid)
-            self.emit(VantageEvent.OBJECT_REMOVED, obj)
+            self.emit(VantageEvent.OBJECT_DELETED, obj)
 
         # Subscribe to the event stream if this is the first subscription
         if self.stateful and fetch_state and not self._subscribed_to_event_stream:
             await self._subscribe_to_event_stream()
 
         self._initialized = True
         self._logger.info("%s initialized", self.__class__.__name__)
@@ -172,15 +172,15 @@
 
         self._logger.info("%s fetched state", self.__class__.__name__)
 
     def subscribe(
         self,
         callback: EventCallback[T],
         id_filter: Union[int, Tuple[int], None] = None,
-        event_filter: Union[VantageEvent, Tuple[VantageEvent], None] = None,
+        event_filter: Union[VantageEvent, Tuple[VantageEvent, ...], None] = None,
     ) -> Callable[[], None]:
         """Subscribe to status changes for objects managed by this controller.
 
         Args:
             callback: The callback to call when an object changes.
             id_filter: The Vantage IDs to subscribe to, all objects if None.
             event_filter: The event types to subscribe to, all events if None.
```

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/blind_groups.py` & `aiovantage-0.6.0/src/aiovantage/controllers/blind_groups.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/blinds.py` & `aiovantage-0.6.0/src/aiovantage/controllers/blinds.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/buttons.py` & `aiovantage-0.6.0/src/aiovantage/controllers/buttons.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/dry_contacts.py` & `aiovantage-0.6.0/src/aiovantage/controllers/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/gmem.py` & `aiovantage-0.6.0/src/aiovantage/controllers/gmem.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Controller holding and managing Vantage variables."""
-
+import re
 from typing import Sequence, Union
 
 from typing_extensions import override
 
 from aiovantage.command_client.interfaces import GMemInterface
+from aiovantage.command_client.utils import parse_byte_param
 from aiovantage.config_client.objects import GMem
 from aiovantage.controllers.base import BaseController, State
 
 
 class GMemController(BaseController[GMem], GMemInterface):
     """Controller holding and managing Vantage variables."""
 
@@ -38,10 +39,15 @@
     def _parse_value(self, vid: int, value: str) -> Union[int, str, bool]:
         # Parse the results of a GMem lookup into the expected type.
         gmem: GMem = self[vid]
 
         if gmem.is_bool:
             return bool(int(value))
         if gmem.is_str:
+            # Handle byte array strings
+            if re.match(r"^[\[\{].*[\]\}]$", value):
+                byte_param = parse_byte_param(value)
+                return byte_param.decode().rstrip("\x00")
+
             return value
 
         return int(value)
```

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/light_sensors.py` & `aiovantage-0.6.0/src/aiovantage/controllers/light_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/loads.py` & `aiovantage-0.6.0/src/aiovantage/controllers/loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/omni_sensors.py` & `aiovantage-0.6.0/src/aiovantage/controllers/omni_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/rgb_loads.py` & `aiovantage-0.6.0/src/aiovantage/controllers/rgb_loads.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/stations.py` & `aiovantage-0.6.0/src/aiovantage/controllers/stations.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/tasks.py` & `aiovantage-0.6.0/src/aiovantage/controllers/tasks.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/src/aiovantage/controllers/temperature_sensors.py` & `aiovantage-0.6.0/src/aiovantage/controllers/temperature_sensors.py`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/LICENSE` & `aiovantage-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/README.md` & `aiovantage-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/pyproject.toml` & `aiovantage-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiovantage-0.5.0/PKG-INFO` & `aiovantage-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiovantage
-Version: 0.5.0
+Version: 0.6.0
 Summary: Interact with and control Vantage InFusion home automation controllers.
 Project-URL: Documentation, https://github.com/loopj/aiovantage#readme
 Project-URL: Issues, https://github.com/loopj/aiovantage/issues
 Project-URL: Source, https://github.com/loopj/aiovantage
 Author-email: James Smith <james@loopj.com>
 License-Expression: MIT
 License-File: LICENSE
```

