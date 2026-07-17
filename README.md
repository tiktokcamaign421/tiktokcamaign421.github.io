# PayoutAudit — 3-tap funnel (v6, final)

Blurred store footage runs the background (grocery aisle + Target orbit),
crossfading per screen. The ending is a single-focus sequence: an animated
"reading answers / matching programs / signals matched" readout driven by
the real match math, then the best-match reveal — store offer name and a
$750 odometer count-up — then the audit receipt prints, then the ledger.

## Offers
Three store deal-reward paths (Target / Amazon / Costco), matched from the
quiz answers. The $750 figure is each partner's published top reward tier;
it is always presented as "Up to $750," tied to completing listed deals,
with requirements auto-expanded on the best match and the top-tier-not-
typical note in the FAQ. That framing is what keeps TikTok review and
network compliance off your back.

## Deploy / update
Replace the repo contents with this folder:
```
git add . && git commit -m "v6" && git push
```

## Before sending traffic
1. Tracking links — three `#PASTE_TRACKING_LINK_n` urls in the OFFERS
   config at the top of the script in index.html.
2. Footer Terms / Privacy / Contact are placeholders; a live privacy
   policy is required by most ad platforms and CPA networks.
3. Confirm $750 matches each offer's current published cap; update the
   `cap` field per offer if a partner changes tiers.
