# Checkout Test Cases

## Purpose

This document contains the functional test cases for the Checkout module of the Shopify Sauce Demo application.

## Scope

The Checkout module includes testing of:

- Checkout information form
- Required field validation
- Order summary
- Checkout overview
- Order completion
- Cancel checkout
- Error messages
- Checkout navigation

- ---

## Test Case Summary

| Module | Total Test Cases | Status |
|---------|-----------------:|--------|
| Checkout | 17 | ✅ Completed |

### TC_CHECKOUT_001 – Verify Checkout Information Page Loads Successfully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_001 |
| **Module** | Checkout |
| **Requirement** | Checkout Information |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has at least one product in the cart and is on the Cart page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click the **Checkout** button from the Cart page. | The application navigates to the Checkout Information page. |
| 2 | Verify the Checkout Information page is displayed. | The page loads successfully with the customer information form. |
| 3 | Verify the available input fields. | The **First Name**, **Last Name**, and **Postal Code** fields are displayed along with the **Continue** and **Cancel** buttons. |

#### Expected Result

The Checkout Information page loads successfully and displays all required input fields and action buttons.

### TC_CHECKOUT_002 – Verify User Can Enter Valid Checkout Information

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_002 |
| **Module** | Checkout |
| **Requirement** | Checkout Information |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User is on the Checkout Information page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid First Name. | The value is accepted. |
| 2 | Enter a valid Last Name. | The value is accepted. |
| 3 | Enter a valid Postal Code. | The value is accepted. |
| 4 | Click the **Continue** button. | The application navigates to the Checkout Overview page. |

#### Expected Result

The user can successfully enter valid checkout information and proceed to the Checkout Overview page.

### TC_CHECKOUT_003 – Verify Required Field Validation

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_003 |
| **Module** | Checkout |
| **Requirement** | Required Field Validation |
| **Priority** | High |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Checkout Information page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Leave the **First Name**, **Last Name**, and **Postal Code** fields empty. | All required fields remain blank. |
| 2 | Click the **Continue** button. | The application validates the input. |
| 3 | Verify the validation message. | An appropriate error message is displayed indicating that the required fields must be completed. |

#### Expected Result

The user cannot proceed to the Checkout Overview page until all required fields are completed, and an appropriate validation message is displayed.

### TC_CHECKOUT_004 – Verify Validation for Missing First Name

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_004 |
| **Module** | Checkout |
| **Requirement** | Required Field Validation |
| **Priority** | High |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Checkout Information page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Leave the **First Name** field empty. | The First Name field remains blank. |
| 2 | Enter valid values for **Last Name** and **Postal Code**. | The values are accepted. |
| 3 | Click the **Continue** button. | The application validates the input. |
| 4 | Verify the validation message. | An error message indicating that the **First Name** is required is displayed. |

#### Expected Result

The user cannot proceed to the Checkout Overview page until a valid **First Name** is entered.

### TC_CHECKOUT_005 – Verify Validation for Missing Last Name

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_005 |
| **Module** | Checkout |
| **Requirement** | Required Field Validation |
| **Priority** | High |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Checkout Information page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid **First Name**. | The value is accepted. |
| 2 | Leave the **Last Name** field empty. | The Last Name field remains blank. |
| 3 | Enter a valid **Postal Code**. | The value is accepted. |
| 4 | Click the **Continue** button. | The application validates the input. |
| 5 | Verify the validation message. | An error message indicating that the **Last Name** is required is displayed. |

#### Expected Result

The user cannot proceed to the Checkout Overview page until a valid **Last Name** is entered.

### TC_CHECKOUT_006 – Verify Validation for Missing Postal Code

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_006 |
| **Module** | Checkout |
| **Requirement** | Required Field Validation |
| **Priority** | High |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Checkout Information page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid **First Name**. | The value is accepted. |
| 2 | Enter a valid **Last Name**. | The value is accepted. |
| 3 | Leave the **Postal Code** field empty. | The Postal Code field remains blank. |
| 4 | Click the **Continue** button. | The application validates the input. |
| 5 | Verify the validation message. | An error message indicating that the **Postal Code** is required is displayed. |

#### Expected Result

The user cannot proceed to the Checkout Overview page until a valid **Postal Code** is entered.

### TC_CHECKOUT_007 – Verify Checkout Overview Page Displays Correct Order Information

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_007 |
| **Module** | Checkout |
| **Requirement** | Checkout Overview |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has entered valid checkout information and navigated to the Checkout Overview page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Complete the Checkout Information form with valid data. | The Checkout Overview page is displayed. |
| 2 | Review the products listed in the order summary. | All selected products are displayed with the correct name, quantity, and price. |
| 3 | Verify the payment, shipping, and total information. | The payment information, shipping information, subtotal, tax, and total are displayed correctly. |

#### Expected Result

The Checkout Overview page displays the correct order summary, including product details, payment information, shipping information, and total amount.

### TC_CHECKOUT_008 – Verify User Can Complete Checkout Successfully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_008 |
| **Module** | Checkout |
| **Requirement** | Order Completion |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User is on the Checkout Overview page with valid order information. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Review the order details on the Checkout Overview page. | The order information is displayed correctly. |
| 2 | Click the **Finish** button. | The checkout process is completed. |
| 3 | Verify the confirmation page. | A confirmation message indicating that the order has been placed successfully is displayed. |

#### Expected Result

The user successfully completes the checkout process and the application displays the order confirmation page.

### TC_CHECKOUT_009 – Verify Cancel Button Returns User to the Cart Page

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_009 |
| **Module** | Checkout |
| **Requirement** | Checkout Navigation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User is on the Checkout Information page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Checkout Information page. | The page is displayed successfully. |
| 2 | Click the **Cancel** button. | The application navigates back to the Cart page. |
| 3 | Verify the Cart page contents. | The previously added products are still displayed in the cart. |

#### Expected Result

Clicking the **Cancel** button returns the user to the Cart page without removing the products from the cart.

### TC_CHECKOUT_010 – Verify Order Summary Displays Correct Total Amount

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_010 |
| **Module** | Checkout |
| **Requirement** | Order Summary |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User is on the Checkout Overview page with one or more products in the order. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Complete the Checkout Information form with valid details. | The Checkout Overview page is displayed. |
| 2 | Review the order summary. | The subtotal, tax, and total amount are displayed. |
| 3 | Verify the total amount. | The total amount equals the subtotal plus the applicable tax. |

#### Expected Result

The Checkout Overview page displays the correct subtotal, tax, and final total for the order.

### TC_CHECKOUT_011 – Verify User Cannot Complete Checkout with Invalid Information

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_011 |
| **Module** | Checkout |
| **Requirement** | Input Validation |
| **Priority** | High |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Checkout Information page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter invalid or incomplete information in one or more required fields. | The invalid data is entered. |
| 2 | Click the **Continue** button. | The application validates the input. |
| 3 | Verify the application's response. | The user remains on the Checkout Information page and an appropriate validation error message is displayed. |

#### Expected Result

The application prevents the user from proceeding to the Checkout Overview page until valid checkout information is provided.

### TC_CHECKOUT_012 – Verify Checkout Overview Displays Correct Product Details

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_012 |
| **Module** | Checkout |
| **Requirement** | Checkout Overview |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has entered valid checkout information and is on the Checkout Overview page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to the Checkout Overview page after entering valid checkout information. | The Checkout Overview page is displayed. |
| 2 | Review the products listed in the order summary. | Each product displays the correct name, description, quantity, and price. |
| 3 | Compare the displayed product details with the products added to the cart. | The product details match exactly with the selected cart items. |

#### Expected Result

The Checkout Overview page displays the correct product details for all items included in the order.

### TC_CHECKOUT_013 – Verify User Can Return to Product Page After Order Completion

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_013 |
| **Module** | Checkout |
| **Requirement** | Order Completion |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has successfully completed the checkout process and is on the order confirmation page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Complete the checkout process. | The order confirmation page is displayed. |
| 2 | Click the **Back Home** button. | The application navigates to the Product page. |
| 3 | Verify the Product page is displayed. | The Product page loads successfully and the user can continue browsing products. |

#### Expected Result

After completing an order, the user can successfully return to the Product page by clicking the **Back Home** button.

### TC_CHECKOUT_014 – Verify Checkout Can Be Cancelled from the Overview Page

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_014 |
| **Module** | Checkout |
| **Requirement** | Checkout Navigation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has entered valid checkout information and is on the Checkout Overview page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to the Checkout Overview page. | The Checkout Overview page is displayed. |
| 2 | Click the **Cancel** button. | The application navigates back to the Product page. |
| 3 | Verify the Product page is displayed. | The Product page loads successfully and the user can continue shopping. |

#### Expected Result

Clicking the **Cancel** button on the Checkout Overview page returns the user to the Product page without causing any application errors.

### TC_CHECKOUT_015 – Verify Checkout Confirmation Page Displays Success Message

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_015 |
| **Module** | Checkout |
| **Requirement** | Order Confirmation |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has successfully completed the checkout process. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Complete the checkout process by clicking the **Finish** button. | The Checkout Complete page is displayed. |
| 2 | Observe the confirmation section. | A success message confirming the order completion is displayed. |
| 3 | Verify the confirmation page contents. | The confirmation icon, thank-you message, and completion text are displayed correctly. |

#### Expected Result

The Checkout Confirmation page displays a clear success message confirming that the order has been completed successfully.

### TC_CHECKOUT_016 – Verify Checkout Overview Displays Correct Tax Calculation

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_016 |
| **Module** | Checkout |
| **Requirement** | Order Summary |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has entered valid checkout information and is on the Checkout Overview page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to the Checkout Overview page with one or more products in the order. | The Checkout Overview page is displayed. |
| 2 | Review the subtotal, tax, and total values. | The subtotal, tax, and total are visible. |
| 3 | Verify the tax calculation. | The displayed tax is calculated correctly according to the application's business rules, and the total equals the subtotal plus tax. |

#### Expected Result

The Checkout Overview page displays the correct tax amount, and the final total is calculated accurately.

### TC_CHECKOUT_017 – Verify Checkout Process Handles Direct Access to Confirmation Page Gracefully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_CHECKOUT_017 |
| **Module** | Checkout |
| **Requirement** | Checkout Navigation |
| **Priority** | Medium |
| **Type** | Functional / Negative |
| **Precondition** | User has not completed the checkout process. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Attempt to access the Checkout Confirmation page directly using its URL. | The application processes the request. |
| 2 | Observe the application's response. | The user is redirected to the appropriate page (such as the Product or Cart page) or shown an appropriate message. |
| 3 | Verify the application remains stable. | No application errors or unexpected behavior occur. |

#### Expected Result

The application prevents unauthorized direct access to the Checkout Confirmation page and handles the request gracefully without displaying errors.






