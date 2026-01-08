# FLOWIC

FLOWIC is a lightweight Windows clipboard image processing tool designed to reduce repetitive image operations in real-world engineering workflows.

The project solves frequent, small, but high-cost inefficiencies encountered during daily design and documentation tasks. It remains extremely compact (approx. 196KB) while delivering professional-grade image clarity.

---

## 🌟 New Features (v1.2.0.0)

- **Intelligent Image Engine**: Automatically detects "Graphic Mode" (charts, CAD, code) vs "Photo Mode" (landscapes, portraits) using 400-point entropy sampling.
- **Anti-Aliased Scaling**: Implements high-precision super-sampling logic to eliminate "staircase" artifacts on diagonal lines.
- **Energy-Balanced Sharpening**: A custom sharpening kernel `(7*Center - Side) / 3` ensures text and thin lines remain bold and legible even after 50% downsampling.
- **Office-Level Precision**: Resolves pixel phase shifts in non-integer scaling (e.g., 0.7x), ensuring screenshots look sharp in Word/Excel reports.

---

## ⌨️ Shortcuts

- **Ctrl + G** Get current image size as reference (sets the target dimensions).

- **Ctrl + R** Force scaling using the current mode.

- **F9 (Binary Inversion)** Converts image to high-contrast Black & White.

- **F10 (Background Whitening)** Cleans dark backgrounds to pure white while preserving foreground details.

---

## 🚀 Changelog

### v1.2.0.0 (2026-01-08)
**Major Update: Smart Image Engine**
- **Content Awareness**: Millisecond-level grid sampling to determine image types.
- **Graphic Enhancement**: 
    - Eliminated aliasing on diagonal lines.
    - Reinforced faded lines using a custom energy-balanced convolution.
    - Fixed "blurring" issues caused by non-integer scaling ratios.
- **Photo Processing**: Switched to Bicubic Interpolation with Gamma compensation for smooth gradients.
- **Optimization**: Retained zero-dependency architecture; binary size optimized at ~185KB.

### v1.1.0.1 (2026-01-02)
- Added support for JPG/PNG/BMP clipboard formats.
- Fixed image scaling mode persistence.
- Added single-instance protection.
- Improved High-DPI compatibility (100%-250%).

---

## Background

Developed by an engineer for engineers. This tool bridges the gap between **extreme portability** and **visual precision**, ensuring every engineering screenshot is professional, clear, and perfectly sized for documentation.
