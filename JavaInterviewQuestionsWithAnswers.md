# 📘 Java Interview Questions & Concepts

This document contains a curated list of Java questions covering core concepts, coding behavior, object-oriented principles, and advanced topics. Use it for revision, mock interviews, or building your own knowledge base.

---

## 🔤 String & Character Operations

1. **Finding the position of a character in a string**  
   _If you wanted to find out where the position of the letter `v` (i.e. return 2) in the string `s` containing `"Java"`, which of the following could you use?_  
   - a) `mid(2,s)`  
   - b) `charAt(2)`  
   - ✅ c) `s.indexOf('v')`  
   - d) `indexOf(s,'v')`

---

## 🔌 JDBC & Database Connectivity

2. **What are all the different ways to get a connection from database by using JDBC?**

---

## ⚠️ Compilation & Syntax Checks

3. **Which of the following lines will compile without warning or error?**  
   - a) `float f = 1.3;` ❌ (1.3 is double by default)  
   - b) `char c = "a";` ❌ (double quotes denote String)  
   - c) `byte b = 257;` ❌ (257 exceeds byte range)  
   - d) `boolean b = null;` ❌ (boolean can't be null)  
   - ✅ e) `int i = 10;`

---

## 🧠 Object Class & Method Overriding

4. **List Object Class methods and explain when to override `equals()` and `hashCode()` methods.**

---

## 🖥️ Command Line Arguments

5. **What will be printed out if this code is run with the following command line?**
```bash
CMD>> java myprog good morning
public class myprog {
    public static void main(String argv[]) {
        System.out.println(argv[2]);
    }
}
```
Runtime error: ArrayIndexOutOfBoundsException because only two arguments are passed (argv[0] = "good", argv[1] = "morning"), but argv[2] is accessed.

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

9. **How does a program destroy an object that it creates?**
10. **What are all the different ways to create an Object in Java Applications?**
11. **What are all the differences between checked exceptions and unchecked exceptions?**
12. **What are all the features of Object-Oriented Model?**
13. **Can you explain clearly how you implemented encapsulation in your project, explain the different ways of implementing encapsulation?**
14. **Can you explain clearly how you implemented encapsulation and abstraction in your project?**
15. **What is constructor?**
