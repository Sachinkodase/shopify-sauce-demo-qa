# Product Test Cases

## Purpose

This document contains the functional test cases for the Product module of the Shopify Sauce Demo application.

## Scope

The Product module includes testing of:

- Product listing
- Product information
- Product images
- Product pricing
- Product availability
- Add to Cart functionality
- Remove from Cart functionality
- Product sorting
- Product detail page

- ---

## Test Case Summary

| Module | Total Test Cases | Status |
|---------|-----------------:|--------|
| Product | 17 | ✅ Completed |

---

## Test Cases

### TC_PROD_001 – Verify Product Listing Page Loads Successfully

| Field | Details |
|--------|---------|
| **Test Case ID** | TC_PROD_001 |
| **Module** | Product |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User opens the Shopify Sauce Demo application. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Shopify Sauce Demo application. | Homepage loads successfully. |
| 2 | Navigate to the product listing page (if not the default page). | Product listing page is displayed without errors. |
| 3 | Observe the products displayed on the page. | All available products are visible with their information. |

#### Expected Result

The product listing page loads successfully and displays all available products without any missing or broken content.

### TC_PROD_002 – Verify Product Name is Displayed

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_002 |
| **Module** | Product |
| **Requirement** | Product Information |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed successfully. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Observe each product card. | Each product displays a product name. |
| 3 | Verify the product names are readable and not truncated unexpectedly. | Product names are clearly visible and correctly displayed. |

#### Expected Result

Every product displayed on the Product page has a visible and correctly formatted product name.

### TC_PROD_003 – Verify Product Price is Displayed

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_003 |
| **Module** | Product |
| **Requirement** | Product Pricing |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed successfully. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Observe the price displayed for each product. | Every product has a visible price. |
| 3 | Verify the price format. | Prices are displayed in the correct currency and format (e.g., ₹99.00 or $99.00). |

#### Expected Result

Every product displays a valid price in the correct format without missing or incorrect values.

### TC_PROD_004 – Verify Product Image is Displayed

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_004 |
| **Module** | Product |
| **Requirement** | Product Images |
| **Priority** | High |
| **Type** | Functional / UI |
| **Precondition** | Product listing page is displayed successfully. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Observe each product card. | Every product displays an image. |
| 3 | Verify the images load correctly. | Images are displayed without distortion, broken links, or placeholders. |

#### Expected Result

Every product displays the correct image, and all images load successfully without any visual defects.

### TC_PROD_005 – Verify Product Detail Page Opens Successfully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_005 |
| **Module** | Product |
| **Requirement** | Product Detail Page |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed successfully. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Click on any product name or product image. | The Product Detail page opens successfully. |
| 3 | Verify the product information on the detail page. | The product name, image, price, and description are displayed correctly. |

#### Expected Result

The Product Detail page opens successfully and displays the complete information for the selected product.

### TC_PROD_006 – Verify Add to Cart Button is Displayed

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_006 |
| **Module** | Product |
| **Requirement** | Add to Cart |
| **Priority** | High |
| **Type** | Functional / UI |
| **Precondition** | Product listing page is displayed successfully. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Observe each product card. | An **Add to Cart** button is displayed for each available product. |
| 3 | Verify the button is enabled and clickable. | The **Add to Cart** button is active and ready for interaction. |

#### Expected Result

Every available product displays an enabled **Add to Cart** button.

### TC_PROD_007 – Verify Product Can Be Added to Cart

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_007 |
| **Module** | Product |
| **Requirement** | Add to Cart |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed and the product is available for purchase. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Click the **Add to Cart** button for any product. | The selected product is added to the shopping cart. |
| 3 | Verify the button label changes. | The **Add to Cart** button changes to **Remove**. |
| 4 | Verify the cart icon. | The cart icon updates to reflect the added item. |

#### Expected Result

The selected product is successfully added to the shopping cart, the button changes to **Remove**, and the cart icon is updated accordingly.

### TC_PROD_008 – Verify Product Can Be Removed from Cart

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_008 |
| **Module** | Product |
| **Requirement** | Remove from Cart |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | A product has been added to the shopping cart. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Click the **Remove** button for a product already added to the cart. | The product is removed from the shopping cart. |
| 3 | Verify the button label changes. | The **Remove** button changes back to **Add to Cart**. |
| 4 | Verify the cart icon. | The cart icon updates to reflect the removed item. |

#### Expected Result

The selected product is successfully removed from the shopping cart, the button changes back to **Add to Cart**, and the cart icon is updated accordingly.

### TC_PROD_009 – Verify Multiple Products Can Be Added to Cart

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_009 |
| **Module** | Product |
| **Requirement** | Add to Cart |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed and multiple products are available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Click the **Add to Cart** button for multiple products. | Each selected product is added to the shopping cart. |
| 3 | Verify the cart icon. | The cart icon displays the correct number of added products. |
| 4 | Verify the button labels. | The selected products display the **Remove** button. |

#### Expected Result

Multiple products are successfully added to the shopping cart, the cart icon displays the correct item count, and the selected products display the **Remove** button.

### TC_PROD_010 – Verify Product Sorting Functionality

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_010 |
| **Module** | Product |
| **Requirement** | Product Sorting |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed and the sorting option is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Select a sorting option (e.g., Price: Low to High or Name: A to Z). | The selected sorting option is applied. |
| 3 | Verify the order of the displayed products. | Products are displayed according to the selected sorting option. |

#### Expected Result

Products are sorted correctly based on the selected sorting option.

### TC_PROD_011 – Verify Product Sorting Persists Until Changed

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_011 |
| **Module** | Product |
| **Requirement** | Product Sorting |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed and a sorting option has been selected. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Select a sorting option (e.g., Name: Z to A). | Products are sorted according to the selected option. |
| 3 | Refresh the page or continue browsing within the Product page. | The selected sorting option remains applied until the user changes it. |

#### Expected Result

The selected sorting option remains active until the user selects a different sorting option.

### TC_PROD_012 – Verify Product Availability Status

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_012 |
| **Module** | Product |
| **Requirement** | Product Availability |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed successfully. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Review the products displayed on the page. | Products that are available for purchase are displayed correctly. |
| 3 | Verify that available products can be selected and added to the cart. | Available products can be interacted with and added to the shopping cart successfully. |

#### Expected Result

Available products are displayed correctly and can be successfully added to the shopping cart.

### TC_PROD_013 – Verify Product Description is Displayed

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_013 |
| **Module** | Product |
| **Requirement** | Product Information |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed successfully. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Review the product cards or open a product detail page (if applicable). | The product description is visible. |
| 3 | Verify the description is readable and matches the corresponding product. | The correct description is displayed without truncation or formatting issues. |

#### Expected Result

Each product displays the correct description in a clear and readable format.

### TC_PROD_014 – Verify Product Information Remains Consistent Between Listing and Detail Page

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_014 |
| **Module** | Product |
| **Requirement** | Product Information |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Product listing page is displayed successfully. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed. |
| 2 | Note the product name, price, image, and description for any product. | Product information is visible on the listing page. |
| 3 | Open the selected product's detail page. | The Product Detail page is displayed. |
| 4 | Compare the product information on both pages. | The product name, price, image, and description match on both the listing and detail pages. |

#### Expected Result

The product information remains consistent between the Product Listing page and the Product Detail page.

### TC_PROD_015 – Verify Product Page Handles Large Number of Products Correctly

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_015 |
| **Module** | Product |
| **Requirement** | Product Listing |
| **Priority** | Low |
| **Type** | Functional / Performance |
| **Precondition** | Product listing page contains multiple products. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | Product listing page is displayed successfully. |
| 2 | Scroll through the complete list of products. | All products load and are displayed correctly. |
| 3 | Verify the page remains responsive while browsing the products. | Scrolling and interaction remain smooth without errors or missing products. |

#### Expected Result

The Product page displays all available products correctly and remains responsive while users browse the product list.

### TC_PROD_016 – Verify Product Page Displays Appropriate Message When No Products Are Available

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_016 |
| **Module** | Product |
| **Requirement** | Product Listing |
| **Priority** | Low |
| **Type** | Negative / Functional |
| **Precondition** | No products are available in the product catalog. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page when no products are available. | The Product page loads successfully. |
| 2 | Observe the product listing area. | No products are displayed. |
| 3 | Verify the page behavior. | A clear and user-friendly message is displayed indicating that no products are available. |

#### Expected Result

When no products are available, the application displays an appropriate message instead of showing a blank page or errors.

### TC_PROD_017 – Verify Product Page Handles Invalid Product URL Gracefully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_PROD_017 |
| **Module** | Product |
| **Requirement** | Product Detail Page |
| **Priority** | Medium |
| **Type** | Negative / Functional |
| **Precondition** | User has access to the application. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter an invalid or non-existent product URL in the browser address bar. | The application attempts to load the requested page. |
| 2 | Observe the application's response. | An appropriate error page or "Product Not Found" message is displayed. |
| 3 | Verify the application remains functional. | The user can navigate to other pages without errors or application crashes. |

#### Expected Result

The application handles invalid product URLs gracefully by displaying an appropriate error message or page, without crashing or exposing system errors.








--------:|--------|
| Product | TBD | 🚧 In Progress |
