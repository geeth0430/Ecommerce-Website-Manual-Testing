# [BUG-10] No loading indicator during delayed login (performance_glitch_user)

**Severity:** 🟢 Low
**Priority:** P4
**Status:** Open
**Module:** Login
**Found using account:** `performance_glitch_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC011

## Steps to Reproduce
1. Enter username 'performance_glitch_user' and password 'secret_sauce'
2. Click Login
3. Observe the page during the delay before the inventory page loads

## Expected Result
A loading indicator (spinner or disabled button state) should communicate that the login request is processing.

## Actual Result
Login takes approximately 5 seconds with no visual feedback, giving the impression the page is unresponsive or frozen.

## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-10 screenshot](BUG-10.png)

## Labels
`bug`, `severity:low`, `module:login`
