# Palette Forge

Palette Forge is a next-generation color-system generator built around the OKLCH color space. It produces perceptually consistent tonal ramps, semantic color sets, and WCAG-compliant palettes while remaining 100 percent client-side.

## Key Capabilities

- OKLCH color processing for modern, perceptually uniform ramps
- Automatic tonal scaling from light to dark
- Semantic palettes: success, warning, danger, info
- WCAG-compliant contrast evaluation
- Color-vision deficiency simulation (protanopia, deuteranopia, tritanopia)
- Image to palette extraction
- Export formats: CSS custom properties, Tailwind config, Figma tokens, JSON
- Open-source under CC-BY/MIT

Palette Forge works well for design-system work, UI/UX prototyping, game UI pipelines, accessibility testing, and teaching color theory.

## Quick Start

1. Pick a color with the color picker or enter a hex value.
2. Optionally upload an image to extract its dominant color.
3. Toggle between light and dark themes to review tonal behavior.
4. Review the accessibility panel for contrast compliance.
5. Copy tokens in CSS, Tailwind, Figma, or JSON format.

## Saving Palettes

Use "Save Full Color System" to export every swatch as a PNG, or select "Save as Image" beside each section to capture only the portion you need.

## Technical Overview

The engine uses OKLCH to generate perceptually uniform 50-900 scales, semantic hue variations, and interaction-state tokens (hover, active, disabled). It performs WCAG 2.1 text and non-text audits, simulates color-vision conditions with SVG filters, and optimizes semantic spacing for deuteranopia. Image uploads support dominant-color extraction for brand references. Live previews, contrast matrices, and semantic chips update in real time. Export formats include :root CSS variables, Tailwind extend.colors, and Figma Tokens JSON. The project is built with static HTML/CSS/JS and requires no build tooling.

## Feature Comparison

| Feature                                | Palette Forge | Material Theme Builder | Leonardo | Coolors | Tailwind Tools |
|----------------------------------------|---------------|------------------------|----------|---------|----------------|
| OKLCH color space                      | Yes           | No (HCT only)          | Partial  | No      | No             |
| WCAG contrast scoring                  | Yes           | Partial                | Yes      | No      | No             |
| Semantic color ramps                   | Yes           | No                     | No       | No      | No             |
| Light-to-dark tonal system             | Yes           | No                     | Limited  | No      | Limited        |
| Color-vision simulations               | Yes           | No                     | No       | No      | No             |
| Token exports (CSS vars, Tailwind)     | Yes           | Partial                | No       | No      | Limited        |
| Figma token export                     | Yes           | No                     | No       | No      | No             |
| Image-based color extraction           | Yes           | No                     | No       | Limited | No             |
| 100% client-side (no servers)          | Yes           | No (cloud services)    | No       | No      | No             |
| Open source                            | CC/MIT        | No                     | Yes      | No      | Some tools     |

## License

Licensed under CC BY 4.0. You may share and adapt this work, including commercially, provided you attribute Christopher Davis and document any changes. This tool is provided "as is" and results should be validated before use in production environments.

## Author

- Christopher Davis  
- Version 1.0 — November 2025  
- Email: tweakyourpc@gmail.com
