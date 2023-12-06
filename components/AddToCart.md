# AddToCart

Enables add to cart feature when customer orders a boba tea

## Methods

<!-- @vuese:AddToCart:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|fetchAltText|Retrieved image alt text from the database and image table|-|
|getAltText|Retrieve boba tea image descriptions and images|-|
|increaseQuantity|Allows the user to increase the quantity of a boba tea when in the cart|-|
|decreaseQuantity|Allows the user to decrease the quantity of a boba tea when in the cart|-|
|setTip|Sets the tip based on the percent selected by the customer when ordering|-|
|processPayment|Process the order being inputted by the user, sends user a confirmation message with the details of the order|-|
|fetchCartItems|Retrieves items ordered and added to the cart from the database cart table|-|
|clearCart|Deletes all of the items in the cart|-|
|updateQuantityInDatabase|Update the quantity of the particular menu item in the database in the cart table|-|
|goBack|Navigate the user to the correct ordering page based on their login|-|
|formatOrderDetails|Create the string for order details when the user adds all of their items to the cart|-|
|OrderId|Stores the unique id for every order|-|
|CurrentDate|Sets the date on the cart page when the customer places the order|-|
|CurrentTime|Sets the current time on the cart page when the customer places the order|-|
|addOrderHistory|Adds order data from the cart to the database cart sql table|-|
|GetIngredients|Retrieves ingredients for the specific boba tea drink added to the cart|-|
|InventoryUpdate|Updates inventory quantity with the time, date and ordered boba tea item when order is processed|-|
|updateInventoryForCartItems|Updates ingredients in the inventory database table|-|

<!-- @vuese:AddToCart:methods:end -->


## Computed

<!-- @vuese:AddToCart:computed:start -->
|Computed|Type|Description|From Store|
|---|---|---|---|
|calculateSubtotal|-|Calculates the subtotal before tip, tax and discounts when a customer orders boba tea|No|
|calculateTotal|-|Calculates final total of transaction including subtotal and tip|No|

<!-- @vuese:AddToCart:computed:end -->


