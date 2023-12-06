# PricesOverTime

Displays a line graph of daily order price totals over time, given specified start and end dates.

## Props

<!-- @vuese:PricesOverTime:props:start -->
|Name|Description|Type|Required|Default|
|---|---|---|---|---|
|startDate|start date of order history data to grab. form: yyyy-MM--dd|`String`|`true`|-|
|endDate|end date of order history data to grab. form: yyyy-MM--dd|`String`|`true`|-|

<!-- @vuese:PricesOverTime:props:end -->


## Methods

<!-- @vuese:PricesOverTime:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|drawChart|draws line chart using dates & prices lists|-|
|aggregateData|Called from fetchPricesDates(), to aggregate each day's data -- each date should have 1 price value|-|
|fetchPricesDates|Fetches order history data between startDate and endDate|-|
|refresh|Refreshes all graph data with a new start & end date|newStart -- new start date, newEnd -- new end date|

<!-- @vuese:PricesOverTime:methods:end -->


