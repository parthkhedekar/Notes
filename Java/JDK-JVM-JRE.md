# ☕ Java — Write Once, Run Anywhere

Java’s famous principle **“Write Once, Run Anywhere”** is possible because of the **JVM (Java Virtual Machine)**.  
When Java code is compiled, it becomes **platform-independent bytecode**, which can run on any machine that has a compatible JVM.

---

## 🧩 Components Overview

|Component|Contains|Purpose|
|---|---|---|
|**JDK**|JRE + Development Tools|For developing Java programs|
|**JRE**|JVM + Libraries|For running Java programs|
|**JVM**|Executes Bytecode|Converts bytecode to machine code|

---

## 🧠 **JDK – Java Development Kit**

The **JDK** is the full-featured software development kit for Java.  
It provides everything needed to **write, compile, and debug** Java programs.

**Includes:**

- **JRE**
    
- **Development Tools** (e.g., `javac`, `java`, `jar`, `javadoc`)
    

**Summary:**

`JDK = JRE + Development Tools`

**Example:**  
When you run

`javac MyClass.java`

the **JDK compiler** converts your `.java` file into **bytecode** (`.class` file).

---

## ⚙️ **JRE – Java Runtime Environment**

The **JRE** provides the **runtime environment** required to run Java programs.  
It includes:

- The **JVM**
    
- **Core Java Libraries** (helper classes, built-in APIs)
    
- **Configuration files**
    

**Summary:**

`JRE = JVM + Libraries + Runtime Files`

**Example:**  
When you run

`java MyClass`

the **JRE** ensures the JVM and required libraries execute your program.

---

## 🖥️ **JVM – Java Virtual Machine**

The **JVM** is the engine that actually **executes the Java bytecode**.  
It translates bytecode into **machine code** for the host system.

**Responsibilities:**

- Bytecode execution
    
- **Memory Management (Garbage Collection)**
    
- **Class Loading**
    
- **Security & Exception Handling**
    

**Key Point:**

- The **JVM** is _platform-dependent_
    
- The **bytecode** it runs is _platform-independent_
    

---

## 🔁 **Relationship Diagram**

 
---

## ✅ **In Summary**

`JDK = JRE + Development Tools JRE = JVM + Libraries JVM = Executes Bytecode (Platform Dependent)  → “Write Once, Run Anywhere” is possible because JVM runs the same bytecode on any OS that has a compatible JVM.`

---