# Navigation Test Cases

## Purpose

This document contains the functional test cases for the Navigation module of the Shopify Sauce Demo application.

## Scope

The Navigation module includes testing of:

- Main navigation menu
- Navigation links
- Header navigation
- Footer navigation
- Logo navigation
- Breadcrumb navigation (if applicable)
- Browser Back and Forward navigation
- Navigation consistency across pages

- ## Test Case Summary

| Module | Total Test Cases | Status |
|---------|-----------------:|--------|
| Navigation | 17 | ✅ Completed |

### TC_NAV_001 – Verify Navigation Menu Loads Successfully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_001 |
| **Module** | Navigation |
| **Requirement** | Navigation Menu |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User has opened the application. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the application. | The application loads successfully. |
| 2 | Observe the navigation menu. | The navigation menu is displayed correctly. |

#### Expected Result

The navigation menu loads successfully and is visible to the user.

---

### TC_NAV_002 – Verify Navigation Links Redirect to the Correct Pages

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_002 |
| **Module** | Navigation |
| **Requirement** | Navigation Links |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User is on the application homepage. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click each navigation link. | The selected page opens successfully. |
| 2 | Verify the page content. | The correct page is displayed. |

#### Expected Result

Each navigation link redirects to its intended page.

---

### TC_NAV_003 – Verify Logo Redirects to the Homepage

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_003 |
| **Module** | Navigation |
| **Requirement** | Logo Navigation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User is on any page other than the homepage. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click the application logo. | Homepage loads successfully. |

#### Expected Result

Clicking the logo redirects the user to the homepage.

---

### TC_NAV_004 – Verify Browser Back Button Navigation

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_004 |
| **Module** | Navigation |
| **Requirement** | Browser Navigation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has navigated through multiple pages. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click the browser Back button. | Previous page is displayed correctly. |

#### Expected Result

The browser Back button navigates to the previous page successfully.

---

### TC_NAV_005 – Verify Browser Forward Button Navigation

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_005 |
| **Module** | Navigation |
| **Requirement** | Browser Navigation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has used the browser Back button. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click the browser Forward button. | Next page is displayed correctly. |

#### Expected Result

The browser Forward button navigates to the next page successfully.

---

### TC_NAV_006 – Verify Navigation Menu Remains Accessible Across Pages

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_006 |
| **Module** | Navigation |
| **Requirement** | Navigation Consistency |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User navigates between application pages. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate through multiple pages. | Navigation menu remains visible and functional. |

#### Expected Result

The navigation menu is consistently available throughout the application.

---

### TC_NAV_007 – Verify Active Navigation Link is Highlighted

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_007 |
| **Module** | Navigation |
| **Requirement** | Navigation UI |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User is on a page accessible through the navigation menu. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open a page using the navigation menu. | Active navigation item is highlighted (if supported). |

#### Expected Result

The current page is visually indicated in the navigation menu.

---

### TC_NAV_008 – Verify Footer Navigation Links

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_008 |
| **Module** | Navigation |
| **Requirement** | Footer Navigation |
| **Priority** | Low |
| **Type** | Functional |
| **Precondition** | Footer contains navigation links. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click each footer navigation link. | Correct page opens successfully. |

#### Expected Result

Footer navigation links work correctly.

---

### TC_NAV_009 – Verify Navigation After Browser Refresh

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_009 |
| **Module** | Navigation |
| **Requirement** | Navigation Stability |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User is on any application page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Refresh the browser. | Current page reloads successfully. |
| 2 | Verify navigation menu. | Navigation remains functional. |

#### Expected Result

Navigation works correctly after refreshing the page.

---

### TC_NAV_010 – Verify Navigation Performance

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_010 |
| **Module** | Navigation |
| **Requirement** | Navigation Performance |
| **Priority** | Medium |
| **Type** | Functional / Performance |
| **Precondition** | Application is accessible. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate between multiple pages. | Pages load within acceptable response time. |

#### Expected Result

Navigation between pages is smooth and responsive.

---

### TC_NAV_011 – Verify Invalid Navigation URL Handling

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_011 |
| **Module** | Navigation |
| **Requirement** | Error Handling |
| **Priority** | Medium |
| **Type** | Functional / Negative |
| **Precondition** | User can modify the URL. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter an invalid application URL. | Appropriate error or 404 page is displayed. |

#### Expected Result

The application handles invalid URLs gracefully.

---

### TC_NAV_012 – Verify Navigation Consistency Across Browser Tabs

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_012 |
| **Module** | Navigation |
| **Requirement** | Navigation Consistency |
| **Priority** | Low |
| **Type** | Functional |
| **Precondition** | Application is open in multiple tabs. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate in different browser tabs. | Navigation behaves consistently. |

#### Expected Result

Navigation remains consistent across browser tabs.

---

### TC_NAV_013 – Verify Breadcrumb Navigation (If Available)

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_013 |
| **Module** | Navigation |
| **Requirement** | Breadcrumb Navigation |
| **Priority** | Low |
| **Type** | Functional |
| **Precondition** | Breadcrumb navigation exists. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate using breadcrumb links. | Correct page opens successfully. |

#### Expected Result

Breadcrumb navigation works correctly.

---

### TC_NAV_014 – Verify Keyboard Navigation Between Links

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_014 |
| **Module** | Navigation |
| **Requirement** | Accessibility |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Navigation menu is visible. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Press Tab to move through navigation links. | Focus moves sequentially between links. |
| 2 | Press Enter on a focused link. | Corresponding page opens successfully. |

#### Expected Result

Navigation is fully accessible using the keyboard.

---

### TC_NAV_015 – Verify Navigation Works on Different Screen Sizes

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_015 |
| **Module** | Navigation |
| **Requirement** | Responsive Navigation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Application is viewed on different screen sizes. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Resize the browser or use different devices. | Navigation adapts correctly. |

#### Expected Result

Navigation remains usable across supported screen sizes.

---

### TC_NAV_016 – Verify Navigation Menu Handles Missing Pages Gracefully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_016 |
| **Module** | Navigation |
| **Requirement** | Error Handling |
| **Priority** | Low |
| **Type** | Functional / Negative |
| **Precondition** | A navigation link points to an unavailable page (if testable). |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click the unavailable navigation link. | Appropriate error page or message is displayed. |

#### Expected Result

The application handles unavailable pages gracefully.

---

### TC_NAV_017 – Verify Navigation Remains Functional After Extended Browsing

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_NAV_017 |
| **Module** | Navigation |
| **Requirement** | Navigation Stability |
| **Priority** | Low |
| **Type** | Functional |
| **Precondition** | User has navigated through multiple pages for an extended period. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Continue navigating between pages for several minutes. | Navigation remains responsive and functional. |

#### Expected Result

Navigation continues to function reliably during extended user sessions.




