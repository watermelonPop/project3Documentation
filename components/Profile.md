# Profile

Displays the customer's name, number of points, and rewards dollars -- also give user the option to update account and delete account,

## Methods

<!-- @vuese:Profile:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|fetchUserData|Sends API request to fetch customer data from the database|customerEmail -- user's email from login|
|animateFill|Shows circle being filled with percentage of points.|-|
|toggleSettings|Opens options for user to delete account, update information, or switch account|-|
|updateInformation|Navigates user to the update Information page where they change their data|data -- customer data|
|signOut|Signs user out and navigates back to login page|-|
|deleteAccount|Deletes customers account from the database|userData -- User's information|

<!-- @vuese:Profile:methods:end -->


