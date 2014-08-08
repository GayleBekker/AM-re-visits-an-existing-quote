AM-re-visits-an-existing-quote
==============================

As an Account Manager i want to edit a quote/basket that i have already submitted to my customer as he requires an amendment to the quote.

1.Account Manager adjusts a quote

1.1 Feature: Edit quote submitted to BDC
When I have submitted a quote for approval to the BDC
And I want to edit the quote
So that I can change or remove a product
And satisfy the customer

Background:
Given I am logged in as an AM
And a list of 'my deals' is displayed
And I have already submitted to BDC
And I want to change the deal
And I select the "edit" icon next to the deal
Then the basket is then open to be edited

1.1.1.  Scenario: Edit a submitted quote
Given I have a basket of products
And the basket has an "edit" icon
Then i click the "edit" basket icon

1.1.2   Scenario: Edit Products
Given i have a list of products
And i click on the "edit" button
Then I can edit the products in the basket and the opportunity percentage will display as 19%

1.1.3   Scenario: I want to see the product catalogue
Given I have selected the product to 'edit'
And my product basket is displayed on the right
Then am able to see the 'product catalogue' menu

1.1.4   Scenario: I want to select products from the managed product catalogue menue
Given I have accessed the "product catalogue"
And i select "Packages"
Then i can choose a new package

1.1.5   Scenario: I want to choose a new managed product
Given I have chosen a new product
And i select "add product"
Then i can select the package

1.1.6   Scenario: I want to add the new managed product
Given a product is added
And the undesired product has been replaced
Then the new information is displayed in the basket

1.1.7 Scenario: i want to select unmanaged products from the product catalogue menu
Given i access the "product catalogue"
And i select "unmanaged packages"
Then i can choose a new unmanaged package product

1.1.8 Scenario: I want to choose a new unmanaged product
Given I have chosen a new product
And i select "add product"
Then i can select the product

1.1.9 Scenario: I want to add the new unmanaged product
Given a product is added
And the undesired product has been replaced
Then the new information is displayed in the basket

1.1.10 Scenario: i want to view my new basket
Given I have the new product displayed
And the other items in the basket are displayed
Then I can see the amended basket

1.1.11 Scenario: Submit to the BDC
Given i have selected the new product
And i have added to the basket
Then i can "send to BDC"

1.1.12 Scenario: I want to view my amended deal basket
Given i have completed the basket selection
And I click on "deal overview"
Then i should see the basket 

Background:
Given I am logged in an a BDC
And i have a basket to approve
And the AM is "editing" the basket
And I click on the basket
And a the "Draft" button is red
Then i should not be able to open the basket

1.2 Scenario: When a BDC should not be able to approve a quote
Given i am on the "my deals" page
And the AM is editing the quote
Then I should not be able to open the the basket

1.2.1 Scenario: BDC receives an approval notification
Given the AM has chosen a new product
And i receive a notification
Then i can view the basket which is highlighted in a red

1.2.2. Scenario: BDC to approve basket
Given I have a basket to approve
And I select the red draft button
Then I can see the basket
