# FLOWIC

FLOWIC is a lightweight Windows clipboard image processing tool designed to reduce repetitive image operations in real-world engineering workflows.

The project was built to solve frequent, small but high-cost inefficiencies encountered during daily design and documentation tasks. It remains extremely compact (approx. 185KB) while delivering professional-grade image clarity.

---

## 🌟 New Features (v1.2.0)

- **Intelligent Image Engine**: Automatically detects "Graphic Mode" (charts, CAD, code) vs "Photo Mode" (landscapes, portraits).
- **Anti-Aliased Scaling**: Uses high-precision super-sampling logic to eliminate jagged edges on diagonal lines.
- **Energy-Balanced Sharpening**: A custom sharpening kernel `(7*Center - Side) / 3` ensures text and thin lines remain bold and legible after downsampling.
- **Zero-Dependency Core**: Pure Win32/GDI+ implementation, portable and lightning-fast.

---

## ⌨️ Shortcuts

- **Ctrl + G** Get current image size as reference (source of truth for scaling).

- **Ctrl + R** Force scaling using the current mode.

- **F9** **Binary Inversion**: Inverts colors to Black & White (ideal for high-contrast documentation).

- **F10** **Background Whitening**: Converts dark backgrounds to pure white while preserving foreground details.

---

## 🚀 Changelog / 更新日志

### v1.2.0 (2026-01-08)

#### 🇨🇳 中文版 (Chinese Version)
**【核心更新】图像处理引擎深度进化：智能识别与超采样技术**
* **智能内容感知**：通过网格化采样，毫秒级判定图片类型并自动切换最优缩放策略。
* **图表细节增强 (Office 级渲染)**：
  - **斜线抗锯齿**：解决 1.0x - 0.5x 缩放时的“楼梯感”。
  - **能量平衡锐化**：重塑缩放后发虚的线条，确保文字黑亮、清晰。
  - **超采样逻辑**：解决非整数倍缩放导致的像素偏移。
* **风景照丝滑处理**：采用双三次插值 (Bicubic) 与 Gamma 补偿，确保自然渐变无断层。

#### 🇺🇸 English Version
**【Major Update】Deep Evolution of Image Engine: Smart Detection & Super-sampling**
* **Intelligent Content Awareness**: Grid sampling determines image types in milliseconds to apply specialized scaling strategies.
* **Graphic Detail Enhancement (Office-Level Rendering)**:
  - **Anti-Aliasing**: Eliminates "staircase" artifacts on diagonal lines during downsampling.
  - **Energy-Balanced Sharpening**: Custom kernel reinforces faded lines, keeping text bold and legible.
  - **Super-sampling Logic**: Resolves pixel phase shifts caused by non-integer scaling.
* **Smooth Landscape Processing**: Uses Bicubic Interpolation and Gamma compensation to maintain smooth gradients in natural photos.

---

### v1.1.0.1 (2026-01-02)

**Fixes**
- Supported JPG / PNG / BMP clipboard read.
- Fixed image scaling mode persistence.
- Added single-instance detection.

**UI Improvements**
- Improved High-DPI compatibility (100%-250%).
- Refined UI colors for better integration with modern Windows.

---

## Background

This tool is developed and iterated by an engineer based on real workflow pain points. It focuses on the balance between **extreme portability** and **visual precision**, ensuring that every screenshot pasted into a report looks sharp and professional.
