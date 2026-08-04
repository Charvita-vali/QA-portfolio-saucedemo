# BUG-002: Checkout cannot be completed — Last Name field is unresponsive for problem_user

## Environment
- **URL:** https://www.saucedemo.com
- **Browser:** Chrome (fill in your version)
- **OS:** (fill in yours)
- **User:** problem_user

## Preconditions
- User is logged in as `problem_user`
- At least one item is in the cart

## Steps to Reproduce
1. Log in with username: `problem_user`, password: `secret_sauce`
2. Add any product to the cart (click "Add to cart")
3. Click the cart icon → click "Checkout"
4. On the "Checkout: Your Information" page, click into the **Last Name** field
5. Attempt to type any text (e.g., "Smith")

## Expected Result
User should be able to type into the Last Name field, then click Continue to proceed to the Overview page and complete the order.

## Actual Result
The Last Name field does not accept keyboard input — text cannot be entered. Clicking "Continue" then triggers a validation error ("Last Name is required"), permanently blocking checkout completion for this user.

## Severity
**Critical** — This completely blocks the core business function (purchasing) with no available workaround.

## Priority
**Critical / P0** — Revenue-blocking bug. In a real production environment this would mean zero conversions for affected users and would likely be escalated for an immediate hotfix.

## Attachments
- `screenshots/bug002_checkout_blocked.png` — Cursor in Last Name field with no text entered despite keystrokes
- `screenshots/bug002_validation_error.png` — Resulting "Last Name is required" validation error after clicking Continue

## Additional Notes
This confirms `problem_user` is intentionally seeded with a checkout-blocking defect, likely designed for QA training purposes. Confirmed this does **not** reproduce with `standard_user`, isolating it as user-account-specific rather than an application-wide regression.

---

## Reproducibility

**Always (5/5)**

The issue was reproduced consistently on every attempt during testing.

---

## Environment

- Application: SauceDemo
- Browser: Google Chrome
- Platform: Desktop
- Test User: `problem_user`

---

## Root Cause

Unknown.

Developer investigation required.

---

## Retest Status

Not Retested

---

## Regression Testing

Not Performed

Regression testing will be performed after the defect is fixed.
