---
target_identity: "file:/home/claude/eric-design-web/demos/nacar/index.html"
target_fingerprint: "sha256:72a9173f2a940da370a6eb2cd71f24af63d8d8a188fa6e50289006c0eae4cfb6"
target_path: /home/claude/eric-design-web/demos/nacar/index.html
timestamp: 2026-10-23T15-45-26Z
slug: demos-nacar-index-html
---
---
total_score: 25
max_score: 32
na_heuristics: 7,10
p0_count: 1
p1_count: 1
---
Method: dual-agent (A: design review · B: detector + headless browser)

Score: 25/32 (78%, Good) before fixes. Heuristics 7 and 10 n/a.
Specificity: high — shade card with bottles on colour tiles, live almond-nail preview (brillo/mate/cromo), colour carried into booking and confirmation, "Cuatro mesas" autoclave story, phone as display type.
Detector: 5 cramped-padding, all false positives (containers have 20–56px padding; .done measured while hidden).
Priority issues (all fixed):
- [P0] Form stayed visible after submit (`form{display:grid}` beat `hidden`) → `[hidden]{display:none!important}`.
- [P1] "Hacer otra reserva" rendered as default grey button → reset `button.link`.
- [P2] Two Reservar buttons on mobile first screen → rail button only once docked.
- [P2] Dark strip under nail preview; cromo band too heavy → matched surface, thinner band.
- [P2] .detail / .shape empty without photo → hide .detail, bottle fallback in shape.
- [P2] Content hidden if IntersectionObserver never fires → timed safety net.
- [P2] Focus ring 1.7:1 on light sections; input border 1.4:1 → dark outline there, border #6b5853, 2px input focus.
- [P3] Tap targets (corners, brand, footer) <44px; services missing from select; "hoy" late in day.
Personas: Jordan (form still live after confirm), Casey (duplicate CTAs), Riley (double submit, missing service).
Taste inspector after fixes: 0 FAIL with photos loaded; offline only few-pictures/hero-void (Unsplash blocked in sandbox) + no-footage WARN.
