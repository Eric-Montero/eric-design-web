---
target: demos/fade-club/index.html
total_score: 27
max_score: 40
na_heuristics: 
p0_count: 0
p1_count: 3
target_identity: "file:/home/claude/eric-design-web/demos/fade-club/index.html"
target_fingerprint: "sha256:b03a06c7aca825755e23be0341ff32489b7164591c82e42285d8608043cfa9d4"
target_path: /home/claude/eric-design-web/demos/fade-club/index.html
timestamp: 2026-10-23T14-36-05Z
slug: demos-fade-club-index-html
---
Method: dual-agent (A: design review · B: detector + headless browser)

Score: 27/40 (68%, Acceptable, edge of Good).
Specificity: Dominican copy, RD$ combo, monograms; layout is the gallery-standard booking app; no WhatsApp; photo fallbacks empty.
Detector: 10 CLI (5 cramped-padding FP on rows/paybar, 2 dark-glow on .fab, low-contrast pitch eyebrow 4.0:1, icon-tile-stack welcome logo, cream page bg on desktop stage). Overlay: hidden-screen repeats FP; .screens 16px wider than viewport from date row; promo button 40px tall.
Priority issues:
- [P1] Tab bar stays on Detail; pay bar floats above it.
- [P1] Barber card / centre button land on an unchosen service that can't be changed.
- [P1] Double-booking possible; bookings lost on refresh.
- [P2] Hero fallback wastes the fold.
- [P2] No next action after booking; shop unreachable (no WhatsApp/map).
Personas: Jordan (no service choice, no a. m./p. m., "·" avatar, Sunday dim only), Riley (double booking, refresh, cancel never times out), Casey (two stacked bottom bars).
