# 3D Scan Alignment & Measurement

## Short Description
- This project provides a frontend/backend solution to precisely align raw 3D scan data and perform circumference measurements on cross-sections. The goal is to support manual and automatic alignment workflows as well as provide a robust architecture for visualization, measurement, and server-side auto-alignment services.

## Main Features
- **Manual Alignment (Frontend):**
    - Translation and rotation controls for the 3D model
    - Reset and undo functions
    - Intuitive UI for precise positioning

- **Circumference Measurement Tool (Frontend):**
    - Draggable circular and elliptical contours on cross-sections
    - Real-time display of the circumference
    - Support for multiple cross-section planes

- **Optional Auto-Alignment (Backend):**
    - API endpoint for automatic alignment based on reference models or heuristics
    - Frontend triggers the service and renders the returned aligned model

## Architecture and Technology
- **Frontend:** Three.js-based visualization for browser and mobile support
- **Backend:** REST/HTTP service to perform automatic alignment (e.g., Node.js / Python)
- **Data format:** Supports common 3D formats (PLY, OBJ, GLTF) and server-side conversion if needed
- **Focus:** Clean code, documentation, and responsive UI

## Example API (Conceptual)
- `POST /api/align/auto` — Request: raw scan | Response: aligned model (GLTF/OBJ)
- `GET /api/models/:id` — Delivers stored reference models

## Development and Usage Notes
- **Local Development:** Start frontend with a local dev server; provide backend stub for auto-alignment
- **Tests:** Unit tests for measurement logic and alignment transformations
- **Browser Support:** Modern Chromium and Firefox-based browsers; responsive adjustments for mobile browsers

## Goals for Further Development
- Improved automatic alignment (ICP, ML-based initialization)
- Extended measurement tools (areas, distances, volumes)
- Persistent project and version management for multiple scans

## File
- This description is intended for `README.md` and provides an overview of the content and purpose of the project.
