# Test Plan — SauceDemo E-Commerce Application

## 1. Objective
Verify the core functional flows of SauceDemo (login, product cart, checkout) behave correctly across standard and edge-case scenarios, and identify defects through structured and exploratory testing.

## 2. Application Under Test
- **Name:** SauceDemo
- **URL:** https://www.saucedemo.com
- **Type:** Demo e-commerce web application (front-end only, no real backend/payment)

## 3. Scope

### In Scope
- Login / Authentication
- Product listing and sorting
- Add to cart / Remove from cart
- Checkout information form validation
- Order overview and confirmation

### Out of Scope
- Real payment processing (mocked in this app)
- Backend/API testing (no public API available for this app)
- Performance/load testing (beyond basic UX observation)

## 4. Test Approach
- **Manual functional testing** using positive, negative, and boundary test cases
- **Exploratory testing** using SauceDemo's built-in test user personas to surface intentional defects
- Test case design based on equivalence partitioning and boundary value analysis for form fields

## 5. Test Environment
- **Browser(s):** Chrome (primary), Firefox (secondary, optional)
- **OS:** Windows / macOS
- **Device:** Desktop

## 6. Test Data — User Personas
| Username | Password | Purpose |
|----------|----------|---------|
| standard_user | secret_sauce | Baseline — expected fully functional |
| locked_out_user | secret_sauce | Verify account lockout handling |
| problem_user | secret_sauce | Known to contain UI/functional defects |
| performance_glitch_user | secret_sauce | Verify behavior under artificial latency |

## 7. Entry Criteria
- Application is accessible at the URL above
- Test cases are written and reviewed

## 8. Exit Criteria
- All planned test cases executed
- All identified defects logged with severity/priority
- Critical/blocker defects reported and documented

## 9. Deliverables
- Test case documents (`/test-cases`)
- Bug reports with evidence (`/bug-reports`, `/screenshots`)
- Summary of findings (see README.md)

## 10. Risks / Assumptions
- SauceDemo is a public demo app with intentionally seeded bugs for QA training — some "defects" are by design and used here for practice purposes
- No real backend means data does not persist between sessions
