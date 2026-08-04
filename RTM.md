# Requirement Traceability Matrix (RTM)

## Purpose

The Requirement Traceability Matrix (RTM) maps each functional requirement to one or more test cases to ensure complete test coverage and verify that every requirement has been tested.

| Requirement ID | Requirement Description | Test Case ID | Status |
|----------------|-------------------------|--------------|--------|
| FR-001 | User should be able to log in using valid credentials. | TC_LOGIN_001 | Pass |
| FR-002 | User should not be able to log in using invalid credentials. | TC_LOGIN_002, TC_LOGIN_003 | Pass |
| FR-003 | User should be able to view the product inventory. | TC_CART_001 | Pass |
| FR-004 | User should be able to add products to the shopping cart. | TC_CART_001, TC_CART_002 | Pass |
| FR-005 | User should be able to remove products from the shopping cart. | TC_CART_003, TC_CART_004 | Pass |
| FR-006 | User should be able to complete the checkout process. | TC_CHECKOUT_001 | Pass |
| FR-007 | The application should validate mandatory checkout fields. | TC_CHECKOUT_002, TC_CHECKOUT_003, TC_CHECKOUT_004 | Pass |
| FR-008 | The application should display an order confirmation after a successful checkout. | TC_CHECKOUT_008, TC_CHECKOUT_009 | Pass |

## Summary

- Total Functional Requirements: **8**
- Total Test Cases Mapped: **25**
- Requirements Covered: **100%**
- Uncovered Requirements: **0**
