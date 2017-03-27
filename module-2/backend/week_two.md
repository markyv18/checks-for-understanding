## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR.

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
a database assistant for ruby/sinatra/rails.  allows for rapid queries of the db

2. Assume you have the following model:

```ruby
class Team << ActiveRecord::Base
end
```

What are some methods you can call on `Team`? If these methods aren't defined in the class, how do you have access to them?
access thru the "<< ActiveRecord::Base" inclusion.  "built in"

3. Assume that in your database, a team has the following attributes: "id", "name", owner_id". How would you find the name of a team with an id of 4? Assuming your class only included the code from question 2, how could you find the owner of the same team?
.find(:id/4).name


4. Assume that you added a line to your `Team` class as follows:

```ruby
class Team << ActiveRecord::Base
  belongs_to :owner
end
```

Now how would you find the owner of the team with an id of 4?
.find(:id/4).owner_id.name

5. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
many to many 

6. Define foreign key, primary key, and schema.
F-key: the primary key of another table residing in the current table.  P-key: id for locating rows/values/instances in the current database.  Schema: the structure of the db tables and their columns
7. Describe the relationship between a foreign key on one table and a primary key on another table.
it's the same key linking these two tables together
8. What are the parts of an HTTP response?
verb and path make route 


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
ruby+make=rake db:create - creates the db blob
rake db:create_migration - makes the migration file for creating the structure of the db
rake db:reset - drops and rebuilds the database and re-structures it 
3. What two columns does `t.timestamps null: false` create in our database?
created_at - updated_at
4. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
join table - faculty
5. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
share the primary keys back and forth and insert into the models :belongs_to
6. Give an example of when you might want to store information besides ids on a join table.
When the two tables existence together creates instances of unique things (horrible way of saying it) 
7. Describe and diagram the relationship between patients and doctors.
patient has single doctor - doctor has many patients 
8. Describe and diagram the relationship between museums and original_paintings.
1 to 1 
9. What could you see in your code that would make you think you might want to create a partial?
???
