# Software Architecture Design Assignment

## Team Members
* **Indrajeet Datta** st120644
* **Jithendra Prasad** st120688
* **Greeshma Ravula** st120681

* **Model View Controller** is a software architecture pattern that is used to implement user interfaces.  It separates out application logic into three separate sections:



* **Models** are classes that interact with the database. Any database related actionsshould be placed here.

* **Controllers** handle decisions from the browser and connect the model with the view. In Rails, controllers are implemented as ActionController classes. The controller should not include any database related actions. This should be handled in the proper model.

* **Views** is the presentation layer which is what the user sees. This displays the output, usually HTML.

* **Routers** map HTTP requests from the browser to a Controller#action via the HTTP verb (GET, POST, PUT, DELETE) and the URI of the HTTP request.

![mvc](https://www.javacodegeeks.com/wp-content/uploads/2017/09/mvc.png)

We created a simple web-application call "Quotes for Life" in which the users` can share interesting phylosophical quotes in our web-application.

Our application supports all CRUD operations. i.e
 * **Create**
 * **Read**
 * **Update**
 * **Delete**
 
 

In the web-app we had to define 
* 7 Routes
* 1 controller with 7 actions
* 4 view templates
* 1 Model 

* **Controller** (articles_controller.rb)
![controller](https://i.imgur.com/hQUF05F.png)
![controller](https://i.imgur.com/ZvAE2qD.png)

* **Views** 
 Index View
 ![view](https://i.imgur.com/fJZVFoR.png)
 ![view](https://i.imgur.com/WlkZ97U.png)
 
 Final Homepage in the browser
  ![home]( https://i.imgur.com/2ramnkh.png)
