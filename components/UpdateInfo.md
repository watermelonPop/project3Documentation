# UpdateInfo

Changes customer information (name, password, or email),

## Methods

<!-- @vuese:UpdateInfo:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|updateName|Grabs email from local storage and calls updateInformation function with updated name|-|
|updatePassword|Calls updateInformation function with updated password|-|
|updateEmail|Calls updateInformation function with updated email|-|
|updateInformation|Sends api request to server and updates the customer Information in the database based on values|apiEndpoint -- api request being called value -- value to update the given customer information with|
|goToCustomerLogin|Navigates back to the customerLogin page|-|

<!-- @vuese:UpdateInfo:methods:end -->


