# BUG-001: Product images display incorrect image for all products when logged in as problem_user

## Environment
- **URL:** https://www.saucedemo.com
- **Browser:** Chrome (fill in your version)
- **OS:** (fill in yours)
- **User:** problem_user

## Preconditions
- User has valid `problem_user` credentials

## Steps to Reproduce
1. Navigate to https://www.saucedemo.com
2. Log in with username: `problem_user`, password: `secret_sauce`
3. Observe the Products (Inventory) page
4. Compare product images against product names/descriptions

## Expected Result
Each product should display its own unique, correct image matching its name and description (e.g., "Sauce Labs Backpack" shows a backpack image).

## Actual Result
All products display the same incorrect image (a photo of a dog) regardless of the actual product name or description.

## Severity
**Medium** — This is a visual/data-integrity bug. It doesn't block core functionality like checkout, but it misrepresents products to the user, which matters significantly for an e-commerce application.

## Priority
**High** — Should be fixed soon since it directly affects what customers see and could damage trust/conversion.

## Attachments
- `screenshots/bug001_dog_images.png` — Products page as problem_user, showing dog image for all items
- `screenshots/bug001_standard_user_correct.png` — Products page as standard_user, for comparison, showing correct distinct images

## Additional Notes
Bug does not reproduce with `standard_user`, confirming this is specific to `problem_user`'s test data/mock configuration rather than an application-wide regression.
