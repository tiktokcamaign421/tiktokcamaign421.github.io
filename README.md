# PayoutAudit — 3-tap funnel (v7)

Full-bleed store footage runs the background; the results section is a
scroll-driven Apple-style product page: hero brand reveal, CTA strip, a
"How it works" chapter with per-step animation, the audit receipt, and
the full ranked offer ledger — every block animates as you reach it.

## Offers wired in
- **Amazon Product Reviewer** — https://trksy.org/aff_c?offer_id=789&aff_id=157168
- **Amazon Rewards Ladder** — https://linkthem.net/aff_c?offer_id=144&aff_id=157168
- **Costco Deal Rewards** — https://giftclick.org/aff_c?offer_id=941&aff_id=157168
- **Trader Joe's Deal Rewards** — https://giftclick.org/aff_c?offer_id=854&aff_id=157168
- **Target Reward Program** — https://linkthem.net/aff_c?offer_id=317&aff_id=157168
  drop it into the OFFERS config in index.html)

## Routing (verified)
- Amazon-tech / Amazon-home → Amazon (Reviewer or Ladder based on tag overlap)
- Target → Target
- Trader Joe's / "Mostly grocery stores" → Trader Joe's
- Costco → Costco
- "A bit of everywhere" → Amazon (marketplace default)

## Deploy / update
Replace the repo contents with this folder:
```
git add . && git commit -m "v7" && git push
```

## Before sending traffic
1. (All five offers are wired.)
2. Terms / Privacy / Contact are placeholders; a live privacy policy is
   required by most ad platforms and CPA networks.
3. If a partner changes its top reward tier, update the `cap` on that
   offer so the odometer stays accurate.
