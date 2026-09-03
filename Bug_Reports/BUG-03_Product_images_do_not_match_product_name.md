# [BUG-03] Product images do not match product names (problem_user)

**Severity:** 🟠 High
**Priority:** P2
**Status:** Open
**Module:** Product Listing
**Found using account:** `problem_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC017

## Steps to Reproduce
1. Log in as problem_user / secret_sauce
2. Land on the Inventory page
3. Compare each product's image against its name/description

## Expected Result
Each of the 6 products displays its own distinct, correct product image.

## Actual Result
All 6 products display the same incorrect placeholder image, making it impossible to visually distinguish items in the catalog.


## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-03 screenshot](BUG-03.png)

## Labels
`bug`, `severity:high`, `module:product-listing`
