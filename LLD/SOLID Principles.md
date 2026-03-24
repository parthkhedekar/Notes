### 1. Single Responsible Principle (SRP) : 
	In easy words a function , classs an entity should have only one purpose to do like 

	A class should have only one reason to change. In other words, a class should only have one job, one responsibility, and one purpose.  
  
	If a class takes more than one responsibility, it becomes coupled. This means that if one responsibility changes, the other responsibilities may also be affected, leading to a ripple effect of changes throughout the codebase.

## Advantages of SRP

- **Improved Maintainability:** Changes in one part of the system won't affect other parts, making it easier to maintain and update.
- **Enhanced Readability:** Smaller, focused classes are easier to read and understand.
- **Better Reusability:** Classes with a single responsibility can be reused in different contexts without bringing unnecessary dependencies.
- **Facilitates Testing:** Smaller classes are easier to test, as they have fewer dependencies and responsibilities.
- **Lower Risk in Changes:** Since each class handles only one concern, changes made to it are less likely to cause unintended side effects in other parts of the system.

  

---

## Common Mistakes When Violating SRP

There are a few common mistakes that developers make when violating the Single Responsibility Principle (SRP). Here are some examples:  

- **Mixing Database Logic with Business Logic:** Putting both data access (e.g., SQL, JDBC) and core business rules in the same class. This makes it hard to change the database layer without affecting business logic.
- **Coupling UI Code with Business Logic:** Embedding application logic directly in the UI layer. This makes it tedious to change the UI without affecting the underlying logic.

### 2. Open Close Principle (OCP)
	As per OCP, Software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification.  
	This means that the behavior of a module can be extended without modifying its source code. The goal is to reduce the risk of breaking existing functionality when requirements change.
	example : while travelling we will change the extension of plug not the charger when the socket changes 