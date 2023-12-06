# LoginPage

A login page featuring a form for entering usernames and passwords, authenticating users based on predefined roles upon submission, and redirecting them to corresponding views.

## Methods

<!-- @vuese:LoginPage:methods:start -->
|Method|Description|Parameters|
|---|---|---|
|updateTime|computes the current time in the format HH:mm:ss|-|
|login|Handle the login form submission|-|
|authenticateEmployee|Authenticate employee credentials|employee username, employee password, True if authentication succeeds, false otherwise.|
|authenticateManager|Authenticate manager credentials|manager username, manager password, True if authentication succeeds, false otherwise.|
|authenticateCustomer|Authenticate customer credentials|customer username, customer password, True if authentication succeeds, false otherwise.|
|authenticateCashier|Authenticate cashier credentials|cashier username, cashier password, True if authentication succeeds, false otherwise.|
|openPOS|Open the Point of Sale (POS) view for an employee|employee username|
|openManager|Open the Manager view.|-|
|openCustomer|Open the customer view.|-|
|openCashier|Open the cashier view.|-|

<!-- @vuese:LoginPage:methods:end -->


