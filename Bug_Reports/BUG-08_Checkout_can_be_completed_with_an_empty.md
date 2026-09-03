# [BUG-08] Checkout can be completed with an empty cart (standard_user)

**Severity:** 🟢 Low
**Priority:** P4
**Status:** Open
**Module:** Shopping Cart
**Found using account:** `standard_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC031

## Steps to Reproduce
1. Log in as standard_user / secret_sauce
2. Without adding any items, open the Cart page
3. Click Checkout and complete Steps One and Two

## Expected Result
The system should prevent checkout when the cart contains 0 items, or display a warning.

## Actual Result
Checkout proceeds normally with no validation and the order completes for $0.00 with 0 items.


## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-08 screenshot](BUG-08.png)

## Labels
`bug`, `severity:low`, `module:shopping-cart`
