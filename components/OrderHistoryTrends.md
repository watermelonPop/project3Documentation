# OrderHistoryTrends

Displays a line graph of selected menu items and their order frequencies, given specified start and end dates.

## Props

<!-- @vuese:OrderHistoryTrends:props:start -->
|Name|Description|Type|Required|Default|
|---|---|---|---|---|
|startDate|start date of order history data to grab. form: yyyy-MM--dd|`String`|`true`|-|
|endDate|end date of order history data to grab. form: yyyy-MM--dd|`String`|`true`|-|

<!-- @vuese:OrderHistoryTrends:props:end -->


## Methods

<!-- @vuese:OrderHistoryTrends:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|fetchMenu|fetches all menu item names from postgreSQL database, updates menu var|-|
|fetchPricesFreq|Called from fetchMenu(), to fetch order history data from startDate to endDate|-|
|setFreq|Called from fetchPricesFreq(), uses order history data to fill in dates & frequencies value lists|-|
|datesContains|returns boolean -- whether or not the list arr contains the date curr|arr is a list of dates curr is a specific date in form yyyy-MM-dd|
|dateIndex|returns integer -- index of date curr in list arr|arr is a list of dates curr is a specific date in form yyyy-MM-dd|
|showCheckedDiv|sets modal variable to show modal of menu items with checkboxes next to each|-|
|handleCheckboxChange|appends to selectedItems list with item upon event|event -- checkbox change applied item -- menu item chosen|
|isSelected|returns boolean -- whether or not the menu item was selected by the user|item -- menu item|
|updateChart|Handles chart update + calls the redraw function|-|
|generateRandomColor|returns a randomized color as a hex code|-|
|drawChart|draws the line chart using the dates & frequencies lists, with each menu item having a different random colored line.|-|

<!-- @vuese:OrderHistoryTrends:methods:end -->


