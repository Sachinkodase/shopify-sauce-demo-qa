# Requirement Traceability Matrix (RTM)

| Field | Details |
|--------|---------|
| **Project Name** | Shopify Sauce Demo |
| **Document** | Requirement Traceability Matrix (RTM) |
| **Version** | 1.0 |
| **Prepared By** | Sachin |
| **Prepared Date** | YYYY-MM-DD |
| **Document Status** | Final |

---

## 1. Purpose

The Requirement Traceability Matrix (RTM) establishes traceability between functional requirements and their corresponding test cases. It ensures complete test coverage, verifies that every requirement has been tested, and helps identify any missing or redundant test cases.

---

## 2. Scope

This RTM covers all functional requirements for the Shopify Sauce Demo application, including:

- Homepage
- Product
- Cart
- Checkout
- Search
- Navigation
- Responsive Design

---

## 3. Requirement Traceability Matrix

| Requirement ID | Requirement Description | Module | Test Case(s) | Status |
|----------------|-------------------------|--------|--------------|--------|
| REQ_HOME_001 | Homepage loads successfully | Homepage | TC_HOME_001 | ✅ Covered |
| REQ_HOME_002 | Homepage content is displayed correctly | Homepage | TC_HOME_002 – TC_HOME_017 | ✅ Covered |
| REQ_PROD_001 | Display product listing | Product | TC_PROD_001 | ✅ Covered |
| REQ_PROD_002 | Display product information | Product | TC_PROD_002 – TC_PROD_005 | ✅ Covered |
| REQ_PROD_003 | Add and remove products from cart | Product | TC_PROD_006 – TC_PROD_009 | ✅ Covered |
| REQ_PROD_004 | Sort products | Product | TC_PROD_010 – TC_PROD_011 | ✅ Covered |
| REQ_PROD_005 | Validate product information and availability | Product | TC_PROD_012 – TC_PROD_017 | ✅ Covered |
| REQ_CART_001 | Display cart page | Cart | TC_CART_001 | ✅ Covered |
| REQ_CART_002 | Display selected products | Cart | TC_CART_002 – TC_CART_003 | ✅ Covered |
| REQ_CART_003 | Remove products from cart | Cart | TC_CART_004 | ✅ Covered |
| REQ_CART_004 | Display cart quantity and totals | Cart | TC_CART_005 – TC_CART_010 | ✅ Covered |
| REQ_CART_005 | Proceed to checkout | Cart | TC_CART_011 – TC_CART_017 | ✅ Covered |
| REQ_CHECKOUT_001 | Enter checkout information | Checkout | TC_CHECKOUT_001 – TC_CHECKOUT_006 | ✅ Covered |
| REQ_CHECKOUT_002 | Display checkout overview | Checkout | TC_CHECKOUT_007 – TC_CHECKOUT_010 | ✅ Covered |
| REQ_CHECKOUT_003 | Complete checkout successfully | Checkout | TC_CHECKOUT_011 – TC_CHECKOUT_017 | ✅ Covered |
| REQ_SEARCH_001 | Search for products | Search | TC_SEARCH_001 – TC_SEARCH_004 | ✅ Covered |
| REQ_SEARCH_002 | Validate search input and results | Search | TC_SEARCH_005 – TC_SEARCH_009 | ✅ Covered |
| REQ_SEARCH_003 | Maintain search performance and stability | Search | TC_SEARCH_010 – TC_SEARCH_017 | ✅ Covered |
| REQ_NAV_001 | Navigate using menu links | Navigation | TC_NAV_001 – TC_NAV_003 | ✅ Covered |
| REQ_NAV_002 | Browser navigation | Navigation | TC_NAV_004 – TC_NAV_006 | ✅ Covered |
| REQ_NAV_003 | Maintain navigation consistency | Navigation | TC_NAV_007 – TC_NAV_013 | ✅ Covered |
| REQ_NAV_004 | Keyboard accessibility | Navigation | TC_NAV_014 | ✅ Covered |
| REQ_NAV_005 | Responsive navigation | Navigation | TC_NAV_015 – TC_NAV_017 | ✅ Covered |
| REQ_RESP_001 | Desktop responsiveness | Responsive | TC_RESP_001 | ✅ Covered |
| REQ_RESP_002 | Tablet responsiveness | Responsive | TC_RESP_002 | ✅ Covered |
| REQ_RESP_003 | Mobile responsiveness | Responsive | TC_RESP_003 | ✅ Covered |
| REQ_RESP_004 | Responsive navigation | Responsive | TC_RESP_004 | ✅ Covered |
| REQ_RESP_005 | Responsive product layout | Responsive | TC_RESP_005 – TC_RESP_006 | ✅ Covered |
| REQ_RESP_006 | Responsive cart and checkout | Responsive | TC_RESP_007 – TC_RESP_008 | ✅ Covered |
| REQ_RESP_007 | Responsive UI elements | Responsive | TC_RESP_009 – TC_RESP_015 | ✅ Covered |
| REQ_RESP_008 | Responsive stability | Responsive | TC_RESP_016 – TC_RESP_017 | ✅ Covered |

---

## 4. Coverage Summary

| Module | Requirements | Test Cases | Coverage |
|---------|-------------:|-----------:|---------:|
| Homepage | 2 | 17 | 100% |
| Product | 5 | 17 | 100% |
| Cart | 5 | 17 | 100% |
| Checkout | 3 | 17 | 100% |
| Search | 3 | 17 | 100% |
| Navigation | 5 | 17 | 100% |
| Responsive | 8 | 17 | 100% |
| **Total** | **31** | **119** | **100%** |

---

## 5. Remarks

- Every identified functional requirement has been mapped to one or more test cases.
- No uncovered functional requirements were identified during testing.
- The RTM should be updated whenever new requirements or test cases are added or existing requirements change.
