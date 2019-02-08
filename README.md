# Software Architecture Design Assignment

## Team Members
* **Indrajeet Datta** st120644
* **Jithendra Prasad** st120688
* **Greeshma Ravula** st120681

* **Model View Controller** is a software architecture pattern that is used to implement user interfaces. Therefore, it is commonly used to develop web applications. It separates out application logic into three separate sections:



* **Models** are classes that interact with the database. Any database related actions (such as modifying data before it gets saved inside the database) should be placed here.

* **Controllers** handle decisions from the browser and connect the model with the view. In Rails, controllers are implemented as ActionController classes. The controller should not include any database related actions. This should be handled in the proper model.

* **Views** is the presentation layer which is what the user sees. This displays the output, usually HTML.

* **Routers** map HTTP requests from the browser to a Controller#action via the HTTP verb (GET, POST, PUT, DELETE) and the URI of the HTTP request.

We created a simple web-application call "Quotes for Life" in which the users` can share interesting phylosophical quotes in our web-application.

Our application supports all CRUD operations. i.e
 * **Create**
 * **Read**
 * **Update**
 * **Delete**
 
 

In the web-app we had to define 
* 1 controller with 7 actions
* 4 view templates
* 1 Model 
First, we had to configure the Rails router in (config/routes.rb). Rails has a `resources` method which can be used to declare a standard REST resource:

So our *routes.rb* file looks like this

`Rails.application.routes.draw do
  resources :articles
  root "articles#index"
end`

Then, we entered `$ rake routes` in the Terminal and we can see the 7 routes generated:
#index, #create, #new, #edit, #show, update, #destroy

Then, we generated the controller by using the command
`$rails generate controller Articles`
