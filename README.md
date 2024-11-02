# showing-the-BDD-Scenario-for-DELETING-a-Product-
Scenario: Deleting a product
  Given the following products
    | name   | category | available |
    | ToyCar | Toys     | true      |
  When I delete the product "ToyCar"
  Then the product "ToyCar" should not exist
