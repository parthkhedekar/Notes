We can avoid design patterns keeping time constraints or any other constraints but there are 3 design patterns which cannot be avoided also design patterns were introduced for antipatterns 

#### 1.  DRY(Don't Repeat Yourself) : 
	Every piece of knowledge specifically business knowledge should be kept at one place and it should not repeat itself  
	This principle states that every piece of knowledge must have a single, unambiguous, authoritative representation within a system. In simple terms, avoid duplication of logic or code. Repeating code makes the system hard to maintain and error-prone. If a change is required, you might forget to update all occurrences
#### Importance:

- Reduces redundancy
- Easier maintenance
- Single point of change

#### When Not to Use the DRY Principle:

- **Premature Abstraction:** Don't extract common code too early.
    - At first glance, two code blocks might look similar, but they could change in different ways later.
    - Extracting them into a shared method can create unnecessary coupling between unrelated parts.
- **Performance-Critical Code:** Don't apply DRY to performance-sensitive code if it causes inefficiency.
    - Sometimes, repeating optimized low-level logic is faster than calling a generalized, reusable method.
    - Function calls, indirection, or generic wrappers might **reduce performance** or **block compiler optimizations** like inlining.
- **Sacrificing Readability:** If extracting repeated code **makes the code less readable**, prefer clarity over DRYness.
- **Legacy Codebases:** Don't refactor for DRY's sake in legacy code unless necessary and well-tested.
    - Legacy code might not have tests or complete documentation. Introducing DRY by extracting shared logic can accidentally change behavior.
    - Refactoring legacy code safely often follows the "leave it alone unless you must touch it" rule.