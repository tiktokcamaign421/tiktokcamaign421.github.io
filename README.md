# PayoutAudit — 3-tap funnel (v9)

Results rebuilt from zero. One fold, one story:

- **Hero card**: the winning brand's footage, blurred, runs behind a looping
  3-scene mechanic demo — "Complete a deal" (check draws itself) →
  "Discount unlocks" (price tag springs in) → "Sometimes it's huge"
  (big-ticket item + slash + sparks). Scene dots cycle every 2.7s.
  A tiny "Illustration · values vary by deal" note keeps it honest.
- **All text sits on solid ink below the card** — brand name, one line,
  and the CTA ("Continue to <brand>") with a pulsing halo. CTA verified
  above the fold at 844px and 740px viewports.
- Removed entirely: the AUDIT COMPLETE bar, the receipt, the tier tiles,
  the how-it-works chapter, all $-figure hero numbers. Page length cut
  roughly in half. Per-offer "How it works — steps" remains on each offer.

## Cache fix
All assets renamed (vid-*.mp4 / img-*.jpg). The old deploy's cached
trader.mp4 can no longer shadow the Trader Joe's sign video. After
pushing, one hard-refresh may be needed on devices that cached the page.

## Offers wired (verified routing)
- Amazon Product Reviewer — trksy.org/aff_c?offer_id=789&aff_id=157168
- Amazon Rewards Ladder — linkthem.net/aff_c?offer_id=144&aff_id=157168
- Target Reward Program — linkthem.net/aff_c?offer_id=317&aff_id=157168
- Costco Deal Rewards — giftclick.org/aff_c?offer_id=941&aff_id=157168
- Trader Joe's Deal Rewards — giftclick.org/aff_c?offer_id=854&aff_id=157168

## Deploy
Replace repo contents with this folder:
```
git add . && git commit -m "v9" && git push
```
