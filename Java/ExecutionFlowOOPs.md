# Object Oriented Programming Principles:

Java is an Object-Oriented Programming language where almost everything is treated as a **class** or **object**.  
**Exception:** Primitive data types (int, float, boolean…). Java provides **Wrapper Classes** (Integer, Float, Boolean…) to treat primitives as objects when needed.

---
# **Basic OOP Principles**
## **1. Class**
- A **logical entity**.
- Contains **data members (fields)** and **methods**.
- Methods can be:
    - **Static** → accessed using class name.    
    - **Non-static** → accessed via object.
- Also called **User-Defined Datatype**.
- Blueprint for creating objects.
---

## **2. Object**

- A **physical entity** in memory.
    
- An **instance of a class**.
    
- One class → multiple objects.
    
- Created using the **`new` operator** (except via reflection, cloning, deserialization).
    

---

# **Major OOP Pillars**

## **1. Abstraction**

- Showing only the **necessary** details and hiding the internal implementation.
    
- Examples:
    
    - **DAO layer** (exposing only required fields, hiding database structure).
        
    - **Abstract Classes** & **Interfaces** → define behavior without implementation.
        
- Benefits: Simplicity, reduced complexity, security.
    

---

## **2. Encapsulation**

- **Binding data + methods** that operate on the data into a single unit (class).
    
- Fields are made **private**, accessed via **getters & setters**.
    
- Examples:
    
    - Java modules (**jmod** in Modern JDK) or earlier **rt.jar** (Java library packaging).
        
    - Creating a class with private fields.
        

---

## **3. Modularity**

- Organizing code into **separate, manageable modules/files**.
    
- Improves maintainability & readability.
    
- Java uses **Jigsaw (Java Modules)** → `.jmod` files.
    

---

## **4. Hierarchy** (Relationship + Reusability)

Hierarchy expresses **relationships** between objects & code reuse.

### **i. Association** (Has-A Relationship)

- One class uses another by creating its object.
    
- Example:
    
    `class Car {     Engine e = new Engine();   // Car HAS-A Engine }`
    

### **ii. Inheritance** (Is-A Relationship)

- Child class inherits fields/methods of parent.
    
- Parent class object is not created physically inside child, but **child gets access to parent members**.
    
- Supports **code reuse** & **method overriding**.
    

---

# **Minor OOP Pillars**

## **1. Typing / Polymorphism**

Polymorphism → **"many forms"** of the same method or reference.

### **i. Runtime Polymorphism (Method Overriding)**

- Decided at **runtime** by JVM.
    
- Same method name & signature in child and parent.
    
- Actual method called depends on **object**, not reference.
    

### **ii. Compile-time Polymorphism (Method Overloading)**

- Decided at **compile time**.
    
- Works on **name mangling** (compiler-generated method signatures).
    
- Achieved by changing:
    
    - Number of parameters
        
    - Type of parameters
        
    - Order of parameters
        

---

## **2. Concurrency**

- Ability to execute **multiple threads** concurrently.
    
- Java provides:
    
    - `Thread` class
        
    - `Runnable` interface
        
    - Executors, thread pools
        
- Enables parallelism and better CPU utilization.
    

---

## **3. Persistence**

- Keeping data **stored/saved** beyond program execution.
    
- Supported via:
    
    - **Java I/O**
        
    - **Serialization**
        
    - **JDBC**
        
    - External frameworks (Hibernate, JPA)