# [BUG-04] Checkout does not complete after clicking Finish (error_user)

**Severity:** 🟠 High
**Priority:** P2
**Status:** Open
**Module:** Checkout
**Found using account:** `error_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC048

## Steps to Reproduce
1. Log in as error_user / secret_sauce
2. Add an item to the cart and go to Checkout
3. Enter valid First Name, Last Name and Postal Code
4. Click Continue
5. On the Overview page, click Finish

## Expected Result
The order completes and the 'Thank you for your order' confirmation page is displayed.

## Actual Result
Clicking Finish does not complete the order; the application throws an error and the confirmation page is never reached.


## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-04 screenshot](BUG-04.png)

## Labels
`bug`, `severity:high`, `module:checkout`
