# [BUG-11] Certain products cannot be added to cart (problem_user)

**Severity:** 🟠 High
**Priority:** P2
**Status:** Open
**Module:** Shopping Cart
**Found using account:** `problem_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC035

## Steps to Reproduce
1. Log in as problem_user / secret_sauce
2. On the Inventory page, click 'Add to cart' on Sauce Labs Bolt T-Shirt
3. Click 'Add to cart' on Sauce Labs Fleece Jacket
4. Click 'Add to cart' on Test.allTheThings() T-Shirt (Red)

## Expected Result
Each item is added to the cart, the cart badge increments, and each button changes to 'Remove'.

## Actual Result
None of the three items are added. The cart badge does not increment and the buttons remain in the 'Add to cart' state.

## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-11 screenshot](BUG-11.png)

## Labels
`bug`, `severity:high`, `module:shopping-cart`
