---
target_identity: "file:/home/claude/eric-design-web/demos/nacar/index.html"
target_fingerprint: "sha256:6cc3b4e3d945bdcf9e3c9916b2d2128a9afec527e88813cab88f15411bc63e2a"
target_path: /home/claude/eric-design-web/demos/nacar/index.html
timestamp: 2026-10-23T18-05-24Z
slug: demos-nacar-index-html
---
---
total_score: 24
max_score: 32
na_heuristics: 7,10
p0_count: 0
p1_count: 2
---
Method: dual-agent (A: design review · B: detector + headless browser), after the rebuild onto the Lumière/Navaja family style.

Previous version scored 20/32 with a P0 brand break (different fonts, square corners, no header, no theme toggle). Rebuilt with Cormorant + Hanken Grotesk, Navaja header/console, Lumière arch hero, light/dark toggle, rose accent, self-hosted photos.
Score now: 24/32 (75%, Good). Consistency 1 → 3.
Detector: cramped-padding on .shade and flat-type-hierarchy — false positives (nails bleed off on purpose; detector saw only small headings).
Issues found and fixed:
- [P1] Mobile: no booking button after the hero → header Reservar kept on phones.
- [P1] Content hidden if IntersectionObserver never fires → all groups revealed after 2.5s; reduced motion shows everything at once.
- [P2] Two confirm buttons on mobile last step → sticky bar hides at the confirm step; title without price.
- [P2] Step bar lacked Navaja's connectors and the mobile step name → restored.
- [P2] "p. m.." double period; "Confirmar por WhatsApp" after booking → fixed, renamed "Enviar por WhatsApp".
- [P2] Chrome finish read as a glitch → diagonal reflection; mate desaturates.
- [P2] Four photos repeated, salon interior was a hair salon → 12 distinct nail photos.
- [P3] Times without a. m./p. m. → Mañana/Tarde groups; Blanco francés swatch outlined; days 44px; today focus ring 2px; aria-describedby on errors; placeholder contrast; arch inner ring above photo; "Hacer otra reserva" resets the picker.
Taste inspector: 0 FAIL (no-footage WARN).
