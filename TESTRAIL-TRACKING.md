# SauceDemo E-Commerce QA — TestRail Test Management

**Project:** SauceDemo E-Commerce QA
**Companion to:** [QA-portfolio-saucedemo](https://github.com/Charvita-vali/QA-portfolio-saucedemo)

Live TestRail project: test cases organized by feature, executed as a formal test run with logged results and comments — complementing the manual test plan and Jira defect tracking in this repository.

## Test Case Structure

| Section | Test Cases |
|---|---|
| Login | Verify login with valid username and password; Verify login fails with invalid password |
| Cart | Verify user can add item to cart; Verify cart persists across page navigation |
| Checkout | Verify checkout completes with valid shipping info; Verify order confirmation displays after checkout |

## Test Run — 8/22/2026

All 6 test cases executed and marked **Passed**, each with a logged comment describing the exact steps taken and observed result — for example:

> "Entered invalid password. Error message 'Epic sadface: Username and password do not match any user in this service' displayed correctly."

**Result: 100% passed (6/6).**

## Screenshots

- `testrail-run-results.png` — Test Run summary showing 100% passed across all sections
- `testrail-checkout-results.png` — Checkout section results
- `testrail-case-detail.png` — Individual test case with logged result, comment, and timestamp

---

*Built as a companion to the [SauceDemo manual testing project](https://github.com/Charvita-vali/QA-portfolio-saucedemo) to demonstrate hands-on experience with TestRail test case management and execution.*
