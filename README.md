# 3D Model Reconstruction from 2D Images

This project focuses on reconstructing a 3D model from multiple 2D images.  
It is organized into two modules:

- Primary Module: 3D Model Generation
- Secondary Module: Image Acquisition

## Overview

The system captures object images from different viewpoints and uses them to generate a 3D representation.  
The goal is to provide a practical pipeline that connects data capture with model reconstruction.

## Implemented Modules

### 1. 3D Model Generation (Primary)

This module is responsible for creating the final 3D model from collected 2D images.

Main responsibilities:
- Preprocess input images
- Extract visual features
- Match features across views
- Reconstruct scene/object structure
- Produce a 3D output model

### 2. Image Acquisition (Secondary)

This module handles image capture planning and collection.

Main responsibilities:
- Capture images from multiple angles
- Maintain consistent lighting/background (where possible)
- Ensure sufficient overlap between consecutive views
- Prepare images for the reconstruction pipeline

## Current Repository Structure

- `3D Model generation web.html` - web interface/prototype for 3D model generation
- `Image Acquisition mobile design` - mobile-side design/assets for image acquisition workflow
- `README.md` - project documentation

## Typical Workflow

1. Acquire object images using the Image Acquisition module.
2. Validate image quality (sharpness, coverage, overlap).
3. Feed images into the 3D Model Generation module.
4. Run reconstruction steps to generate the 3D model.
5. Review/export the reconstructed output.

## Requirements

Depending on your implementation stack, you may need:

- A modern web browser (for web module/prototype)
- Mobile device or mobile emulator (for acquisition design flow)
- Reconstruction backend/tools (if connected externally)

> Note: This repository currently contains interface/design artifacts and documentation.  
> Add runtime dependencies and scripts once the processing backend is integrated.

## How to Run (Current State)

### Web Prototype
1. Open `3D Model generation web.html` in a browser.
2. Interact with the available UI to review the 3D generation flow.

### Mobile Design
1. Open the `Image Acquisition mobile design` assets in your preferred design/viewing tool.
2. Review acquisition screens and user flow.

## Limitations

- End-to-end automated reconstruction pipeline may not be fully integrated yet.
- Output quality depends heavily on image quality and view coverage.
- Real-world performance can vary with lighting, texture, and object geometry.

## Future Improvements

- Integrate a complete reconstruction backend into the web flow
- Add automated image quality checks before processing
- Support direct mobile-to-web image upload pipeline
- Add export support for common 3D formats (e.g., `.obj`, `.ply`, `.glb`)
- Add evaluation metrics for reconstruction quality

## Author

Saira Ahmed
