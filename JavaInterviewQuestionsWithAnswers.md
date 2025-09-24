# 📘 Java Interview Questions & Concepts

This document contains a curated list of Java questions covering core concepts, coding behavior, object-oriented principles, and advanced topics. Use it for revision, mock interviews, or building your own knowledge base.

---
## String & Character Operations
1. **Finding the position of a character in a string**  
   _If you wanted to find out where the position of the letter `v` (i.e. return 2) in the string `s` containing `"Java"`, which of the following could you use?_  
   - a) `mid(2,s)`  
   - b) `charAt(2)`  
   - ✅ c) `s.indexOf('v')`  
   - d) `indexOf(s,'v')`  
   
## JDBC & Database Connectivity
2. **What are all the different ways to get a connection from a database by using JDBC?**

## Compilation & Syntax Checks
3. **Which of the following lines will compile without warning or error?**  
   - a) `float f = 1.3;` ❌ (1.3 is double by default)  
   - b) `char c = "a";` ❌ (double quotes denote String)  
   - c) `byte b = 257;` ❌ (257 exceeds byte range)  
   - d) `boolean b = null;` ❌ (boolean can't be null)  
   - ✅ e) `int i = 10;`

## Command Line Arguments
5. **What will be printed out if this code is run with the following command line?**
```bash
CMD>> java myprog good morning
public class myprog {
    public static void main(String argv[]) {
        System.out.println(argv[2]);
    }
}
```
6. **What will happen if you try to compile and run the following code?**
```bash
    public class Q { 
        public static void main(String argv[]){ 
            int anar[]=new int[5];
            System.out.println(anar[0]);
        }
    }
```
7. **What will happen if you try to compile and run the following code?**
```bash
public class MyClass {
    public static void main(String arguments[]) {
        amethod(arguments);
    }
    public void amethod(String[] arguments) {
        System.out.println(arguments);
        System.out.println(arguments[1]);
    }
}
```
8. **What will be the result of attempting to compile and run the following code?**
```bash
abstract class MineBase {
    abstract void amethod();
        static int i;
    }
    public class Mine extends MineBase {
        public static void main(String argv[]){
            int[] ar=new int[5];
            for(i=0;i < ar.length;i++)
                System.out.println(ar[i]);
        }
    }
```

## Object Class & Method Overriding
4. **List Object Class methods and explain when to override `equals()` and `hashCode()` methods.**

## Object Creation & Management
9. **How does a program destroy an object that it creates?**
10. **What are all the different ways to create an Object in Java Applications?**
11. **What are all the differences between checked exceptions and unchecked exceptions?**
12. **What are all the features of the Object-Oriented Model?**
13. **Can you explain clearly how you implemented encapsulation in your project, explain the different ways of implementing encapsulation?**
14. **Can you explain clearly how you implemented encapsulation and abstraction in your project?**
15. **What is a constructor?**
16. **What are all the rules for constructors?**
17. **How many constructors can you write inside a single class?**
18. **I have around 30 constructors inside a single class, how can you call the 21st constructor inside the 15th constructor?**
19. **What are the differences between overloading and overriding?**
20. **Can you tell me the difference between an array and the collection framework?**
21. **What is cloning and the different types of cloning?**
22. **Can you tell me the difference between shallow copy and deep copy?**
23. **What is a static block, and how many static blocks can we write inside a single class?**
24. **I have static blocks, instance blocks, and a main method present inside a class; what is the order of execution?**
25. **What is SCP (String Constant Pool)?**
26. **What is auto boxing and auto unboxing?**
27. **Can you tell me something about the AutoCloseable interface?**
28. **Can you tell me something about try-with-resources?**
29. **What are all the different ways to fetch the data from collection interfaces/classes?**
30. **I want to store IPL League Franchise names in an order; which collection would you prefer to use?**