---
description: Enforces an 80/20 black-dominant monochrome computational minimalism standard for engineering portfolios, prohibiting decorative AI clichés and project redundancy.
globs: ["**/*README*.md", "**/*.svg"]
always_on: true
---

# Monochrome Computational Minimalism Standard

1. **Color Ratio & Palette**:
   - **Strict 80/20 Black/White Rule**: 80% Black (`#000000`, `#050505`, `#111111`), 20% White (`#FFFFFF`).
   - Zero colored accents: No blue, purple, green, neon, or rainbow gradients.
   - Structural contrast is achieved through geometry, line weight (0.8px–2px), white opacity levels (0.15–1.0), and generous negative space.

2. **Content Architecture (Identity vs. Evidence)**:
   - Do NOT duplicate repository or project catalogues inside the profile README. Repositories already provide proof; the README provides identity, philosophy, technology, and activity context.
   - Standard rhythm: `01 / IDENTITY` (Hero) → `02 / ENGINEERING FOCUS` → `03 / TECHNOLOGY` → `04 / ENGINEERING ACTIVITY` → `05 / CURRENTLY EXPLORING` → `06 / CONNECT`.

3. **Signature Animation Architecture**:
   - Animation must communicate computational identity (neural networks, distributed systems, topological DAGs), not superficial decoration.
   - Use multi-phase staged SMIL sequences:
     - **Phase 1 (Boot)**: System initialization telemetry.
     - **Phase 2 (Formation)**: Nodes appear, structural connections draw in.
     - **Phase 3 (Processing)**: Packets traverse edges.
     - **Phase 4 (Stable State)**: Calm, persistent equilibrium.
   - All animated assets must be self-hosted in `assets/` without external JS dependencies (`hero.svg`, `focus.svg`, `activity.svg`).

4. **GitHub Theme Adaptation & Background Illusion**:
   - Because GitHub blocks external CSS/HTML background modification outside the README container, SVGs must act as seamless theme containers matching GitHub's native page background colors:
     - Dark Mode (`prefers-color-scheme: dark`): Match deep black / GitHub dark (`#0d1117` / `#000000`).
     - Light Mode (`prefers-color-scheme: light`): Match GitHub light (`#ffffff` / `#fafafa`).
   - All animated assets must be paired into `<picture>` containers:
     ```html
     <picture>
       <source media="(prefers-color-scheme: dark)" srcset="./assets/<name>-dark.svg">
       <source media="(prefers-color-scheme: light)" srcset="./assets/<name>-light.svg">
       <img src="./assets/<name>-dark.svg" width="100%" alt="...">
     </picture>
     ```

5. **Identity & Title Invariants**:
   - Developer Name: Strictly use `RAYMUND GERARD ESTACA`. Do NOT use "ARDS" or informal pseudonyms.
   - Professional Title: Strictly use `FULL STACK AI ASSISTED DEVELOPER`.

6. **SVG Animation Reliability Standards**:
   - Base geometries must always be drawn with full base dimensions (never `width="0"` or hidden offsets) so graphics remain visible on static renderers and cached proxies.
   - Motion must be cyclical and continuous using `repeatCount="indefinite"` with `animateMotion` and `animateTransform` rather than one-shot `fill="freeze"`.
