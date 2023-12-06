# SalesTrends

Displays the following graph options: "Select Graph" / "Prices Over Time" / "Order History Trends" / "Menu Pairs". These graphs show different information about the order history postgreSQL database.

## Methods

<!-- @vuese:SalesTrends:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|setCurrentDate|calculates the current date and returns in string form: yyyy-MM-dd|-|
|setTimeFrame|sets the current graph's timeframe, by resetting the selectedGraphType to "Select Graph" and then updating the selectedGraphType back to the originally chosen type. This refreshes the data & graph information & rerenders.|timeFrame -- 1W / 1M / 3M / 1Y -- timeframe to grab data from for the graph|
|calculateDate|returns a yyyy-MM--dd formatted string date using the given year, month, and day|year -- integer year, month -- integer month, day -- integer day|
|formatDate|formats date given to be yyyy-MM-dd|date -- specified string date|
|toggleDateSelection|updates showDateSelection, and displays date selection panel for user|-|
|updateDateRange|handles user inputted start & end dates -- refreshes the data & component|-|

<!-- @vuese:SalesTrends:methods:end -->


## Computed

<!-- @vuese:SalesTrends:computed:start -->
|Computed|Type|Description|From Store|
|---|---|---|---|
|startDate|-|computes the startDate based on timeframe/user input|No|
|endDate|-|computes the endDate based on timeframe/user input. For timeframe, the endDate is always today.|No|

<!-- @vuese:SalesTrends:computed:end -->


