# OrderHistory

Fetches order history data from the specified dates/timeframe, displays it in a table.

## Methods

<!-- @vuese:OrderHistory:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|fetchOrderHistoryData|fetches order history data based on start & end dates specified by user|-|
|setCurrentDate|set currentDate with the current date|-|
|setTimeFrame|sets the start & end dates based on timeframe selected by user|timeframe -- Today / 1D / 1W / 1M / 3M -- timeframe to grab data from|
|calculateDate|returns a yyyy-MM--dd formatted date using the given year, month, and day|year -- integer year, month -- integer month, day -- integer day|
|formatDate|formats date given to be yyyy-MM-dd|date -- specified string date|
|toggleDateSelection|updates showDateSelection, and displays date selection panel for user|-|
|updateDateRange|updates the start & end dates and regrabs order history data to display|-|

<!-- @vuese:OrderHistory:methods:end -->


