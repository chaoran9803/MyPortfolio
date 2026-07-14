# Portfolio site — design settings (remember across sessions)

**Pages:** index.dc.html (Home), experience.dc.html, projects.dc.html, contact.dc.html — linked via plain `<a>` nav.

**Palette (dark/blue, code-style):**
- bg `#0a0f1c`, card bg `#101725`, chip bg `#132038` / hover `#1c3357`
- ink `#e7edfb`, muted text `#7d8bab`, body text `#b6c4e6`
- accent blue `#2f6fed`, accent hover `#5b9bff`, button text `#eaf2ff`
- borders `rgba(90,150,255,0.22)`, shadows `rgba(0,0,0,0.4)`

**Type:** JetBrains Mono everywhere (headings + body) — monospace/"code" look.

**Motion system:**
- Entrance: `fadeUp` keyframes, staggered per section (0.1s increments).
- Hover: buttons/cards/chips lift (`translateY(-2 to -6px)`) + blue glow shadow; nav tabs get a pill background (`#1c3357`) + lift on hover.
- Cursor effect: fixed circular lens (`#liquid-lens`) using `backdrop-filter:url(#liquid)` (SVG feTurbulence+feDisplacementMap), follows cursor with easing/lerp, intensity scales with mouse speed, soft radial mask edge.
- Background: subtle meteor shower — diagonal streaks (`meteorFall` keyframes), fixed layer behind content (z-index:0), content wrapper at z-index:1.

Keep new sections consistent with this system (same hex tokens, same hover/lift pattern, same JetBrains Mono).
