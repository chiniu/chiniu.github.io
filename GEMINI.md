# Project Overview

This project is a web-based interface for controlling an "Eink Frame" device. It allows users to connect to the device via Bluetooth, send images, and draw on the screen. The interface is built with HTML, CSS, and vanilla JavaScript.

The core functionalities of this web application are:
- **Bluetooth Connectivity:** It uses the Web Bluetooth API to connect to the e-ink device, send commands, and transfer data.
- **Image Upload and Processing:** Users can upload images, which are then processed using various dithering algorithms (Floyd-Steinberg, Atkinson, etc.) to match the e-ink display's color limitations.
- **Canvas Drawing:** A canvas element allows users to draw, write text, and erase, and then send the resulting image to the device.
- **Device Control:** The interface provides controls for clearing the screen, sending raw commands, and managing the device.

# Building and Running

This is a static web project and does not require a build process. To run the application, simply open the `index.html` file in a web browser that supports the Web Bluetooth API (e.g., Chrome, Edge).

There are no explicit build or test commands found in the project.

# Development Conventions

The project uses vanilla JavaScript and follows a modular pattern by separating different functionalities into their own files:
- `main.js`: Handles the main application logic, including Bluetooth communication and UI management.
- `dithering.js`: Contains functions for various image dithering algorithms.
- `paint.js`: Manages the canvas drawing and text insertion functionalities.
- `crop.js`: Implements the image cropping functionality.

The code is not formatted with a consistent style, and there are no linting configurations. The project uses a versioning system for the CSS and JS files by appending a query string (e.g., `?v=20250731`).
