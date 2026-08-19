# WiFi Sensing — Live 3D Point Cloud Viewer

Hosted at: https://heripurnamawibu-art.github.io/Inspired_Wifi_Sensing_Project/pointcloud/

Based on the original RuView project by ruvnet.

## Modes

- Default — synthetic in-browser demo (no backend, no network calls).
- `?backend=auto` — fetch from `/api/splats` on the same origin
  (only works when the viewer is served by `ruview-pointcloud serve`).
- `?backend=<url>` — fetch from `<url>/api/splats`. The intended
  local-ESP32 use is `?backend=http://127.0.0.1:9880`.
- `?live=1` — require a live backend; show an offline message instead
  of falling back to the synthetic demo.

See ADR-094 for the deployment design.
