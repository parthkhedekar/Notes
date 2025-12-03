# Object Oriented Programming Principles:

Java is an object oriented language with everything is stored or used as class or object just here the exception is primitive datatypes but for this we have wrapper classes 

**OOPs has 2 basic principles** :- 

	1. Class:
		a. Class is a logical entity 
		b. consists of data members and methods 
		c. methods can be static , non-static (Static can be accessed through class
		 names while for non static classes needs to be accessed by creating
		 objects )
		d. also called as user defined datatype
		
	2. Object:
		a. a physical entity 
		b. just an instance of class
		c. one class can have multiple objects
		d. in java to create a object we need new operator
	

#### Major pillars :
	1. Abstraction
		a. Getting to know only required information
		b. DAO layer where we are only exposing required fields not whole table 
		c. Abstract Classes and Interfaces (They define behaviour without actual implementation)
	2. Encapsulation
		a. Binding data and code together
		b. class binds data members and member functions
		c. Jmods or rtJar (Java internally stores its helper classes or libraries in jmod currently priorly in rt.jar)
		d. creating a class
	3. Modularity
		a. Modularity is just keeping everything arranged and in seperate files 
		b. jmods is good example where java has arranged everything in modules
	4. Hierarchy
		a. it justs represents code reusability and establishes relationship between 2 entities  
		b. it is further subdivided in:
			i.  Association (Having Has - A Relationship)
				a. Creating object of dependency class inside the dependent class.
				(Car Has a Engine {})
			ii. Inheritence (Having Is - A Relationship)
				a. Object of parent class created automatically inside the child
				class
#### Minor Pillars :

	1. Typing / Polymorphism 
		a. Polymorphism is having code in different forms 
		b. is further divided in 2 types
			i.  Runtime Polymorphism (Method overriding)
				a. is decided at the time of runtime by JVM
				b. the same function is overrided in child classes  and the child 
				function is called when the object of child class is created 
				irrespective of the reference created
			ii. Compiletime Polymorphism (Method overloading)
				a. is decided at the time of compilation
				b. name mangling is concept on which it is working 
				c. for overloading number of parameters, sequence of parameters,
				 and data types of parameters can be changed and method 
				 overloading works
	2. Concurrency
		a. Number of processes threads that can work concurrently
		b. Java Supports multi threading
	3. Persistence
		a. keeping data persisted 
		b. Java Supports persistence through Java I/O and jdbc also various topics 
	




