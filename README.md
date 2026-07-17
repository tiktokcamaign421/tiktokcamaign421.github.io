# PayoutAudit — 3-tap funnel (v5)

Full-bleed video funnel. The footage is the background under an ink scrim
with a slow drift; scenes crossfade per screen (receipts → box → receipts).
Choreographed intro, per-word headline, magnetic CTA, and a FLIP answer
trail — tapped answers physically fly up into breadcrumb chips.

## Structure
```
index.html   — markup, styles, logic (single file)
assets/      — 3 looping MP4s (H.264) + posters
```

## Deploy / update
Replace the repo contents with this folder, then:
```
git add . && git commit -m "v5" && git push
```

## Before sending traffic
1. Tracking links — OFFERS config at the top of the script in index.html
   (three `#PASTE_TRACKING_LINK_n` urls).
2. Terms / Privacy / Contact — footer links are placeholders; a live
   privacy policy is required by most ad platforms and CPA networks.

## Notes
- If video can't load (old webview, blocked autoplay), the poster takes
  over automatically — never an empty frame.
- prefers-reduced-motion / no-JS render the complete page statically.
- No dollar-amount promises, countdowns, or fabricated proof. Disclosure
  on every screen; per-offer requirements; "Guarantees … 0" on the receipt.
