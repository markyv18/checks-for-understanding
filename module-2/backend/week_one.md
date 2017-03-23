## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb. GET PUT POST DELETE PATCH
2. What is Sinatra? - library for ruby (not a full framework)
4. What is MVC? model - view - controller navigation of front/back end of websites
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes? better set up, easier flow and organization
6. What types of variables are accessible in our view templates without explicitly passing them? instance variables
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
 @count = 1 (inserted between line 15 and 16) 
  ```ruby
  get '/horses' do
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?
explicitily list it out in the erb "locals: "

9. What's the purpose of ERB? giving front end access to back end data

10. Why do I need a development AND test database?
smaller, faster, dont mess with main db
11. What's responsive design?
CSS that adapts to size of screen or windo
12. What is CRUD and why is it important?
method to follow for building out functionality 
13. What does HTTP stand for? hyper text transfer protocol 
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways? <%= =>  (dont know the other)
15. What's an ORM?  object relational mapping 
16. What's the most commonly used ORM in ruby (Sinatra & Rails)?  active record
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
get new   post new    get show   put show   delete show   get all 
18. What's a migration?   sets up tables in db
19. When you create a migration, does it automatically modify your database?  gotta rake it first?
20. How does a model relate to a database?  brings the data into a manipulatible form (each row) 
21. What's the difference between agile workflow and waterfall method?   agile circular, waterfall linear
22. What is the difference between `#new` and `#create`? 
new is an instance, create is an instance tied to the database 
