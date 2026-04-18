# E-commerce Coupon Template

Marketplace template repository for Ordo.

This repository is intentionally split into two views of the same template:

- `ordo-template.json`
  Single-file marketplace manifest consumed by Ordo's GitHub installer.
- `template/`
  Source template in the same multi-file layout used by the built-in platform templates.

## Repository Metadata

- Template ID: `ecommerce-coupon`
- Difficulty: `beginner`
- Icon: `shopping-cart`
- Marketplace topic: `ordo-template`

## What This Template Does

This decision flow issues discount coupons based on:

- whether the promotion window is open
- the user's VIP level
- the cart amount

Decision outcomes:

- `GRANTED` with `coupon_type = vip` and `discount_rate = 0.2`
- `GRANTED` with `coupon_type = standard` and `discount_rate = 0.1`
- `NO_COUPON`
- `NOT_ELIGIBLE`

## Files

Root marketplace entry:

- `ordo-template.json`

Raw source template:

- `template/meta.json`
- `template/facts.json`
- `template/concepts.json`
- `template/ruleset.json`
- `template/samples.json`
- `template/contract.json`
- `template/tests.json`
- `template/i18n/en.json`
- `template/i18n/zh-CN.json`
- `template/i18n/zh-TW.json`

## Install In Ordo

1. Connect GitHub inside Ordo Studio.
2. Open Marketplace.
3. Search for this repository by topic `ordo-template` or by repository name.
4. Install it into an organization as a new project.

## Notes

- The marketplace installer reads `ordo-template.json` from the repository root.
- The `template/` directory is included so the repository remains auditable and reusable outside the marketplace flow.
