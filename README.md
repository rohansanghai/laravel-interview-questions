# Laravel interview questions

List of laravel interview question which are most widely asked.

> Click :star:if you like the project. Pull Requests are highly appreciated.

### Table of Contents
-------------------------------------------------------------------
| No. | Questions |
|---- | ---------
|1  | [What are the Laravel events?](##what-are-the-laravel-events) |
|2  | [What is service providers in Laravel?](#what-is-service-providers-in-laravel) |
|3  | [How you will register ServiceProvider?](#how-you-will-register-serviceprovider)|
|4  | [What is Service Container in Laravel?](#)|
|5  | [How you will inject dependency in class level/Explain Dependency Injection in Laravel?](#)|
|6  | [What is Laravel Contracts?](#)|
|7  | [What are Laravel Facades?](#)|
|8  | [Explain the Laravel Eloquent Model?](#)|
|9  | [What is the queue in Laravel?](#)|
|10 | [How can we enable a query log?](#)|
|11 | [What is Traits in Laravel?](#)|
|12 | [What is Middleware in Laravel?](#)|
|13 | [How to check the request is AJAX or not?](#)|
|14 | [How can you reduce memory usage in Laravel?](#)|
|15 | [Which class is used to handle exceptions?](#)|
|16 | [Explain faker in Laravel?](#)|
|17 | [How will you check table is exists or in the database?](#)|
|18 | [What is the significant difference between insert() and insertGetId() function in Laravel?](#)|
|19 | [Explain Laravel guard?](#)|
|20 | [The relationship used in Laravel?](#)|
|21 | [What are the aggregate methods provided by Laravel?](#)|
|22 | [What is namespace in Laravel?](#)|
|23 | [Explain Loggin in Laravel?](#)|
|24 | [Define hashing in Laravel?](#)|
|25 | [Please write some additional where Clauses in Laravel?](#)|

1.  ### What are the Laravel events?
    Laravel events provide simple observer implementation, allowing you to subscribe and listen to various events that occur in your application.events classes are stored in app/Events dictionary & listeners are stored in the app/Listeners dictionary. They will create when using artisan console for Events & Listeners.
    
    **[⬆ Back to Top](#table-of-contents)**
    
2.  ### What is service providers in Laravel?
    Service providers are the central place where your application is bootstrapped. Laravel core services also bootstrapped by service providers. All service providers extend Illimunate\Support\ServiceProvider class. Which contains the boot and register method.
    
    **[⬆ Back to Top](#table-of-contents)**
    
3.  ### How you will register ServiceProvider?
    You can register service providers in the config/app.php configuration file that contains an array where you can mention the service provider class name.
    
    **[⬆ Back to Top](#table-of-contents)**
    
4.  ### What is Service Container in Laravel?
    It is useful in resolving class dependencies and performing dependency injection in Laravel. Dependency - class dependencies are “injected” into the class via the constructor or, in some cases, “setter” methods.
    
    **[⬆ Back to Top](#table-of-contents)**
    
5.  ### How you will inject dependency in class level / Explain Dependency Injection in Laravel?
    Dependency injection is a technique whereby one object supplies the dependencies of another object. A dependency is an object that can be used (a service). You can do dependency injection via Constructor, setter and property injection.
    
    **[⬆ Back to Top](#table-of-contents)**
    
6.  ### What is Laravel Contracts?
    Laravel contract is a set of interfaces that define core services provided by the Laravel framework.
    
    **[⬆ Back to Top](#table-of-contents)**
    
7.  ### What are Laravel Facades?
    Laravel facades are nothing but interfaces, that are available in the application service provider.
    
    **[⬆ Back to Top](#table-of-contents)**
    
8.  ### Explain the Laravel Eloquent Model?
    Laravel's Eloquent ORM is a simple Active Record implementation for working with your database.
    
    **[⬆ Back to Top](#table-of-contents)**
    
9.  ### What is the queue in Laravel?
    The Laravel queue service provides a unified API across a variety of different queue back-ends. Queues allow you to defer the processing of a time-consuming task, such as sending an e-mail, until a later time which drastically speeds up web requests to your application. Queue driver used - Redis server.
    
    **[⬆ Back to Top](#table-of-contents)**
    
10. ### How can we enable a query log?
    DB::connection()->enableQueryLog();
    
    **[⬆ Back to Top](#table-of-contents)**

11. ### What is Traits in Laravel?
    Traits are a simple group of methods that you want to include in another class. A Trait, like an abstract class, cannot be instantiated by itself. The trait is created to reduce the limitations of single inheritance in PHP by enabling a developer to reuse sets of methods freely in several independent classes living in different class hierarchies.
    
    **[⬆ Back to Top](#table-of-contents)**
    
12. ### What is Middleware in Laravel?
    Acts middle man between request and response.
    Two types -
      Global Middleware - It will apply to every route request.
      Route Middleware - It is applicable for a particular route.
      
    **[⬆ Back to Top](#table-of-contents)**
     
13. ### How to check the request is AJAX or not?
    we can use $request->ajax() method to check request is ajax or not.
    
    **[⬆ Back to Top](#table-of-contents)**
    
14. ### How can you reduce memory usage in Laravel?
    While processing a large amount of data, you can use the cursor method in order to reduce memory usage.
    
    **[⬆ Back to Top](#table-of-contents)**
    
15. ### Which class is used to handle exceptions?
    Laravel exceptions are handled by App\Exceptions\Handler class.
    
    **[⬆ Back to Top](#table-of-contents)**
    
16. ### Explain faker in Laravel?
    It is a type of module or packages which is used to create fake data. This data can be used for testing purposes. It is can also be used to generate: 1) Numbers, 2) Addresses, 3) DateTime, 4) Payments, and 5) Lorem text.
    
    **[⬆ Back to Top](#table-of-contents)**
    
17. ### How will you check table is exists or in the database?
    Use hasTable() Laravel function to check the desired table is exists in the database or not.
    
    **[⬆ Back to Top](#table-of-contents)**
    
18. ### What is the significant difference between insert() and insertGetId() function in Laravel?
    Insert(): This function is simply used to insert a record into the database. It not necessary that ID should be autoincremented.
    InsertGetId(): This function also inserts a record into the table, but it is used when the ID field is auto-increment.
    
    **[⬆ Back to Top](#table-of-contents)**
    
19. ### Explain Laravel guard?
    Laravel guard is a special component that is used to find authenticated users. The incoming requested is initially routed through this guard to validate credentials entered by users. Guards are defined in ../config/auth.php file.
    
    **[⬆ Back to Top](#table-of-contents)**
    
20. ### The relationship used in Laravel?
    One To One
    One To Many
    One To Many (Inverse)
    Many To Many
    Has Many Through
    Polymorphic Relations
    Many To Many Polymorphic Relations
    
    **[⬆ Back to Top](#table-of-contents)**

21. ### What are the aggregate methods provided by Laravel?
    count()
    max()
    min()
    avg()
    sum()
    
    **[⬆ Back to Top](#table-of-contents)**
   
22. ### What is namespace in Laravel?
    A namespace allows a user to group the functions, classes, and constants under a specific name.
    
    **[⬆ Back to Top](#table-of-contents)**

23. ### Explain Loggin in Laravel?
    It is a technique in which system log generated errors. Loggin is helpful to increase the reliability of the system. Laravel supports various logging modes like Syslog, daily, single, and error log modes.
    
    **[⬆ Back to Top](#table-of-contents)**

24. ### Define hashing in Laravel?
    It is the method of converting text into a key that shows the original text. Laravel uses the Hash facade to store the password securely in a hashed manner.
    
    **[⬆ Back to Top](#table-of-contents)**

25. ### Please write some additional where Clauses in Laravel?
    Laravel provides various methods that we can use in queries to get records with our conditions.
    These methods are given below
    where()
    orWhere()
    whereBetween()
    orWhereBetween()
    whereNotBetween()
    orWhereNotBetween()
    wherein()
    whereNotIn()
    orWhereIn()
    orWhereNotIn()
    whereNull()
    whereNotNull()
    orWhereNull()
    orWhereNotNull()
    whereDate()
    whereMonth()
    whereDay()
    whereYear()
    whereTime()
    whereColumn()
    orWhereColumn()
    whereExists()
    
    **[⬆ Back to Top](#table-of-contents)**
