# Search Test Cases

## Purpose

This document contains the functional test cases for the Search module of the Shopify Sauce Demo application.

## Scope

The Search module includes testing of:

- Search functionality
- Search results
- Partial keyword search
- Exact keyword search
- Invalid search terms
- Empty search input
- No results found
- Search performance

- ---

## Test Case Summary

| Module | Total Test Cases | Status |
|---------|-----------------:|--------|
| Search | 17 | ✅ Completed |

### TC_SEARCH_001 – Verify Search Function Loads Successfully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_001 |
| **Module** | Search |
| **Requirement** | Search Functionality |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User is on the Product page where the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Open the Product page. | The Product page loads successfully. |
| 2 | Locate the search field. | The search field is visible and accessible. |
| 3 | Verify the search field is enabled. | The search field accepts user input. |

#### Expected Result

The search feature is displayed correctly and is ready to accept user input.

### TC_SEARCH_002 – Verify Search Using an Exact Product Name

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_002 |
| **Module** | Search |
| **Requirement** | Search Functionality |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User is on the Product page and products are available for search. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter the exact name of an existing product into the search field. | The search term is accepted. |
| 2 | Execute the search (press **Enter** or click the search button, if applicable). | The search is performed successfully. |
| 3 | Verify the search results. | The matching product is displayed in the search results. |

#### Expected Result

Searching with an exact product name returns the correct matching product.

### TC_SEARCH_003 – Verify Search Using a Partial Product Name

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_003 |
| **Module** | Search |
| **Requirement** | Search Functionality |
| **Priority** | High |
| **Type** | Functional |
| **Precondition** | User is on the Product page and products are available for search. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a partial product name into the search field. | The search term is accepted. |
| 2 | Execute the search (press **Enter** or click the search button, if applicable). | The search is performed successfully. |
| 3 | Verify the search results. | Products matching the partial keyword are displayed. |

#### Expected Result

Searching with a partial product name returns all relevant matching products.

### TC_SEARCH_004 – Verify Search is Case-Insensitive

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_004 |
| **Module** | Search |
| **Requirement** | Search Functionality |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User is on the Product page and products are available for search. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter the name of an existing product using a different letter case (e.g., uppercase or lowercase). | The search term is accepted. |
| 2 | Execute the search. | The search is performed successfully. |
| 3 | Verify the search results. | The correct matching product is displayed regardless of the letter case used. |

#### Expected Result

The search feature returns the correct results regardless of whether the search keyword is entered in uppercase, lowercase, or mixed case.

### TC_SEARCH_005 – Verify Search with an Invalid Product Name

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_005 |
| **Module** | Search |
| **Requirement** | Search Functionality |
| **Priority** | Medium |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter an invalid or non-existent product name into the search field. | The search term is accepted. |
| 2 | Execute the search. | The search is performed successfully. |
| 3 | Verify the search results. | No matching products are displayed, and an appropriate "No results found" message is shown (if supported by the application). |

#### Expected Result

The application handles invalid search terms gracefully by displaying no matching products and an appropriate message without errors.

### TC_SEARCH_006 – Verify Search with Empty Input

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_006 |
| **Module** | Search |
| **Requirement** | Search Validation |
| **Priority** | Medium |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Leave the search field empty. | The search field remains blank. |
| 2 | Execute the search (press **Enter** or click the search button, if applicable). | The application processes the request. |
| 3 | Verify the application's response. | The application either displays all products or prompts the user to enter a search term, according to the application's intended behavior. |

#### Expected Result

The application handles an empty search input gracefully without displaying errors or unexpected behavior.

### TC_SEARCH_007 – Verify Search Results Update for Different Search Terms

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_007 |
| **Module** | Search |
| **Requirement** | Search Results |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid search term and execute the search. | Matching search results are displayed. |
| 2 | Replace the search term with a different valid keyword. | The new search term is accepted. |
| 3 | Execute the search again. | The search results update to match the new keyword. |

#### Expected Result

The search results refresh correctly each time the user enters a different search term.

### TC_SEARCH_008 – Verify Search Results Are Cleared When the Search Field Is Cleared

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_008 |
| **Module** | Search |
| **Requirement** | Search Results |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User has performed a search and search results are displayed. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Perform a search using a valid keyword. | Matching search results are displayed. |
| 2 | Clear the search field. | The search field becomes empty. |
| 3 | Observe the product list. | The application resets the search results according to its intended behavior (e.g., displays all products or no filtered results). |

#### Expected Result

Clearing the search field resets the search results without requiring a page refresh or causing any application errors.

### TC_SEARCH_009 – Verify Search Handles Special Characters Gracefully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_009 |
| **Module** | Search |
| **Requirement** | Search Validation |
| **Priority** | Medium |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter one or more special characters (e.g., `@`, `#`, `%`, `!`) into the search field. | The search term is accepted. |
| 2 | Execute the search. | The search is performed successfully. |
| 3 | Verify the application's response. | The application handles the input gracefully by displaying appropriate results or a "No results found" message, without errors. |

#### Expected Result

The application processes search queries containing special characters without crashing, displaying errors, or behaving unexpectedly.

### TC_SEARCH_010 – Verify Search Performance with Valid Input

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_010 |
| **Module** | Search |
| **Requirement** | Search Performance |
| **Priority** | Medium |
| **Type** | Functional / Performance |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid product name into the search field. | The search term is accepted. |
| 2 | Execute the search. | The search request is submitted successfully. |
| 3 | Observe the response time. | Search results are displayed within an acceptable response time without noticeable delay. |

#### Expected Result

The application returns relevant search results promptly, providing a smooth and responsive user experience.

### TC_SEARCH_011 – Verify Search Retains the Entered Search Term After Results Are Displayed

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_011 |
| **Module** | Search |
| **Requirement** | Search Functionality |
| **Priority** | Low |
| **Type** | Functional |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid product name into the search field. | The search term is accepted. |
| 2 | Execute the search. | Matching search results are displayed. |
| 3 | Verify the search field after the results are displayed. | The entered search term remains visible in the search field. |

#### Expected Result

The search field retains the user's entered search term after the search results are displayed, allowing the user to review or modify the query.

### TC_SEARCH_012 – Verify Search Handles Leading and Trailing Spaces

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_012 |
| **Module** | Search |
| **Requirement** | Search Validation |
| **Priority** | Medium |
| **Type** | Functional |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a valid product name with leading and trailing spaces (e.g., " Backpack "). | The search term is accepted. |
| 2 | Execute the search. | The search is performed successfully. |
| 3 | Verify the search results. | The correct matching product is displayed despite the extra spaces. |

#### Expected Result

The application ignores unnecessary leading and trailing spaces and returns the correct search results.

### TC_SEARCH_013 – Verify Search Handles Numeric Input Gracefully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_013 |
| **Module** | Search |
| **Requirement** | Search Validation |
| **Priority** | Low |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a numeric value (e.g., `12345`) into the search field. | The search term is accepted. |
| 2 | Execute the search. | The search is performed successfully. |
| 3 | Verify the application's response. | The application displays matching products (if any) or an appropriate "No results found" message without errors. |

#### Expected Result

The application handles numeric search input gracefully without crashing, displaying errors, or behaving unexpectedly.

### TC_SEARCH_014 – Verify Search Handles Very Long Input Gracefully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_014 |
| **Module** | Search |
| **Requirement** | Search Validation |
| **Priority** | Medium |
| **Type** | Functional / Negative |
| **Precondition** | User is on the Product page and the search feature is available. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Enter a very long string of characters into the search field (e.g., more than 100 characters). | The search term is accepted. |
| 2 | Execute the search. | The search is performed successfully. |
| 3 | Verify the application's response. | The application handles the input gracefully by displaying matching results (if any) or an appropriate "No results found" message without errors. |

#### Expected Result

The application handles excessively long search input without crashing, slowing down significantly, or displaying unexpected behavior.

### TC_SEARCH_015 – Verify Search State After Browser Refresh

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_015 |
| **Module** | Search |
| **Requirement** | Search Functionality |
| **Priority** | Low |
| **Type** | Functional |
| **Precondition** | User has performed a search and search results are displayed. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Perform a search using a valid product name. | Matching search results are displayed. |
| 2 | Refresh the browser page. | The page reloads successfully. |
| 3 | Verify the search field and displayed products. | The application behaves according to its intended design (e.g., search is retained or reset) without displaying errors. |

#### Expected Result

Refreshing the page does not cause application errors, and the search feature behaves consistently with the application's expected design.

### TC_SEARCH_016 – Verify Search Handles No Products Available

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_016 |
| **Module** | Search |
| **Requirement** | Search Results |
| **Priority** | Low |
| **Type** | Functional / Negative |
| **Precondition** | The Product page is accessible, but no products are available for display. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Navigate to the Product page when no products are available. | The page loads successfully. |
| 2 | Enter any search term into the search field. | The search term is accepted. |
| 3 | Execute the search. | The application indicates that no products are available or no results are found, without displaying errors. |

#### Expected Result

The search feature handles the absence of products gracefully by displaying an appropriate message and remaining fully functional.

### TC_SEARCH_017 – Verify Search Handles Unexpected Errors Gracefully

| Field | Value |
|--------|-------|
| **Test Case ID** | TC_SEARCH_017 |
| **Module** | Search |
| **Requirement** | Search Error Handling |
| **Priority** | Low |
| **Type** | Functional / Negative |
| **Precondition** | The search feature is available, and an unexpected backend or network error can be simulated. |

#### Test Steps

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Simulate an unexpected backend or network error while performing a search. | The search request is interrupted. |
| 2 | Observe the application's response. | A user-friendly error message is displayed (if supported), and the application remains responsive. |
| 3 | Retry the search after the error condition is resolved. | The search feature functions normally. |

#### Expected Result

The application handles unexpected search errors gracefully without crashing, and users are able to retry the search successfully once the issue is resolved.








