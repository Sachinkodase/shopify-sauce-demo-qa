# Responsive Test Cases

## Purpose

This document contains the functional test cases for the Responsive module of the Shopify Sauce Demo application.

## Scope

The Responsive module includes testing of:

- Desktop responsiveness
- Tablet responsiveness
- Mobile responsiveness
- Responsive navigation
- Product layout responsiveness
- Cart responsiveness
- Checkout responsiveness
- Orientation changes
- Browser resizing

## Test Case Summary

| Module | Total Test Cases | Status |
|---------|-----------------:|--------|
| Responsive | 17 | ✅ Completed |

---

### TC_RESP_001 – Verify Homepage Displays Correctly on Desktop

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_001 |
| **Module** | Responsive |
| **Requirement** | Desktop Responsiveness |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Application is opened on a desktop browser. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the homepage on a desktop browser. | Homepage loads successfully. |
| 2 | Verify page layout. | All elements are displayed correctly. |

#### Expected Result

Homepage displays correctly on desktop screens.

---

### TC_RESP_002 – Verify Homepage Displays Correctly on Tablet

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_002 |
| **Module** | Responsive |
| **Requirement** | Tablet Responsiveness |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Application is opened on a tablet or tablet emulator. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the homepage on a tablet. | Homepage loads successfully. |
| 2 | Verify page layout. | Elements resize and align correctly. |

#### Expected Result

Homepage is fully usable on tablet devices.

---

### TC_RESP_003 – Verify Homepage Displays Correctly on Mobile

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_003 |
| **Module** | Responsive |
| **Requirement** | Mobile Responsiveness |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Application is opened on a mobile device or emulator. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the homepage on a mobile device. | Homepage loads successfully. |
| 2 | Verify page layout. | Content fits the screen without horizontal scrolling. |

#### Expected Result

Homepage displays correctly on mobile devices.

---

### TC_RESP_004 – Verify Navigation Menu Adapts to Different Screen Sizes

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_004 |
| **Module** | Responsive |
| **Requirement** | Responsive Navigation |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Application is open on multiple screen sizes. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Resize the browser window. | Navigation adjusts automatically. |
| 2 | Verify navigation usability. | Navigation remains functional. |

#### Expected Result

Navigation adapts correctly to different screen sizes.

---

### TC_RESP_005 – Verify Product Grid Adjusts to Screen Size

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_005 |
| **Module** | Responsive |
| **Requirement** | Product Layout |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Product page is open. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Resize the browser or use different devices. | Product grid adjusts correctly. |

#### Expected Result

Product cards are displayed appropriately for each screen size.

---

### TC_RESP_006 – Verify Product Images Scale Correctly

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_006 |
| **Module** | Responsive |
| **Requirement** | Image Responsiveness |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Product page is displayed. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | View products on multiple screen sizes. | Images resize without distortion. |

#### Expected Result

Product images remain clear and properly scaled.

---

### TC_RESP_007 – Verify Cart Page is Responsive

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_007 |
| **Module** | Responsive |
| **Requirement** | Cart Responsiveness |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | Cart contains at least one item. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the cart on different devices. | Cart layout adjusts correctly. |

#### Expected Result

Cart remains usable across supported screen sizes.

---

### TC_RESP_008 – Verify Checkout Page is Responsive

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_008 |
| **Module** | Responsive |
| **Requirement** | Checkout Responsiveness |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User is on the checkout page. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open checkout on multiple screen sizes. | Layout adjusts correctly. |

#### Expected Result

Checkout remains fully usable on all supported devices.

---

### TC_RESP_009 – Verify Buttons Remain Accessible on Small Screens

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_009 |
| **Module** | Responsive |
| **Requirement** | UI Responsiveness |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Application is open on a mobile device. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Verify all action buttons. | Buttons remain visible and clickable. |

#### Expected Result

Buttons are accessible without overlap or clipping.

---

### TC_RESP_010 – Verify Text Remains Readable on All Devices

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_010 |
| **Module** | Responsive |
| **Requirement** | Typography |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Application is open on different devices. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Inspect page text. | Text remains readable without zooming. |

#### Expected Result

Typography scales appropriately across screen sizes.

---

### TC_RESP_011 – Verify Browser Resize Does Not Break Layout

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_011 |
| **Module** | Responsive |
| **Requirement** | Layout Stability |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Application is open in a browser. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Continuously resize the browser window. | Layout adjusts smoothly. |

#### Expected Result

No layout breaks occur during browser resizing.

---

### TC_RESP_012 – Verify Landscape Orientation

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_012 |
| **Module** | Responsive |
| **Requirement** | Device Orientation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Mobile device supports landscape mode. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Rotate device to landscape mode. | Layout adjusts correctly. |

#### Expected Result

Application functions correctly in landscape orientation.

---

### TC_RESP_013 – Verify Portrait Orientation

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_013 |
| **Module** | Responsive |
| **Requirement** | Device Orientation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Mobile device supports portrait mode. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Rotate device to portrait mode. | Layout adjusts correctly. |

#### Expected Result

Application functions correctly in portrait orientation.

---

### TC_RESP_014 – Verify Responsive Layout After Browser Refresh

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_014 |
| **Module** | Responsive |
| **Requirement** | Layout Stability |
| **Priority** | Low |
| **Type** | Functional |
| **Precondition** | Application is open on any supported device. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Refresh the browser. | Responsive layout is maintained. |

#### Expected Result

Refreshing the page does not affect responsive behavior.

---

### TC_RESP_015 – Verify No Horizontal Scroll Appears on Mobile

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_015 |
| **Module** | Responsive |
| **Requirement** | Mobile Layout |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | Application is open on a mobile device. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Browse multiple pages on mobile. | No unnecessary horizontal scrolling occurs. |

#### Expected Result

Pages fit within the mobile viewport.

---

### TC_RESP_016 – Verify Responsive Layout Under Slow Network Conditions

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_016 |
| **Module** | Responsive |
| **Requirement** | Performance |
| **Priority** | Low |
| **Type** | Functional |
| **Precondition** | Browser network throttling is enabled. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Load the application using a slow network profile. | Responsive layout loads correctly after content is available. |

#### Expected Result

Responsive layout remains stable under slow network conditions.

---

### TC_RESP_017 – Verify Responsive Layout Handles Unexpected Errors Gracefully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_RESP_017 |
| **Module** | Responsive |
| **Requirement** | Error Handling |
| **Priority** | Low |
| **Type** | Functional / Negative |
| **Precondition** | An unexpected rendering or resource-loading error can be simulated. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Simulate a rendering or resource-loading error. | The application remains usable and displays content as gracefully as possible. |

#### Expected Result

The responsive layout handles unexpected issues without causing major usability problems.
