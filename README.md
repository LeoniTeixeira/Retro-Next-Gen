# Retro-Next-Gen

**Retro-Next-Gen** is a specialized game engine focused on 16-bit era aesthetics and behaviors (SNES/Mega Drive style), but built with a modern technical foundation. The project emphasizes a strict separation between visual data and physical logic, allowing for high-fidelity retro experiences with updated performance and flexibility.

## 🎯 Project Purpose

The goal is to recreate the development experience of classic consoles, overcoming original hardware limitations (such as color palettes and memory constraints) while maintaining sub-pixel precision, sensor-based collision, and 8x8 pixel tile segmentation.

## 🛠️ Tech Stack

- **Language:** Go (Golang) - For performance, concurrency, and simplicity.

- **Base Engine:** [Ebitengine](https://ebitengine.org/) - A dead-simple 2D game library for Go.

- **Shaders:** Kage (Ebitengine's shading language) for palette manipulation and visual effects.

- **Versioning:** Git following the `Verb: #ID - Title` commit pattern.

## ⚙️ Technical Highlights

1. **8x8 Tile System:** All rendering is based on 8x8 pixel block segmentation, optimizing memory usage and CPU cache locality.

2. **Dedicated Collision Map:** Physics are independent of visuals. A standalone logical map dictates player and world interactions.

3. **TileDefinitions:** Efficient use of Bitmasks to define properties like `Solid`, `Damage`, `Slippery`, or `Platform`.

4. **Flexible Resolution:** Native support for real-time switching between 4:3 and 16:9 aspect ratios without pixel distortion.

---

*Developed with a focus on technical solidity and retro precision.*
