# Afterimage

Afterimage is a live face-tracking anatomy mirror. Select an overlay and the skull, brain, or facial muscle illustration follows your face as you move in front of the camera.

> This is an artistic camera effect. It does not show real anatomy, create X-ray images, or provide medical information.

## Run locally

Camera access requires a secure context: use HTTPS when hosted or `localhost` during local development.

There is no build step. From this folder, start a static web server:

```bash
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000), allow camera access, and choose an anatomy layer. The first start downloads the MediaPipe Vision runtime and face landmark model. A network connection is needed to load those resources.

## Layers and controls

- **Skull** — tracked skull outline, eye sockets, nasal cavity, teeth, jaw, and neck vertebrae
- **Brain** — a tracked brain illustration with lobe folds
- **Muscles** — a tracked facial muscle illustration
- **Overlay glow** — adjusts the illustration intensity
- **End session** — stops the local webcam stream

## Privacy

The camera starts only after you click **Start face tracking** and grant permission. MediaPipe runs face landmark detection locally in the browser. The camera frames are not uploaded by this app. The library and model files are fetched from jsDelivr and Google Cloud when first needed.

## Browser support

Use a current Chrome, Edge, Firefox, or Safari browser with WebAssembly and camera support. The camera API requires HTTPS or localhost. For best tracking performance, use a device with hardware acceleration enabled.

## Files

- `index.html` — app UI, camera handling, local face tracking, and original canvas anatomy illustrations
- `README.md` — setup and feature notes

## License

No license has been selected for this repository yet. Add a license before inviting reuse or redistribution.
