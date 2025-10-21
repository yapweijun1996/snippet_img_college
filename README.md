# Snippet Image Collage

This repository demonstrates a responsive, no-crop image collage layout implemented entirely in a single `index.html` file. The page showcases multiple collage configurations and the JavaScript algorithms responsible for arranging images into balanced compositions.

## Overview

The layout engine preloads images, wraps them in absolutely positioned tiles, and attempts to fill each collage container using a column-first strategy. When the optimal column arrangement cannot be found, the engine falls back to balanced row layouts and special handling for small image sets.

## Key Features

- **Column-first solver** that maximizes container utilization by evenly distributing images into columns while respecting minimum image sizes and gap constraints.
- **Row-based fallback** to ensure aesthetically pleasing layouts when the column solver cannot satisfy constraints.
- **Quantized positioning** so every tile snaps to integer pixel values, preventing visible seams or drift.
- **Resize awareness** via observers that recompute layouts when container dimensions change.

Refer to `index.html` for the complete implementation and example collages showcasing different configurations.
