# Test design
## Test design techniques  
Testing the registration form using the most popular test design technique - creating equivalence classes and boundary values.  
The following user story was used to create the test data.  

User Registration  

EN: As a new user,  
I want to create an account on the website,  
So that I can access personalized features and content.  

Acceptance Criteria:  

The user must enter a username and password to create an account.  
The username must contain 3 to 15 characters and can include letters, numbers, and symbols: _.  
The password must be at least 8 characters long, including at least one letter and one number.  
The button "Войти" should change to "Выйти" after successful registration.  

Exception Cases:  

If the username or password does not meet the requirements, the user sees the message: "The username must contain 3 to 15 characters and can include letters, numbers, and symbols: _. The password must be at least 8 characters long, including at least one letter and one number".  
In case of a server error, the user receives the message: "An error occurred while processing the request".  

[User Registration](https://docs.google.com/spreadsheets/d/10-J-I-4K6tQvR2SgXdzFPXb5F2ei2ZBI/edit?usp=sharing&ouid=103546442425628569603&rtpof=true&sd=true)

## Pairwise for filtering and sorting 

The Online Store app has a great opportunity to use the Pairwise Testing technique: filtering and sorting functions. Filtering and sorting requirements are also presented as user stories.  

Filtering the product list  
EN: As a customer, I want to filter the product list by price, category, manufacturer, and the availability of free shipping to find products that meet my search criteria.  

Acceptance Criteria:  

Customers can specify a price range, select a category, manufacturer, and free shipping option to filter the product list.  
Customers can reset all selected filters with a single click.  
The product list updates according to the applied filters.  
Exception Cases:  

If applying filters does not change the product list (e.g., due to no products matching the criteria), an appropriate notification is displayed.  

Sorting the product list  

EN: As a customer, I want to sort the list of products by name and price to quickly find products that match my preferences.  

Acceptance Criteria:  

Customers can choose to sort products by name (from A to Z and from Z to A) and by price (from low to high and from high to low).  
The product list updates according to the chosen sort order.  

[Filtering and sorting](https://docs.google.com/spreadsheets/d/1QUbPx9tZ_pq4PZp6Xptry-Yd9BC5hVGo/edit?usp=sharing&ouid=103546442425628569603&rtpof=true&sd=true)

## Decision Table for Paypal Payment   
Application of the test design technique "Decision Table".  

Our application has a module that includes payment via Paypal.  

A Paypal account has three statuses: valid, invalid and blocked, as well as such a characteristic as an available balance, which can be zero or positive.  

If the card status is valid and the balance on the account is sufficient for the purchase, the user can make the purchase. In all other cases, the transaction will be rejected.  

[Paypal Payment](https://docs.google.com/spreadsheets/d/1rXVJE0l-eddQ5RowH4bKzTJdbPLCGUdv/edit?usp=drive_link&ouid=103546442425628569603&rtpof=true&sd=true)
