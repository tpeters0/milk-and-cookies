# Fridge Management App

We're going to building a fridge management app to keep track of all of our food and drink using ActiveRecord. It may be helpful to review the docs for [ActiveRecord Basics](http://edgeguides.rubyonrails.org/active_record_basics.html) and [ActiveRecord Associations](http://edgeguides.rubyonrails.org/association_basics.html) for this.

# Part 1 - Database Schemas
- Create a new database called kitchen_db.
- Create the database tables to model Fridge, Food, and Drink and their relationships and validations (See specs below).
- Create your tables using ActiveRecord migrations.

# Part 2 - Setting up ActiveRecord
- Hook up your main ruby file to the kitchen_db
- Use your menu system to incorporate methods to perform the specific ActiveRecord actions.
- Populate your database (using ActiveRecord) with at least 3 fridges, 3 foods, and 3 drinks (associated correctly!).

# Specs!

### Menu Spec

- Your program should have a menu that allows you to perform the following actions:
  * List all Fridges
  * Add a Fridge
  * Delete a Fridge
  * View all food items in a specific fridge
  * Add a food item to a fridge
  * Eat a food item from a fridge (delete it)
  * View all drink items in a specific fridge
  * Add a drink item to a fridge
  * Consume PART of a drink from a fridge (update its size in ounces)
  * Consume ALL of a drink from a fridge (delete it)

### Fridge Spec
* has a location
* has a brand
* has a size in cubic feet
* has food in it
* has drinks in it

### Food Spec
* has a name
* has a weight in pounds
* is vegan or not
* has a timestamp of when it was put in the fridge

### Drink Spec
* has a name
* has a size in ounces
* is either alcoholic or not

### Validations Part

* Fridges don't have to contain food or drink in them, but they must have a location, brand and size. Make sure you validate for these using ActiveRecord.
* You can only have 10 food items in your fridge
* Update you restrictions to only allow 50 total ounces of drinks in your fridge

# Bonus!
- Write some tests!
  - Test your validations.