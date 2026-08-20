# 🎵 AI Music Generator

A browser-based **AI Music Generator** : Music Generation with AI**.

The application uses a lightweight **LSTM neural network** with TensorFlow.js to learn patterns from symbolic music note sequences and generate new original melodies directly in the browser.

## ✨ Features

* 🧠 LSTM-based AI music generation
* 🎼 Built-in symbolic music dataset
* 🎵 Original melody generation
* 🎛️ Dynamic music styles
* 🎹 Multiple instrument sounds
* 🎚️ Adjustable tempo from 60–160 BPM
* ▶️ Play generated music
* ⏹️ Stop playback
* 📊 Real-time music visualization
* 💾 Automatic MIDI file download
* 📱 Responsive design
* ⚡ Lightweight browser-based implementation
* 🔒 No backend server required

## 🎼 Music Styles

The application supports different musical styles:

* Classical
* Epic Cinematic
* Indian Cinematic
* Ambient
* Folk

The **Indian Cinematic** mode creates an original epic-style melody using custom note patterns and percussion accents. It does **not reproduce copyrighted movie songs or melodies**.

## 🎹 Instruments

The generated music can be played using different synthesized sounds:

* Piano
* Strings
* Flute
* Guitar
* Synth

## 🎚️ Tempo Control

The tempo can be adjusted dynamically between:

**60 BPM – 160 BPM**

This allows the generated music to be played at different speeds.

## 🧠 AI Model

The application uses a lightweight **Long Short-Term Memory (LSTM)** neural network.

The model contains:

* LSTM layer with 24 units
* Dense layer with 12 neurons
* Output layer for predicting the next musical note
* Adam optimizer
* Mean Squared Error loss

The model is trained directly inside the browser using **TensorFlow.js**.

## 📚 Data Processing

The application uses short symbolic music sequences represented as MIDI note numbers.

The processing pipeline is:

```text
Music Note Sequences
        ↓
MIDI Note Numbers
        ↓
Normalization
        ↓
3-Note Input Sequences
        ↓
LSTM Neural Network
        ↓
Next Note Prediction
        ↓
Generated Melody
```

## 🎵 Music Generation

The LSTM predicts the next note based on the previous three notes.

Small controlled variations are added to the prediction, and the generated notes are adjusted according to the selected musical scale.

This allows different styles to produce different original melodies.

## 🔊 Audio Generation

The project uses the browser's **Web Audio API** to synthesize the generated notes.

Different oscillator types are used to create different instrument-like sounds:

| Instrument | Sound Type |
| ---------- | ---------- |
| Piano      | Triangle   |
| Strings    | Sawtooth   |
| Flute      | Sine       |
| Guitar     | Triangle   |
| Synth      | Square     |

The Indian Cinematic mode also adds original low-frequency percussion accents.

## 💾 MIDI Export

Generated music can be downloaded as a standard:

```text
.mid
```

MIDI file.

The download starts automatically when the user clicks the **MIDI** button.

The generated filename includes the selected style and timestamp, for example:

```text
AI-Indian-Music-2026-08-20T16-45-30-123Z.mid
```

The file is downloaded to the browser's default download location.

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript
* TensorFlow.js
* LSTM Neural Network
* Web Audio API
* MIDI File Generation
* Canvas API

## 📂 Project Structure

```text
AI-Music-Generator/
│
└── index.html
```

The complete application is implemented in a single HTML file.

## 🚀 How to Run

### Option 1 – Open Locally

1. Download `index.html`.
2. Open the file in a modern web browser.
3. Wait for TensorFlow.js to initialize.
4. Click **Train AI**.
5. Select a music style and instrument.
6. Adjust the tempo if required.
7. Click **Generate**.
8. Click **Play** to listen to the generated music.
9. Click **MIDI** to download the generated music.

### Option 2 – GitHub Pages

1. Create a GitHub repository named:

```text
AI-Music-Generator
```

2. Upload `index.html`.
3. Go to **Settings → Pages**.
4. Select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`.
6. Click **Save**.
7. Open the generated GitHub Pages URL.

## ⚡ Performance

The project is optimized for browser execution by using:

* A lightweight LSTM architecture
* A small training dataset
* Only 10 training epochs
* Efficient TensorFlow tensor cleanup
* Short generated sequences
* Lightweight canvas visualization
* Non-blocking asynchronous training and playback

## ⚠️ Requirements

The application requires:

* A modern web browser
* JavaScript enabled
* Internet connection when loading TensorFlow.js from the CDN

Once the application is loaded, music generation and playback run in the browser.

The project demonstrates practical implementation of:

* AI/ML concepts
* LSTM neural networks
* Sequence prediction
* Music generation
* Browser-based machine learning
* Audio synthesis
* MIDI generation

## 👨‍💻 Author

**MANDLA NITEESH KUMAR**

---

⭐ If you like this project, consider giving the repository a star!
