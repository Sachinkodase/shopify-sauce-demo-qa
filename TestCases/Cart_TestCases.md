# Cart Test Cases

## Purpose

This document contains the functional test cases for the Cart module of the Shopify Sauce Demo application.

## Scope

The Cart module includes testing of:

- Add items to cart
- Remove items from cart
- Update cart contents
- Cart item quantity
- Cart total calculation
- Continue shopping
- Proceed to checkout
- Empty cart behavior

- ---

## Test Case Summary

| Module | Total Test Cases | Status |
|---------|-----------------:|--------|
| Cart | 17 | ✅ Completed |

### TC_CART_001 – Verify Cart Page Loads Successfully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_001 |
| **Module** | Cart |
| **Requirement** | Cart Page |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has at least one product added to the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add a product to the cart. | The product is added successfully. |
| 2 | Click the cart icon. | The Cart page opens successfully. |
| 3 | Verify the Cart page contents. | The selected product is displayed in the cart with its details. |

#### Expected Result

The Cart page loads successfully and displays the products added by the user.

### TC_CART_002 – Verify Added Product is Displayed in the Cart

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_002 |
| **Module** | Cart |
| **Requirement** | Cart Items |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has added at least one product to the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add a product to the cart. | The product is added successfully. |
| 2 | Open the Cart page. | The Cart page is displayed. |
| 3 | Verify the product details in the cart. | The correct product name, image, price, and quantity are displayed. |

#### Expected Result

The product added to the cart is displayed with the correct details.

### TC_CART_003 – Verify Multiple Products Are Displayed in the Cart

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_003 |
| **Module** | Cart |
| **Requirement** | Cart Items |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has added multiple products to the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add two or more products to the cart. | All selected products are added successfully. |
| 2 | Open the Cart page. | The Cart page is displayed. |
| 3 | Verify the products listed in the cart. | All added products are displayed with the correct name, price, and quantity. |

#### Expected Result

All products added by the user are displayed correctly in the Cart with accurate details.

### TC_CART_004 – Verify Product Can Be Removed from the Cart

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_004 |
| **Module** | Cart |
| **Requirement** | Remove Cart Item |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has at least one product in the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Cart page. | The Cart page is displayed. |
| 2 | Click the **Remove** button for a product. | The selected product is removed from the cart. |
| 3 | Verify the cart contents. | The removed product no longer appears in the cart. |

#### Expected Result

The selected product is successfully removed from the cart, and the cart is updated accordingly.

### TC_CART_005 – Verify Cart Item Quantity is Displayed Correctly

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_005 |
| **Module** | Cart |
| **Requirement** | Cart Item Quantity |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has added one or more products to the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add one or more products to the cart. | Products are added successfully. |
| 2 | Open the Cart page. | The Cart page is displayed. |
| 3 | Verify the quantity shown for each product. | The quantity displayed matches the number of items added for each product. |

#### Expected Result

The quantity displayed for each cart item is accurate and reflects the user's selected items.

### TC_CART_006 – Verify Continue Shopping Button Navigates to the Product Page

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_006 |
| **Module** | Cart |
| **Requirement** | Continue Shopping |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User is on the Cart page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Cart page. | The Cart page is displayed. |
| 2 | Click the **Continue Shopping** button. | The application navigates to the Product page. |
| 3 | Verify the Product page is displayed. | The Product page loads successfully and the user can continue shopping. |

#### Expected Result

Clicking the **Continue Shopping** button redirects the user to the Product page successfully.

### TC_CART_007 – Verify Checkout Button Navigates to the Checkout Information Page

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_007 |
| **Module** | Cart |
| **Requirement** | Checkout Navigation |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has at least one product in the cart and is on the Cart page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Cart page with at least one product in the cart. | The Cart page is displayed. |
| 2 | Click the **Checkout** button. | The application navigates to the Checkout Information page. |
| 3 | Verify the Checkout Information page is displayed. | Fields for customer information (e.g., First Name, Last Name, Postal Code) are visible. |

#### Expected Result

Clicking the **Checkout** button successfully navigates the user to the Checkout Information page.

### TC_CART_008 – Verify Empty Cart Displays Appropriate Message

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_008 |
| **Module** | Cart |
| **Requirement** | Empty Cart |
| **Priority** | Medium |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Cart page with no products in the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Ensure all products have been removed from the cart. | The cart contains no products. |
| 2 | Open the Cart page. | The Cart page is displayed. |
| 3 | Observe the cart contents. | The application displays an appropriate empty cart message or indicates that no items are present. |

#### Expected Result

When the cart is empty, the application clearly indicates that there are no items in the cart without displaying errors.

### TC_CART_009 – Verify Cart Contents Persist During the User Session

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_009 |
| **Module** | Cart |
| **Requirement** | Cart Persistence |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has added one or more products to the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add one or more products to the cart. | The products are added successfully. |
| 2 | Navigate to another page within the application. | Navigation completes successfully. |
| 3 | Return to the Cart page. | The previously added products are still displayed in the cart. |

#### Expected Result

Products remain in the cart while the user continues browsing the application during the same session.

### TC_CART_010 – Verify Cart Displays Correct Total Number of Items

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_010 |
| **Module** | Cart |
| **Requirement** | Cart Item Count |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has added multiple products to the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add multiple products to the cart. | Products are added successfully. |
| 2 | Observe the cart badge/icon. | The cart badge displays the correct number of items. |
| 3 | Open the Cart page and count the listed products. | The number of products displayed matches the cart badge count. |

#### Expected Result

The cart badge and the Cart page display the correct total number of items added by the user.

### TC_CART_011 – Verify Cart State Updates After Removing an Item

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_011 |
| **Module** | Cart |
| **Requirement** | Cart Update |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has multiple products in the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add two or more products to the cart. | Products are added successfully. |
| 2 | Open the Cart page. | The Cart page is displayed. |
| 3 | Remove one product from the cart. | The selected product is removed successfully. |
| 4 | Verify the remaining cart contents and cart badge. | The removed product is no longer displayed, the remaining products are unchanged, and the cart badge reflects the updated item count. |

#### Expected Result

The cart updates immediately after an item is removed, and both the cart contents and item count remain accurate.

### TC_CART_012 – Verify User Can Proceed to Checkout with Multiple Items

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_012 |
| **Module** | Cart |
| **Requirement** | Checkout Navigation |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has multiple products in the cart and is on the Cart page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add two or more products to the cart. | Products are added successfully. |
| 2 | Open the Cart page. | The Cart page is displayed with all selected products. |
| 3 | Click the **Checkout** button. | The application navigates to the Checkout Information page. |
| 4 | Verify the checkout page loads correctly. | The Checkout Information page is displayed and ready for user input. |

#### Expected Result

The user can successfully proceed to the Checkout Information page with multiple products in the cart.

### TC_CART_013 – Verify Cart Retains Items After Returning from Checkout Information Page

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_013 |
| **Module** | Cart |
| **Requirement** | Cart Persistence |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has one or more products in the cart and has navigated to the Checkout Information page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add one or more products to the cart. | Products are added successfully. |
| 2 | Open the Cart page and click **Checkout**. | The Checkout Information page is displayed. |
| 3 | Navigate back to the Cart page using the application's navigation (or Cancel button, if available). | The Cart page is displayed. |
| 4 | Verify the cart contents. | All previously added products are still present in the cart. |

#### Expected Result

The cart retains all previously added items when the user returns from the Checkout Information page without completing the checkout process.

### TC_CART_014 – Verify Cart Handles Browser Refresh Correctly

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_014 |
| **Module** | Cart |
| **Requirement** | Cart Persistence |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has one or more products in the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add one or more products to the cart. | Products are added successfully. |
| 2 | Open the Cart page. | The Cart page displays the added products. |
| 3 | Refresh the browser page. | The Cart page reloads successfully. |
| 4 | Verify the cart contents after the refresh. | All previously added products remain in the cart. |

#### Expected Result

Refreshing the browser does not remove products from the cart, and the cart contents remain unchanged.

### TC_CART_015 – Verify Cart Displays Correct Product Details After Refresh

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_015 |
| **Module** | Cart |
| **Requirement** | Cart Persistence |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has one or more products in the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Add one or more products to the cart. | Products are added successfully. |
| 2 | Open the Cart page and note the product details (name, price, and quantity). | Product details are displayed correctly. |
| 3 | Refresh the browser page. | The Cart page reloads successfully. |
| 4 | Verify the product details after the refresh. | The product name, price, and quantity remain correct and unchanged. |

#### Expected Result

After refreshing the browser, all product details remain accurate and consistent with the items previously added to the cart.

### TC_CART_016 – Verify Cart Handles Direct Access Without Items

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_016 |
| **Module** | Cart |
| **Requirement** | Empty Cart |
| **Priority** | Medium |
| **Type** | Negative / Functional |
| **Precondition** | User has no products in the cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Ensure the cart is empty. | No products are present in the cart. |
| 2 | Navigate directly to the Cart page using the application's cart URL or cart icon. | The Cart page loads successfully. |
| 3 | Verify the page contents. | The application indicates that the cart is empty and does not display any products or errors. |

#### Expected Result

The Cart page loads successfully with an empty cart and displays the appropriate empty state without any application errors.

### TC_CART_017 – Verify Cart Page Loads Without Errors

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CART_017 |
| **Module** | Cart |
| **Requirement** | Cart Page |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has access to the application. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Cart page. | The Cart page loads successfully. |
| 2 | Observe the page for any loading issues or error messages. | No errors, broken elements, or unexpected behavior are present. |
| 3 | Verify all cart page components are displayed correctly. | The cart page layout, buttons, and product section (or empty cart state) are displayed correctly. |

#### Expected Result

The Cart page loads successfully and all page elements are displayed correctly without any errors.








