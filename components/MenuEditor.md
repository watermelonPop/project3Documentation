# MenuEditor

Displays all menu items from the database in a grid. Each menu item is clickable, and allows managers to edit the name, description & upload their own images to the database.

## Methods

<!-- @vuese:MenuEditor:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|fetchMenu|fetches images, descriptions & names of all menu items from the postgreSQL database|-|
|fetchAltText|fetches alt texts for all images from the postgreSQL database|-|
|getAltText|traverses altText list, returns alt text for the image|image -- image to find alt text for|
|openEditDialog|opens the editor modal for the specified menu item at the index|index -- index of specified menu item|
|applyEdit|Handles applying changes to menu items from the editor, uses updateMenuNameDesc() as a helper function to update the database.|index -- menu item to be changed|
|closeEditDialog|closes the editor modal|-|
|handleImageUpload|handles when an image is uploaded by the user|event -- image is uploaded by the user|
|updateMenuNameDesc|called as helper function in applyEdit(). Updates the postgreSQL database with the menu item's new name, description, and image|-|

<!-- @vuese:MenuEditor:methods:end -->


