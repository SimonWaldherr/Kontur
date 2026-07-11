# Kontur

**Kontur** converts bitmap graphics into editable SVG files directly in the browser. It is designed for logos, lettering, symbols, and clean color areas—without uploads: image processing stays on your device.

- **Source code:** [SimonWaldherr/Kontur](https://github.com/SimonWaldherr/Kontur)
- **Live app:** [simonwaldherr.github.io/Kontur](https://simonwaldherr.github.io/Kontur/)

## Features

- Import images by drag and drop or file picker, including PNG, JPG, WebP, BMP, and TIFF
- Automatically vectorize images and compare the original, processed image, and resulting SVG
- Inspect and refine SVG paths and color layers in the browser
- Choose between Auto, Standard, and Expert modes
- Adjust thresholding, smoothing, colors, and image-preprocessing settings
- Export the finished SVG file

## Local and private

The browser version processes image data locally. No image upload to an external service is required.

## Run locally

Kontur is a static website. Clone this repository and either open `index.html` in a modern browser or serve the repository root with any static web server. The vectorization workspace is available at [`tool.html`](./tool.html).

To publish it with GitHub Pages, use the repository root as the deployment source.

## Technology

- [Potrace](https://potrace.sourceforge.net/) via WebAssembly for contour and path vectorization
- [ImageTracerJS](https://github.com/jankovicsandras/imagetracerjs) as an optional color-layer comparison engine
- HTML, CSS, and JavaScript as a static browser build

## License notes

Kontur uses open-source components. In particular, Potrace and `esm-potrace-wasm` are licensed under GPL-2.0, while ImageTracerJS is released under the Unlicense. Distribution of this project is subject to the respective dependency licenses.
