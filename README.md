# Afterimage

Afterimage is a small, browser-based camera mirror experiment. It uses a live webcam feed and CSS filters to create a high-contrast, x-ray-inspired look, with a minimal control panel and adjustable effect intensity.

> This is a visual effect only. It does not produce or simulate a medical X-ray and cannot reveal bones, organs, or other information beneath the skin.

## Run it

Camera access is available only in a secure browser context: use `https://` when hosted, or `localhost` for local development.

The project has no build step or dependencies. From the project folder, start a local server, for example:

```bash
python -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) and select **Enable camera**. Allow camera access when prompted. Use **End session** to stop the camera.

## Features

- Live, mirrored webcam preview
- Stylized monochrome and green-tinted visual treatment
- Adjustable effect intensity
- Responsive layout for desktop and mobile
- Camera video stays in the browser tab and is not uploaded by this app

## Privacy

The page requests camera access only after you choose **Enable camera**. Video is displayed locally in the page. No analytics, accounts, or server-side video processing are included.

## Browser support

Use a modern browser with `getUserMedia` support. Camera access requires HTTPS or localhost. If access is denied, update the browser's site permissions and try again.

## Project files

- `index.html` — complete standalone app, styles, and camera controls
- `README.md` — setup, feature, and privacy notes

## License

No license has been selected for this repository yet. Add a license before inviting reuse or redistribution.
