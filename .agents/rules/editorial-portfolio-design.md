---
description: Enforces editorial, minimalist engineering standards for portfolio and README design, prohibiting generic AI aesthetic tropes.
globs: ["**/*README*.md", "**/*.svg"]
always_on: true
---

# Editorial Engineering Design Standards

1. **Aesthetic Philosophy**:
   - Deliver an "editorial AI-engineering technical paper / lab interface" aesthetic (reminiscent of Linear, Apple technical whitepapers, or Swiss typography).
   - Prohibit generic "AI-generated" tropes: neon blue/purple cyberpunk glows, starfield particle storms, bouncing/rotating technology icons, trophy walls, and widget clutter.

2. **Color System**:
   - **Light Canvas (Default)**: 95% White/Off-white (`#FFFFFF`, `#FAFAFA`), 4% Deep Black (`#111111`, `#000000`), 1% Subtle Neutral Gray (`#E5E5E5`, `#555555`).
   - **Dark Canvas (GitHub Dark)**: 95% Deep Neutral Dark (`#0A0A0A`, `#0D1117`), 4% Crisp White (`#EDEDED`, `#FFFFFF`), 1% Structural Gray (`#262626`, `#888888`).
   - Accent color is pure structural contrast (black on light, white on dark). No unsolicited rainbow/neon palettes.

3. **Motion & Animation Vocabulary**:
   - Animation must represent **computation and system flow**, never superficial decoration.
   - Allowed primitives: slow coordinate grid drift (20-30s), single discrete signal dot traversing an architecture pipeline (7-12s), subtle pulse/scan (4-9s).
   - Technology badges and skill icons must remain completely static.

4. **GitHub Platform Architecture**:
   - Use standard `<picture>` wrappers with `(prefers-color-scheme: dark)` and `(prefers-color-scheme: light)` for all hero and system SVG assets.
   - SVGs must be 100% self-contained using pure SMIL (`<animate>`, `<animateTransform>`, `<path>`) without external JS or cross-origin dependencies.
