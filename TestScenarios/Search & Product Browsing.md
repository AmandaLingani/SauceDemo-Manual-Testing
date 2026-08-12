# Test Scenario
TS-001: Verify that search functionality works
-Description: Verify that available items can be found and appropriate messages are displayed for unavailable items or invalid searches

TS-002: Verify product browsing functionality
-Description: Verify that available products are displayed correctly, with appropriate information including names, descriptions, prices and images

## Test Cases
Test Case ID: TC-001
Title: Verify search function filters and displays products with matching products
Preconditions: Item exists in the system 
Steps:
  1. Go to the search bar
  2. Type 'Grey Jacket'
  3. Press 'Enter/Search'
Expected Results: Items with the name 'Grey Jacket' are displayed with their respective information
Actual Results: All items are displayed
Status: FAIL

Test Case ID: TC-002
Title: 
Verify nothing is displayed for products that do not exist
Preconditions: Product is not in the system
Steps: 
  1. Go to the search bar
  2. Type in a word that doesn't exist (e.g. Black Pants)
  3. Press 'Enter/Search'
Expected Results: No products are returned and an appropriate message is displayed.
Actual Results: No products are displayed and an appropriate message is displayed "No results found for Black pants"
Status: PASS



