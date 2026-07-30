# Test Data

| Field | Details |
|--------|---------|
| **Project Name** | Shopify Sauce Demo |
| **Document** | Test Data |
| **Version** | 1.0 |
| **Prepared By** | Sachin |
| **Prepared Date** | YYYY-MM-DD |
| **Document Status** | Final |

---

## 1. Purpose

This document contains the test data used during manual functional testing of the Shopify Sauce Demo application. It includes valid and invalid input values used to verify application behavior under different test scenarios.

---

## 2. Valid Customer Information

| Field | Test Data |
|------|-----------|
| First Name | John |
| Last Name | Doe |
| Postal Code | 10001 |

---

## 3. Invalid Customer Information

| Test Scenario | Test Data |
|--------------|-----------|
| Empty First Name | *(blank)* |
| Empty Last Name | *(blank)* |
| Empty Postal Code | *(blank)* |
| Numeric First Name | 12345 |
| Numeric Last Name | 98765 |
| Special Characters | @#$%^ |
| Long First Name | ABCDEFGHIJKLMNOPQRSTUVWXYZABCDEFGHIJKLMN |

---

## 4. Product Test Data

| Product Name |
|--------------|
| Sauce Backpack |
| Sauce Bike Light |
| Sauce Bolt T-Shirt |
| Sauce Fleece Jacket |
| Sauce Onesie |
| Sauce Labs T-Shirt |

---

## 5. Search Test Data

| Test Scenario | Search Value |
|--------------|--------------|
| Valid Product | Backpack |
| Partial Product Name | Back |
| Lowercase Search | backpack |
| Uppercase Search | BACKPACK |
| Invalid Product | Laptop |
| Numeric Search | 12345 |
| Special Characters | @@@@ |
| Empty Search | *(blank)* |

---

## 6. Cart Test Data

| Scenario | Test Data |
|----------|-----------|
| Single Product | Sauce Backpack |
| Multiple Products | Backpack, Bike Light, Onesie |
| Empty Cart | No Products |
| Remove Product | Remove Sauce Backpack |

---

## 7. Checkout Test Data

| Field | Valid Value | Invalid Value |
|------|-------------|---------------|
| First Name | John | *(blank)* |
| Last Name | Doe | *(blank)* |
| Postal Code | 10001 | *(blank)* |

---

## 8. Browser and Environment

| Item | Details |
|------|---------|
| Browser | Google Chrome (Latest) |
| Operating System | Windows 11 |
| Device | Desktop/Laptop |
| Screen Resolution | 1920 × 1080 |
| Network | Stable Internet Connection |

---

## 9. Boundary and Negative Test Data

| Test Type | Test Data |
|-----------|-----------|
| Empty Input | *(blank)* |
| Numeric Input | 12345 |
| Alphabetic Input | ABCDE |
| Special Characters | !@#$%^&* |
| Long String | ABCDEFGHIJKLMNOPQRSTUVWXYZABCDEFGHIJKLMNOPQRSTUVWXYZABCDEFGHIJKLMNOPQRSTUVWXYZ |
| Spaces Only | `"     "` |

---

## 10. Remarks

- Test data was selected to cover both positive and negative test scenarios.
- Valid data was used to verify expected application behavior.
- Invalid and boundary value data was used to validate input handling and error messages.
- Test data may be updated if application functionality or business requirements change.
