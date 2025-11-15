# Street View for Cardboard

**Street View for Cardboard** is a web-based viewer that lets you explore Google Street View in VR mode using a cardboard headset and your mobile phone. Just tap a location on the map, go fullscreen, and slide your phone into the viewer for an immersive experience.

## 🗺️ Features

- **Interactive world map** to pick any location on Earth.
- **Google Street View integration** in VR (side-by-side) mode.
- **Cardboard-ready viewer** with dual iframes simulating left and right eye views.
- **Fullscreen mode** for a seamless VR experience.
- Supports basic look-around and navigation features using device sensors and screen taps.

## 📁 Project Structure

```
Street-View-For-Cardboard/
├── index.html          # The main map interface to select a location
├── viewer/
│   └── index.html      # Side-by-side Street View for VR mode
└── embed/
    └── index.html      # Street View panorama for embedding
```

- `index.html`: Allows users to select a location on a world map and navigate to the VR viewer.
- `viewer/index.html`: Creates a side-by-side Street View display for placing inside a cardboard viewer.
- `embed/index.html`: Displays a single Street View panorama (used by both eye views in the viewer).

## 🚀 Demo Instructions

1. **Open the app** on your mobile device and switch to landscape mode.
2. **Select a location** by tapping anywhere on the map.
3. Tap **“Let’s go!”** to enter VR mode.
4. On the next screen, tap **“Go Fullscreen.”**
5. **Place your phone** into a cardboard viewer.
6. **Tilt your head** to look around. To move within Street View, tap on the screen on both sides (you may need to cut multiple holes in your cardboard viewer for this).

## 🧰 Setup & Usage

### Requirements

- A mobile device with a gyroscope (optional but recommended).
- A cardboard VR viewer.
- A Google Maps JavaScript API key.

### Setup

1. Clone or download the repo.
2. Replace `YOUR_API_KEY` in both:
   - `index.html`
   - `embed/index.html`
3. Serve the files via a local or remote web server.

> Please note: The Maps API may not work properly if opened directly via the `file://` protocol.

### Example

After setup, navigate to:

```
http://localhost/Street-View-For-Cardboard/
```

Pick a location, go fullscreen, and start exploring!

## 🛠️ Possible Improvements

- Improved movement/navigation without having to tap the screen (Or only requiring a tap on one side).
- UI enhancements for better VR interaction.

## 🧪 Tested On

- Firefox 129.0
- Android 9
- Samsung Galaxy S10e (SM-G970U)
- POP! Cardboard 3.0 Viewer

## 📄 License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License.  
See the [LICENSE](LICENSE) file for details.
