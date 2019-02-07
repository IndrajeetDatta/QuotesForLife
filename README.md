# Software Architecture Design Assignment

**Model View Controller** is a software architecture pattern that is used to implement user interfaces. Therefore, it is commonly used to develop web applications. It separates out application logic into three separate sections:



* **Models** are classes that interact with the database. Any database related actions (such as modifying data before it gets saved inside the database) should be placed here.

* **Controllers** handle decisions from the browser and connect the model with the view. In Rails, controllers are implemented as ActionController classes. The controller should not include any database related actions. This should be handled in the proper model.

* **Views** is the presentation layer which is what the user sees. This displays the output, usually HTML.

* **Routers** map HTTP requests from the browser to a Controller#action via the HTTP verb (GET, POST, PUT, DELETE) and the URI of the HTTP request.
