# PayoutAudit — 3-tap funnel (v8)

Results section rebuilt from scratch: everything a user needs on the
first fold, then chapters that animate in as you scroll.

## First fold (no scroll needed)
- **Device-frame hero card** playing the winning brand's video sharp inside
  a phone-shaped frame, scrim'd at the bottom for legibility.
- **"You can claim up to · Trader Joe's / Target / Amazon / Costco"** — big
  brand name, per the winning offer.
- **Count-up from $0 → $750** on a two-color emerald gradient with a
  progress ring around it filling as the number climbs. Sparks fire at
  the end; the CTA immediately picks up a pulsing halo.
- **"Continue to <brand>"** — the primary CTA sits directly under the card,
  above the fold. Sponsored + T&C fine print stays quiet under it.

## Just below the fold
- **The ladder** — four visual tiles ($50 → $150 → $400 → $750) with icons
  and the top tier highlighted emerald. Replaces the wall of text.

## Below that (scroll-triggered)
- **How it works** — same 4 steps, now with per-step icons instead of prose.
- **The audit** receipt prints line by line when you reach it.
- **All matches** — full offer ledger, best offer's requirements auto-open.
- FAQ, footer.

## Offers wired in (verified)
- Amazon Product Reviewer — https://trksy.org/aff_c?offer_id=789&aff_id=157168
- Amazon Rewards Ladder — https://linkthem.net/aff_c?offer_id=144&aff_id=157168
- Target Reward Program — https://linkthem.net/aff_c?offer_id=317&aff_id=157168
- Costco Deal Rewards — https://giftclick.org/aff_c?offer_id=941&aff_id=157168
- Trader Joe's Deal Rewards — https://giftclick.org/aff_c?offer_id=854&aff_id=157168

## Deploy
```
git add . && git commit -m "v8" && git push
```

## Notes
- Reveal-hero visuals: the "storefront sign" video is now Trader Joe's;
  the "aisle" video is the fallback for the "everywhere" answer.
- If a partner changes its top reward tier, update the `cap` field on that
  offer so the odometer stays accurate.
