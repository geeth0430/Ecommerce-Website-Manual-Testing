# [BUG-07] Checkout Name/Zip fields accept invalid character types (standard_user)

**Severity:** 🟡 Medium
**Priority:** P3
**Status:** Open
**Module:** Checkout
**Found using account:** `standard_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC042

## Steps to Reproduce
1. Log in as standard_user / secret_sauce
2. Add an item and go to Checkout
3. Enter First Name '12345', Last Name '@@@@', Postal Code '####'
4. Click Continue

## Expected Result
Fields should validate character type: Name fields should reject purely numeric/symbolic input and Postal Code should reject non-alphanumeric symbols.

## Actual Result
No client-side validation is applied to character type. Any combination of numbers and symbols is accepted and the user proceeds to the Overview page.

## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-07 screenshot](BUG-07.png)

## Labels
`bug`, `severity:medium`, `module:checkout`
