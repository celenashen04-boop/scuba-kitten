# Scuba Kitten

Do the scuba dance in front of your webcam: put your left hand on your nose and wave your right hand in front of your face. A 3D model of the Scuba Kitten automaton copies your waving forearm's angle, so it waves exactly as fast as you do.

- Body tracking: [MediaPipe Pose Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/pose_landmarker) (runs in the browser)
- 3D: [three.js](https://threejs.org), with the model's real linkage animated (gears, crank shuttle, arm hinge)
- Optional: **Connect Arduino** drives the physical motor kitten over Web Serial (Chrome/Edge)

## Run

The page has to be served over http (opening the file directly won't load the 3D model):

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000 in Chrome and click **Start camera**.
