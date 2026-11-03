# Event camera on the Meta Ray-Ban Display

Web app page for the Meta Ray-Ban Display glasses: shows the picture of an event camera (last 100 ms) and the gesture
label of a spiking neural network, streamed live from a laptop or an AMD Kria board (bachelor's thesis at fortiss,
project EMMANÜELA).

- `index.html` is the page (600 × 600, black is transparent on the glasses' additive display).
- `config.json` holds the WebSocket address of the current stream. The stream runs through a tunnel whose address
  changes, so the tunnel script updates this file and the page reads it when it (re)connects.

Page: https://jan-vitzthum.github.io/meta_EVcamera_tunnel/

No data is stored here; the stream only exists while the laptop or board is running.
