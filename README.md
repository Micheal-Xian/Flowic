# FLOWIC

FLOWIC is a lightweight Windows clipboard image processing tool designed to reduce repetitive image operations in real-world engineering workflows.

The project was built to solve frequent, small but high-cost inefficiencies encountered during daily design and documentation tasks.

---

## Features

- Read images directly from clipboard (JPG / PNG / BMP)
- Scale images using fixed or reference-based modes
- Keyboard-driven workflow for fast operations
- High-DPI display support (100%–250%)
- Single-instance protection to avoid duplicate runs

---

## Shortcuts

- **Ctrl + G**  
  Get current image size as reference

- **Ctrl + R**  
  Force scaling using the current mode

- **F9 / F10**  
  Execute quick processing actions

---

## Changelog

### v1.1.0.1 (2026-01-02)

**Fixes**
- Fixed clipboard JPG image read failure (now supports JPG / PNG / BMP)
- Fixed image scaling mode not being remembered after restart
- Added single-instance detection with popup warning

**UI Improvements**
- Improved High-DPI compatibility
- Unified background color (RGB 242, 242, 242), removed default white frame

---

## Background

This tool is developed and iterated by a single engineer, acting as product designer, developer, and tester, based on real workflow pain points rather than abstract feature design.
