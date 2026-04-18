# E-commerce Coupon Template

Ordo marketplace template for a coupon decision flow.

## What it does

- Grants a VIP coupon when `user_vip_level >= 2` and `cart_amount >= 200`
- Grants a standard coupon when `user_vip_level < 2` and `cart_amount >= 500`
- Returns `NOT_ELIGIBLE` when the promotion window is closed

## Install

This repository is meant to be discovered by Ordo's GitHub marketplace search.
It exposes the required `ordo-template.json` file at the repository root.

## Topic

Add the GitHub topic `ordo-template` so Ordo can find it in the marketplace.
