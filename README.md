# PayoutAudit — 3-tap funnel

Ink-dark, video-led bridge funnel for the shopping-discount offers.
Same motion system as the Playful bridge page (blur-through reveals,
spring curve, choreographed intro). Zero dependencies.

## Structure
```
index.html   — markup, styles, logic (single file)
assets/      — ping-pong looped MP4s (H.264), posters, cutouts
```

## Deploy
Drag the folder to Netlify/Vercel/Cloudflare Pages, or push to a repo
and enable GitHub Pages (main / root).

## Before sending traffic
1. **Tracking links** — in index.html, OFFERS config (top of the script),
   replace the three `#PASTE_TRACKING_LINK_n` urls.
2. **Terms / Privacy / Contact** — footer links are placeholders; a live
   privacy policy is required by most ad platforms and CPA networks.

## Notes
- The hero video is used twice on purpose: sharp inside the card, and
  enlarged + blur(60px) + ~13% opacity as the page's living background.
  The background copy crossfades per screen (cart → box → receipts).
- If video can't load (old webview, blocked autoplay), posters take over
  automatically — the page never shows an empty frame.
- All animation is transform/opacity/filter. `prefers-reduced-motion`
  and no-JS render the complete page statically.
- No dollar-amount promises, no countdowns, no fabricated proof.
  Disclosure on every screen; requirements listed per offer;
  "Guarantees … 0" printed on the audit receipt.
