# Homepage Test Cases

## Project Information

**Module:** Homepage

**Application:** Shopify Sauce Demo

**Website:** https://sauce-demo.myshopify.com/

## Test Cases

| TestCase ID | Test Scenario | Test Case | Preconditions | Test Steps | Test Data | Expected Result | Priority | Status |
|--------------|---------------|-----------|---------------|------------|-----------|-----------------|----------|--------|

| TC_HP_001 | Verify homepage loads successfully | Verify that the homepage loads without any errors when the user accesses the website. | User has a stable internet connection. | 1. Open a web browser.<br>2. Navigate to https://sauce-demo.myshopify.com/.<br>3. Press Enter. | Website URL | Homepage loads successfully and displays the header, product section, and footer without any errors. | High | Not Executed |

| TC_HP_002 | Verify company logo is displayed | Verify that the company logo is visible on the homepage. | Homepage is loaded successfully. | 1. Open the homepage.<br>2. Observe the header section. | N/A | The company logo is displayed correctly in the header without distortion. | High | Not Executed |

| TC_HP_003 | Verify navigation menu is displayed | Verify that the navigation menu is visible and accessible on the homepage. | Homepage is loaded successfully. | 1. Open the homepage.<br>2. Observe the top navigation menu. | N/A | Navigation menu is visible and all menu options are displayed correctly. | High | Not Executed |

| TC_HP_004 | Verify product cards are displayed | Verify that product cards are displayed with all required information. | Homepage is loaded successfully. | 1. Open the homepage.<br>2. Scroll to the product section.<br>3. Observe the product cards. | N/A | Each product card displays the product image, product name, price, and Add to Cart button. | High | Not Executed |

| TC_HP_005 | Verify product images are displayed | Verify that every product card displays the correct product image. | Homepage is loaded successfully. | 1. Open the homepage.<br>2. Scroll to the product section.<br>3. Verify each product image is displayed. | N/A | Every product card displays a clear and correctly aligned product image without broken or missing images. | High | Not Executed |

| TC_HP_006 | Verify product names are displayed | Verify that every product card displays the product name correctly. | Homepage is loaded successfully. | 1. Open the homepage.<br>2. Scroll to the product section.<br>3. Verify the product name on each card. | N/A | Every product card displays the correct product name without truncation or missing text. | High | Not Executed |

| TC_HP_007 | Verify product prices are displayed | Verify that every product card displays the correct product price. | Homepage is loaded successfully. | 1. Open the homepage.<br>2. Scroll to the product section.<br>3. Verify the price displayed on each product card. | N/A | Every product card displays a valid price in the correct currency and format. | High | Not Executed |

| TC_HP_008 | Verify Add to Cart button is displayed | Verify that every product card displays an Add to Cart button. | Homepage is loaded successfully. | 1. Open the homepage.<br>2. Scroll to the product section.<br>3. Verify the Add to Cart button for each product. | N/A | Every product card displays an enabled and clearly visible Add to Cart button. | High | Not Executed |

| TC_HP_009 | Verify Add to Cart button functionality | Verify that clicking the Add to Cart button adds the selected product to the shopping cart. | Homepage is loaded successfully. | 1. Open the homepage.<br>2. Click the Add to Cart button for any product.<br>3. Observe the cart icon. | Any available product | The selected product is added to the shopping cart and the cart count is updated. | High | Not Executed |

| TC_HP_010 | Verify cart icon navigation | Verify that clicking the cart icon navigates the user to the shopping cart page. | At least one product is added to the cart. | 1. Add a product to the cart.<br>2. Click the cart icon. | Any available product | The shopping cart page opens and displays the added product(s). | High | Not Executed |






