---
target: demos/navaja/index.html
total_score: 24
max_score: 32
na_heuristics: 7,10
p0_count: 0
p1_count: 2
target_identity: "file:/home/claude/eric-design-web/demos/navaja/index.html"
target_fingerprint: "sha256:14a145b77de98ccc1f93eb8ca7b339f39922e45619b0033201c11c19f5a57dfd"
target_path: /home/claude/eric-design-web/demos/navaja/index.html
timestamp: 2026-10-23T14-36-05Z
slug: demos-navaja-index-html
---
Method: dual-agent (A: design review · B: detector + headless browser)

Score: 24/32 (75%, Good). Heuristics 7 and 10 n/a (Persuade).
Specificity: booking console is authored (RD$, "El que esté libre", toalla caliente); perks strip, footer and image fallback were generic.
Detector: 10 CLI (4 low-contrast on empty summary values, 2 undersized "Barber Studio", italic serif h1, cramped-padding FP, overused font, flat hierarchy partial FP); overlay adds nested-cards (deliberate console panels) and placeholder advisories. Calendar days 36px, footer links 23px.
Priority issues:
- [P1] Mobile flow: no guidance, unlabeled stepper, no reachable action.
- [P1] Confirmation undersold: no service/price, no WhatsApp or calendar.
- [P2] Image fallback reads as broken (identical gold blobs, empty hero).
- [P2] Times without a. m./p. m.; "Sin escoger" at 2:1 contrast; footer 24h vs 12h.
- [P3] Empty panels under short columns; numbering duplicated.
Personas: Jordan ("·" avatar, no contact link), Riley (1-char name message, 13-digit phone, Agendar otra wipes data, refresh loses state), Casey (no sticky CTA, focus under header).
