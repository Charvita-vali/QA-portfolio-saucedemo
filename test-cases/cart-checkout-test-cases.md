# Test Cases — Cart & Checkout Module

**Application:** SauceDemo
**Modules:** Cart, Checkout
**URL:** https://www.saucedemo.com
**Preconditions for all cases:** User is logged in with `standard_user` / `secret_sauce` unless otherwise noted

## Cart Module

| ID | Title | Steps | Expected Result | Priority | Status |
|----|-------|-------|------------------|----------|--------|
| TC_CART_01 | Add single item to cart | 1. Click "Add to cart" on one product | Cart icon shows count = 1 | High | |
| TC_CART_02 | Add multiple items | 1. Add 3 different products to cart | Cart icon shows count = 3 | High | |
| TC_CART_03 | Remove item from product page | 1. Add item<br>2. Click "Remove" on same product | Cart count decreases by 1 | High | |
| TC_CART_04 | Remove item from cart page | 1. Add item<br>2. Go to cart<br>3. Click "Remove" | Item disappears from cart list, count updates | High | |
| TC_CART_05 | Cart persists after navigation | 1. Add item<br>2. Navigate to another page<br>3. Return to Products | Cart count remains unchanged | Medium | |
| TC_CART_06 | Empty cart checkout attempt | 1. Go to cart with 0 items<br>2. Click Checkout | Should block or show empty checkout appropriately | Medium | |
| TC_CART_07 | Continue shopping button | 1. On cart page, click "Continue Shopping" | Returns to Products page, cart retains items | Low | |
| TC_CART_08 | Cart badge visual (problem_user) | 1. Login as `problem_user`<br>2. Add items | Cart badge/count should display correctly (known buggy user) | Medium | |

## Checkout Module

| ID | Title | Steps | Expected Result | Priority | Status |
|----|-------|-------|------------------|----------|--------|
| TC_CHK_01 | Valid checkout info | 1. Add item → Checkout<br>2. Fill First Name, Last Name, Zip<br>3. Click Continue | Proceeds to Overview page | High | |
| TC_CHK_02 | Missing first name | 1. Leave First Name blank, fill rest<br>2. Click Continue | Error: "First Name is required" | High | |
| TC_CHK_03 | Missing last name | 1. Leave Last Name blank, fill rest<br>2. Click Continue | Error: "Last Name is required" | High | |
| TC_CHK_04 | Missing zip/postal code | 1. Leave Zip blank, fill rest<br>2. Click Continue | Error: "Postal Code is required" | High | |
| TC_CHK_05 | Cancel checkout | 1. On checkout info page, click Cancel | Returns to Cart page, items retained | Medium | |
| TC_CHK_06 | Order summary accuracy | 1. Complete checkout to Overview page | Item total + tax = correct total displayed | High | |
| TC_CHK_07 | Finish order | 1. On Overview page, click Finish | "Thank You" confirmation page shown, cart emptied | High | |
| TC_CHK_08 | Cart empties after order | 1. Complete an order<br>2. Check cart icon | Cart count = 0 | Medium | |
| TC_CHK_09 | Back button after order | 1. Complete order<br>2. Click "Back Home" | Returns to Products page | Low | |
| TC_CHK_10 | Special characters in name fields | 1. Enter `<script>alert(1)</script>` in First Name<br>2. Click Continue | Input handled safely, no script execution | Medium | |

## Notes
- TC_CHK_10 is a light XSS-awareness test, useful for demonstrating security-conscious QA thinking in interviews
- TC_CART_08 links directly to BUG-001 (see `/bug-reports`)
