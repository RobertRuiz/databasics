## Databasics

Fork this repository into your own github profile.

Before closing the homework assignment issue:

- Update this README as follows:
  - [ ] For each question (just after or below the question itself) include the SQL you wrote to generate the answer
  - [ ] For each question (just after or below the question itself) include the *answer* to the question asked.

- Also:
  - [ ] Commit the updated `store.sqlite3` database file
  - [ ] Include a link to your forked repo in the comments when closing the issue.


NOTE: To run sqlite with this database: `sqlite3 store.sqlite3`

NOTE: You may want to keep a backup of the `store.sqlite3` file in case you damage the file. *OR* you can use the command `git checkout store.sqlite3` to undo any changes to the database file since the fork or your last commit.

## Explorer Mode

- [ ] How many users are there?
      select * from users;
      50

- [ ] What are the 5 most expensive items?
      select title, price from items order by price;
      title                      price     
      -------------------------  -------------------  
      Ergonomic Steel Car        9341      
      Sleek Wooden Hat           9390      
      Awesome Granite Pants      9790      
      Small Wooden Computer      9859      
      Small   Cotton Gloves      9984

- [ ] What's the cheapest book? (Does that change for "category is exactly 'book'" versus "category contains       'book'"?)
      select title, price from items order by price;
      title                      price     
      -------------------------  -------------------  
      Incredible Concrete Chair  121

      select title, price from items where category = "Books";
      title                      price     
      -------------------------  -------------------
      Ergonomic Granite Cha      1496

- [ ] Who lives at "6439 Zetta Hills, Willmouth, WY"? Do they have another address?


- [ ] Correct Virginie Mitchell's address to "New York, NY, 10108".


- [ ] How much would it cost to buy one of each tool?


- [ ] How many total items did we sell?


- [ ] How much was spent on books?


- [ ] Simulate buying an item by inserting a User for yourself and an Order for that User.


## Adventure Mode

- [ ] What item was ordered most often? Grossed the most money?


- [ ] What user spent the most?


- [ ] What were the top 3 highest grossing categories?
