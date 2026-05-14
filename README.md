# kofun

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A collection of examples for rendering 3D models of ancient Japanese tombs (kofun) in the browser. This project demonstrates various methods for loading and displaying VRML 1.0 models using Three.js and A-Frame.

## Demos

- **[Solid Model Viewer (Three.js)](https://code4fukui.github.io/kofun/kofun.html)**: An interactive viewer with orbit controls, rendering a solid model using the standard Three.js `VRMLLoader`.
- **[Wireframe Viewer (Three.js)](https://code4fukui.github.io/kofun/test.html)**: A wireframe visualization built with a custom VRML parser in JavaScript.
- **[Basic Scene (A-Frame)](https://code4fukui.github.io/kofun/aframe.html)**: A simple demonstration of loading a VRML model within an A-Frame scene using a custom component.

## Features

- **Multiple Rendering Approaches**: Demonstrates rendering VRML 1.0 models using:
  - The standard Three.js `VRMLLoader` (`kofun.html`)
  - A custom from-scratch VRML parser (`test.html`)
  - An A-Frame custom component (`aframe.html`)
- **Interactive Viewers**: Both Three.js examples include interactive orbit controls for model inspection.
- **VRML Data**: Utilizes `.wrl` (VRML 1.0) files representing the multi-layered geometry of the tombs.

## Usage

To run these examples locally, you need to serve the files from a local web server, as browser security policies prevent loading models directly from the filesystem.

1.  Clone this repository:
    ```sh
    git clone https://github.com/code4fukui/kofun.git
    ```
2.  Navigate to the project directory:
    ```sh
    cd kofun
    ```
3.  Start a simple local web server (e.g., using Python):
    ```sh
    # For Python 3
    python -m http.server
    ```
4.  Open one of the example files in your browser:
    - `http://localhost:8000/kofun.html`
    - `http://localhost:8000/test.html`
    - `http://localhost:8000/aframe.html`

## Data Source

The VRML models of the tombs are based on data provided by Sakai City, Japan.

- [3D Comparison of Three Major Tombs in Sakai City](https://www.city.sakai.lg.jp/kanko/rekishi/dkofun/3dhikaku/funbohikaku.html)

## License

MIT License — see [LICENSE](LICENSE).