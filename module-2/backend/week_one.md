## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
* POST - Create of CRUD; used to send data to the server via form and in general "creating"
* GET - Read of CRUD; used to when the user will read data; the server responding to a request
* PUT - Update / replace portion of CRUD 
* PATCH - Update / modify portion of CRUD
* DELETE - Destroy of CRUD; deletes record
2. What is Sinatra? 
* A ruby based (written in Ruby) light web framework that allows you to launch a server and post html/css web files to the web with a ruby backend system. Sinatra has a bunch of useful built-in methods and utilizes a "rack" server. 
4. What is MVC?
* Models/Views/Controller file structure. This can be contained within an "app"subdirectory and refers to the conventional functions of the files that are contained within each folder. Models contain ruby classes that create the outline and relationships (belongs_to & has_many) between objects.  
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
* To ensure functionality with SQL, sinatra knows these routes and how to execute them, and it's proper convention for rails moving forward. 
6. What types of variables are accessible in our view templates without explicitly passing them?
* Instance Variables
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    erb :index
  end
  ```

```html
<p><% @count =></p>
```
8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?
9. What's the purpose of ERB?
* ERB is embedded Ruby in an HTML file, denoted by .erb suffix and is used when utilizing "forms" to respond to client requests.
10. Why do I need a development AND test database?
* Databases design convention is to create like a fortress and modify "real" data violates this thinking. So it's best to keep the databases seperate. This allows allows for a much smaller segment of the "real" db but results in faster testing..
11. What's responsive design?
* Responsive design refers to the web page functionality that adjusts images according to the dynamic browser size. This enables better transition to mobile and ease of viewing on any size screen. "Responsive" refers to how the imgage / text box on the browser can adjust size to ensure all content is visible without scrolling left or right, and allows users to simply scroll or down to access of of the current pages's content. 
12. What is CRUD and why is it important?
* Create - Read - Update - Delete is the 4-step functionality for all database ineractions. These functions comprise all the functions to add, view, edit and delete if necessary information from a database.
13. What does HTTP stand for? 
*  Hyper Text Transfer Protocol, and is the standard language for how computers communicate over the internet. 
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
* Via instance variables which would be formated ``` <= @instance_variable > ``` or methods/class relationships ```<%= horse.breed.name %> ```
15. What's an ORM?
* Object Relationship Mapper, 
16. What's the most commonly used ORM in ruby (Sinatra & Rails)?
* ActiveRecord - Datamapper and Sequel are some others but much less common.
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
* Would need to refer to diagram from Jeff's talk but know where the info is located.
18. What's a migration? 
* Builds the rules that determine the "schema" or how data is entered, formatted, and under which names and relationships the data will be stored in the db. 
19. When you create a migration, does it automatically modify your database?
* Create a migration whenever you need to change how the data is entered, stored or related in regards to other tables. This could be adding or deleting a column for new data or foreign key, changing a column name, adjusting data type or format options. 
20. How does a model relate to a database?
* The model outlines relationships between other models and how they can be accessed via built-in ORM methods, provides the relationships between models and stores validation requirements/methods. 
21. What's the difference between agile workflow and waterfall method?
* Agile is an iterative approach that builds and expands upon each previous iteration, and allows for faster implementation of fixes and upgrades and better response to changing development needs. Waterfall is completing each phase of the project (analysis/development/testing/ship) sequentially, which generally takes much longer and cannot respond to changing requirements. 
22. What is the difference between `#new` and `#create`?
