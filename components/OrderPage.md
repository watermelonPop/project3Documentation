# OrderPage

Displays a Point of Sale (POS) system for cashier's view

## Methods

<!-- @vuese:OrderPage:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|fetchCategoryData|Fetch item's category data from database|-|
|fetchMenuData|Fetch menu data from database|-|
|fetchSizeData|add-ons?type=Size Fetch drink's size data from database|-|
|fetchIceData|Fetch types of ice data from database|-|
|fetchSweetnessData|Fetch types of sweetness data from database|-|
|fetchToppingsData|Fetch types of topping data from database|-|
|aggregate|Organize the menu data by grouping items based on categories.|-|
|openModal|Open a pop-up window that allows the user to customize options|selected item|
|closeModal|Close a pop-up window that allows the user to customize options|-|
|selectSize|Select drink's size based on user's selection|selected drink's size|
|selectIce|Select an ice option based on user's selection|selected an ice option|
|selectSweet|Select drink's sweetness level based on user's selection|selected a sweetness level option|
|selectTopping|Select drink's toppings based on user's selection|selected topping options|
|resetSelectedOptions|reset user's selection for customization|-|
|orderEquals|Determine if orders are identical in terms of item, size, ice, sweetness, and toppings.|order1 and order2|
|checkOrder|Check if a given order already exists in the shopping cart|order|
|findOrder|Searches for the index of a specific order within the cart.|order|
|addToCart|Add an order into the cart|-|
|removeFromCart|Remove order from cart|order|
|getSizeClass|Get drink's size|item|
|getIceClass|Get drink's ice option|item|
|getSweetClass|Get drink's sweetness level option|item|
|getToppingClass|Get drink's toppings|item|
|setDiscount|Set discount options|discount percentage|
|increaseOrder|Increase quantity of order by 1|order|
|decreaseOrder|Decrease quantity of order by 1|order|
|openCheckout|Open display of the checkout panel in the user interface|-|
|closeCheckout|Close display of the checkout panel in the user interface|-|
|checkout|Update inventory stocks and send order details to order history in database|-|
|showMessage|Show message that placing order is completed|-|
|clear|Clear all orders in cart|-|
|OrderId|Set orderID by incrementing the order counter|-|
|CurrentDate|Get the current date in the format YY-mm-dd|-|
|CurrentTime|Get the current time in the format HH:mm:ss|-|
|OrderHistoryInsert|adding cart items to order history adding cart items to order history|-|
|GetIngredients|get ingredients from a drink get ingredients from a drink|drink's name|
|InventoryUpdate|update inventory quantity update inventory quantity|item|

<!-- @vuese:OrderPage:methods:end -->


## Computed

<!-- @vuese:OrderPage:computed:start -->
|Computed|Type|Description|From Store|
|---|---|---|---|
|cartSubtotal|-|Calculate subtotal of items in cart|No|
|calcCartDiscount|-|Calculate discount of total amount|No|
|cartTax|-|Calculate amount of tax in cart|No|
|cartTotal|-|Calculate total amount of items in cart|No|
|cartItems|-|Format order detail of items in cart|No|

<!-- @vuese:OrderPage:computed:end -->


