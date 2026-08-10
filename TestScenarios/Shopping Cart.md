# Test Scenrios
TS-001 – Verify adding items to the shopping cart
Description: Verify that users can add one or more products to the shopping cart successfully.

TS-002 – Verify updating items in the shopping cart
Description: Verify that users can update the contents of the shopping cart where applicable (e.g., quantity, size).

TS-003 – Verify removing items from the shopping cart
Description: Verify that users can remove individual items or clear the shopping cart successfully.

TS-004 – Verify shopping cart validation
Description: Verify that the application correctly handles invalid shopping cart actions and displays appropriate messages.

## Test Cases
Test Case ID: TC-001
Title: Verify all available items can be added to shopping cart
Preconditions: Items are in stock
Steps:
 1. Navigate to 'Catalog'
 2. Select an item
 3. Click 'Add to cart'
Expected Results: Selected item is added to the cart successfully and the user stays in the catalog page
Actual Results: Selected item is added to the cart successfully and user stays in the catalog page
Status: PASS

Test Case ID: TC-002
Title: Verify that sold out items cannot be added to the shopping cart
Preconditions: Item is out of stock
Steps:
 1. Navigate to 'Catalog'
 2. Select a sold out item
Expected Results: There is a 'Sold Out' button and item cannot be added to cart
Actual Results: There is a 'Sold Out' button and item cannot be added to cart
Status: PASS

Test Case ID: TC-003
Title: Verify items in cart can be modified
Preconditions: Item is in stock
             : Item is already in the shopping cart
Steps:
 1. Navigate to 'Shopping Cart'
 2. Modify the quantity(e.g from 1 to 2)
Expected Results: The item quantity is updated successfully from 1 to 2 items
Actual Results: The item quantity is updated successfully from 1 to 2 items
Status: PASS

Test Case ID: TC-004
Title: Verify items in cart can be removed
Preconditions: Item is already in the shopping cart
Steps:
 1. Navigate to 'Shopping Cart'
 2. Remove one item
 3. Click 'Update' button
Expected Results: The item is successfully removed in the cart
Actual Results: The item is successfully removed in the cart
Status: PASS


