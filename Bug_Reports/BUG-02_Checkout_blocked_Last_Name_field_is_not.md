# [BUG-02] Checkout blocked: Last Name field is not editable (problem_user)

**Severity:** 🔴 Critical
**Priority:** P1
**Status:** Open
**Module:** Checkout
**Found using account:** `problem_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC049

## Steps to Reproduce
1. Log in as problem_user / secret_sauce
2. Add any item to the cart and go to Checkout
3. On Checkout Step One, enter First Name 'John'
4. Click into the Last Name field and attempt to type 'Doe'
5. Enter Postal Code '10001'
6. Click Continue

## Expected Result
All three fields accept text input and the user proceeds to the Order Overview page.

## Actual Result
The Last Name field does not accept any keyboard input. The user cannot complete this required field and is blocked from proceeding, making checkout impossible for this account type.


## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-02 screenshot](BUG-02.png)

## Labels
`bug`, `severity:critical`, `module:checkout`
