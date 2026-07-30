# Bug Report Template

## Purpose

This document provides a standardized template for reporting defects identified during functional testing of the Shopify Sauce Demo application. It ensures bug reports are clear, consistent, and contain the information required for developers to reproduce and resolve issues efficiently.

## Bug Report Template

| Field | Details |
|--------|---------|
| **Bug ID** | BUG_001 |
| **Title** | Brief summary of the defect |
| **Module** | Affected module (e.g., Product, Cart, Checkout) |
| **Severity** | Critical / High / Medium / Low |
| **Priority** | High / Medium / Low |
| **Environment** | Browser, OS, Device |
| **Preconditions** | Conditions required before reproducing the bug |
| **Steps to Reproduce** | 1. Step one<br>2. Step two<br>3. Step three |
| **Expected Result** | What should happen |
| **Actual Result** | What actually happened |
| **Status** | Open / In Progress / Fixed / Closed |
| **Reported By** | Tester name |
| **Reported Date** | YYYY-MM-DD |
| **Attachments** | Screenshots, videos, or logs (if applicable) |

---

# Sample Bug Report

| Field | Details |
|--------|---------|
| **Bug ID** | BUG_001 |
| **Title** | Cart badge count does not update after removing the last product |
| **Module** | Cart |
| **Severity** | Medium |
| **Priority** | High |
| **Environment** | Google Chrome (Latest), Windows 11 |
| **Preconditions** | User has one product in the shopping cart. |
| **Steps to Reproduce** | 1. Add a product to the cart.<br>2. Open the cart.<br>3. Remove the product.<br>4. Observe the cart badge. |
| **Expected Result** | The cart badge disappears or updates to show zero items. |
| **Actual Result** | The cart badge continues to display one item even though the cart is empty. |
| **Status** | Open |
| **Reported By** | QA Tester |
| **Reported Date** | YYYY-MM-DD |
| **Attachments** | Screenshot showing the incorrect cart badge (if available). |






