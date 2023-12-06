# MenuPairs

Displays all menu item pairs with their frequency in a table, given specified start and end dates.

## Props

<!-- @vuese:MenuPairs:props:start -->
|Name|Description|Type|Required|Default|
|---|---|---|---|---|
|startDate|start date of order history data to grab. form: yyyy-MM--dd|`String`|`true`|-|
|endDate|end date of order history data to grab. form: yyyy-MM--dd|`String`|`true`|-|

<!-- @vuese:MenuPairs:props:end -->


## Methods

<!-- @vuese:MenuPairs:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|fetchOrderHistoryData|Used to fetch order history data from the postgreSQL database, uses startDate & endDate props|-|
|calculateMenuPairsFrequency|Called from fetchOrderHistoryData(), takes current order history data, and records all menu item pairs with their frequencies.|-|
|recordMenuPairs|Helper function used in calculateMenuPairsFrequency(). Records frequencies of menu item pairs in the menuPairsFrequency list.|The argument, items, is a list of menu items from an order|
|sortMenuPairsByFrequency|Helper function used in calculateMenuPairsFrequency(). Sorts the current menu pairs list descending by frequency|-|

<!-- @vuese:MenuPairs:methods:end -->


