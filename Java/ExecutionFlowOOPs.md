# Object Oriented Programming Principles:

# **Major Pillars of OOP in Java**

## **1. Abstraction**

Abstraction means **showing only the required information and hiding unnecessary details**.

### Key Points:

- **Focus on what, not how.**
- **DAO Layer** → Exposes only required fields instead of the whole table.
    
- **Abstract Classes & Interfaces** → Define behavior without providing complete implementation.
    

### Examples:

- Using a method `startEngine()` without knowing how the engine starts internally.
    
- Hiding complex logic behind APIs.
    

---

## **2. Encapsulation**

Encapsulation means **binding data and the methods that operate on that data within a class**, and **restricting direct access** using access modifiers.

### Key Points:

- A class binds **data members + member functions**.
    
- `private` fields + `public` getters/setters protect data.
    
- Java internally encapsulates libraries in **JMODS** (currently) and **rt.jar** (before Java 9).
    
- Every time you **create a class**, you're encapsulating data and logic inside a single unit.
    

### Example:

`class Student {     private String name;     public String getName() { return name; } }`

---

## **3. Modularity**

Modularity means **organizing code into separate, logical units**, making it easier to manage, understand, and maintain.

### Key Points:

- Keep everything arranged in **separate files / components / packages**.
    
- Java modules (Jigsaw Project) introduced **JMOD files** → a real-world example of good modular design.
    
- Helps in:
    
    - Reusability
        
    - Maintainability
        
    - Scaling the code
        

### Example:

- Separate packages for `controllers`, `services`, `repository`.
    

---

## **4. Hierarchy**

Hierarchy establishes **relationships between classes / objects** and supports **code reusability**.

### Two main types:

---

### **i. Association (Has-A Relationship)**

→ A class contains another class as a dependency.  
→ Achieved by **creating an object of one class inside another**.

**Example:**

`class Car {     Engine engine = new Engine(); // Car HAS-A Engine }`

---

### **ii. Inheritance (Is-A Relationship)**

→ A child class inherits properties and behaviors of a parent class.  
→ JVM automatically includes the parent object inside the child.

**Example:**

`class Animal {} class Dog extends Animal {} // Dog IS-A Animal`

---

If you want, I can convert this entire thing into a **perfect markdown file** ready for your notes.

##### You said:

yes

###### ChatGPT said:

Here is the **clean, crisp, interview-ready Markdown file** exactly the way you’d want it in your notes.

---

# **Major Pillars of OOP in Java**

## **1. Abstraction**

Abstraction means **showing only the necessary information and hiding unnecessary internal details**.

### ✅ Key Points

- Focuses on **what the object does**, not how it does it.
    
- **DAO Layer** → Exposes only required fields instead of the entire table.
    
- **Abstract Classes & Interfaces** define behavior without providing full implementation.
    

### ✅ Example

`interface Vehicle {     void start(); // What to do, not how }`

---

## **2. Encapsulation**

Encapsulation means **binding data (variables) and methods (functions) into a single unit (class)** and controlling access to them.

### ✅ Key Points

- Class binds **data members + member functions**.
    
- Achieved using:
    
    - `private` fields
        
    - `public` getters/setters
        
- Protects the internal state of an object.
    
- Java internally encapsulates libraries using:
    
    - **JMOD files** (Java 9+)
        
    - **rt.jar** (prior to Java 9)
        
- Every time you **create a class**, you're implementing encapsulation.
    

### ✅ Example

`class Student {     private String name; // hidden data      public String getName() {          return name;      } }`

---

## **3. Modularity**

Modularity means **organizing code into separate, independent modules/files**, making the system scalable and maintainable.

### ✅ Key Points

- Keeps code clean, structured, and easy to manage.
    
- Achieved by:
    
    - Packages
        
    - Class separation
        
    - Layered architecture (Controller-Service-DAO)
        
- Java uses **JMODS** as a real-world example of modular structure.
    

### ✅ Example (Package Structure)

`com.project.controller com.project.service com.project.repository com.project.model`

---

## **4. Hierarchy**

Hierarchy defines **relationships between different classes** and supports **code reusability**.

---

### **i. Association (HAS–A Relationship)**

A class contains or uses another class.

### ✅ Key Points

- Achieved by creating an object of one class inside another.
    
- Represents dependency between two entities.
    

### ✅ Example

`class Car {     Engine engine = new Engine(); // Car HAS-A Engine }`

---

### **ii. Inheritance (IS–A Relationship)**

A child class acquires the properties and behaviors of a parent class.

### ✅ Key Points

- Establishes hierarchy.
    
- Promotes code reusability.
    
- JVM automatically includes the parent behavior inside the child.
    

### ✅ Example

`class Animal {} class Dog extends Animal {} // Dog IS-A Animal`
#### Minor Pillars :
	1. Typing / Polymorphism 
	2. Concurrency
	3. Persistence
	
Java is an object oriented language with everything is stored or used as class or object just here the exception is primitive datatypes but for this we have wrapper classes 

OOPs has 2 basic principles :- 

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
	

