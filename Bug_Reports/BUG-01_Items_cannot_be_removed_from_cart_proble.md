# [BUG-01] Items cannot be removed from cart (problem_user)

**Severity:** 🔴 Critical
**Priority:** P1
**Status:** Open
**Module:** Shopping Cart
**Found using account:** `problem_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC034

## Steps to Reproduce
1. Log in as problem_user / secret_sauce
2. Add Sauce Labs Backpack, Sauce Labs Bike Light, and Sauce Labs Onesie to the cart
3. Open the Cart page
4. Click 'Remove' next to each item

## Expected Result
Each item is removed from the cart and the cart badge count decreases accordingly.

## Actual Result
The 'Remove' button does not respond for Backpack, Bike Light, and Onesie. All three items remain in the cart and the badge count does not change.


## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-01 screenshot](BUG-01.png)

## Labels
`bug`, `severity:critical`, `module:shopping-cart`
