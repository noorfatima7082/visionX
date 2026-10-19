# VisionX

A real-time AI vision lab that runs entirely in the browser. No server, no uploads, no install — just open the page and let your webcam do the work.

Final project for **CS-504 Digital Image Processing**, Fall 2025.

## Live demo

Open `index.html` in any modern browser, click **Start Camera**, and switch between the three tabs. (Hosted version: `https://noorfatima7082.github.io/visionX`)

## What it does

**Gesture Lab.** Detects and classifies 12+ hand gestures live using MediaPipe's 21 hand landmarks. Shows the gesture name, confidence, finger status, and a gesture history trail. Works with two hands at once.

**Color Analyzer.** Pulls dominant colors from the live webcam feed using pixel-level quantization. Shows named colors, hex values, HSL metrics, brightness, saturation, and color temperature.

**Face Analyzer.** Finds faces with TinyFaceDetector, overlays 68 facial landmarks, and predicts age, gender, and 7 emotional states in real time. All neural networks run on-device through TensorFlow.js — zero frames leave your computer.

## How it works

Webcam → mode router → three independent modules → live canvas overlay and analysis panel. Everything ships in a single HTML file. Key tech: MediaPipe Hands, face-api.js, TensorFlow.js, WebAssembly, WebGL, and the Canvas API.

## Files in this repo

| File | What it is |
|---|---|
| `index.html` | The VisionX app itself — the live demo |
| `standee.html` | A1 standee poster for the project |
| `slides.html` | The full project presentation deck (10 slides) |

## Team

Built as a team of three: gesture recognition, color analysis, and face analysis.
