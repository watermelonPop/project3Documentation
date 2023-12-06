# Inventory

Displays inventory data & information, and offers the following features to managers: add item to inventory, update remaining quantity of inventory item, update restock quantities, view list of items that need to be restocked, view the excess report for a specified time frame,

## Methods

<!-- @vuese:Inventory:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|showSection|updates currentSection, and shows specified div|section -- specified div section|
|handleInsert|handles inventory item insert, and updates the postgreSQL database accordingly|-|
|fetchRestockQuantities|fetches restock quantities from postgreSQL database -- the minimum quantity that each category has to signal restock|-|
|fetchInventoryData|called from fetchRestockQuantities(). fetches inventory data from postgreSQL database.|-|
|groupInventoryByType|called from fetchInventoryData(). groups inventory data we already grabbed by item type, updates inventoryData & itemList|-|
|getLowItems|called from groupInventoryByType(). traverses inventory data & finds and records all items below the item type's restock quantity.|-|
|isLowItem|returns boolean -- whether or not an item is "low" ie needs to be restocked & should be highlighted|item -- inventory item|
|updateSelectedItem|updates selectedUpdateItem with the item selected in the event|event -- item selected|
|updateQuantityCall|updates inventory restock quantity of the selectedUpdateItem with newQuant in the postgreSQL database|-|
|showExcessReport|shows the excess report form using startDate & endDate -- updates excessreport & displays in section|-|
|toggleAccordion|opens or closes accordion at index, and appends index to openAccordions list if necessary|index -- index of accordion to be toggled|
|isAccordionOpen|returns boolean -- whether or not the accordion at the index is open|index -- index of accordion specified|
|updateRestockArr|Updates the restock quantities list at the index with the quantity|index -- index of item type, quantity -- new restock quantity|
|updateRestockQuantity|called in applyRestockSettings(). Updates restock quantity of specific type of item in the postgreSQL database|productType -- type of inventory item, quantity -- new restock quantity|
|applyRestockSettings|uses updateRestockQuantity() as helper function to update database values|-|
|getAccordionProduct|returns the type of item displayed in the given index's accordion|index -- index of accordion specified|

<!-- @vuese:Inventory:methods:end -->


