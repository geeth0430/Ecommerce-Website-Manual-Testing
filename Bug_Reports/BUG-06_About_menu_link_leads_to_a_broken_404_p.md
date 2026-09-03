# [BUG-06] 'About' menu link leads to a broken/404 page (problem_user)

**Severity:** 🟡 Medium
**Priority:** P3
**Status:** Open
**Module:** Navigation
**Found using account:** `problem_user`
**Environment:** Chrome 128 / Windows 11 / saucedemo.com
**Linked Test Case:** TC051

## Steps to Reproduce
1. Log in as problem_user / secret_sauce
2. Open the hamburger menu
3. Click 'About'

## Expected Result
User is navigated to the Sauce Labs marketing website.

## Actual Result
The link resolves to a broken/404 page instead of the expected external site.


## Screenshot
*Illustrative mockup recreated from the reported steps/actual result — not a live capture of saucedemo.com.*

![BUG-06 screenshot](BUG-06.png)

## Labels
`bug`, `severity:medium`, `module:navigation`
