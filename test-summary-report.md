# Test Summary Report

## Project Information

**Project:** SauceDemo E-Commerce Application  
**Testing Type:** Manual Functional Testing & Exploratory Testing  
**Browser:** Google Chrome  
**Environment:** Desktop (Windows/macOS)

---

## Modules Tested

- Login
- Cart
- Checkout

---

## Test Execution Summary

| Metric | Result |
|--------|--------|
| Total Test Cases Designed | 25 |
| Total Test Cases Executed | 25 |
| Passed | 25 |
| Failed | 0 |
| Blocked | 0 |
| Exploratory Defects Found | 2 |

---

## Defect Summary

| Bug ID | Severity | Priority | Status |
|--------|----------|----------|--------|
| BUG-001 | Medium | High | Open |
| BUG-002 | Critical | Critical | Open |

---

## Test Conclusion

All 25 planned manual test cases were executed successfully using the **standard_user** account.

To improve test coverage, exploratory testing was performed using the **problem_user** account, which led to the discovery of two reproducible defects.

The testing confirmed that the primary business workflows function as expected for the standard user. However, due to the critical checkout defect affecting the **problem_user** account, the application requires defect resolution before being considered fully stable for all supported user types.

---

## Recommendation

The application is functionally stable for the normal user workflow. However, the identified critical checkout defect should be resolved and retested before release for all user scenarios.
