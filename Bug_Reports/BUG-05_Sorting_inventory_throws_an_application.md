# [BUG-05] Sorting inventory throws an application error (error_user)

**Severity:** 🟡 Medium
**Priority:** P3
**Status:** Open
**Module:** Product Sorting
**Found using account:** `error_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC022

## Steps to Reproduce
1. Log in as error_user / secret_sauce
2. On the Inventory page, open the sort dropdown
3. Select 'Price (high to low)'

## Expected Result
Products reorder by descending price with no errors.

## Actual Result
A JavaScript error is thrown in the browser console and the product order does not change.


## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-05 screenshot](BUG-05.png)

## Labels
`bug`, `severity:medium`, `module:product-sorting`
