# Methods
- A method is a block of code which only runs when it is called.
- Methods are a way to write DRY code
- A method is a collection of statements that return a value upon execution, unless the keyword void is added to the method declaration
- Methods are inherited by child classes



## Method Overloading
Method overloading is providing two separate methods in a class with the same name but different arguments, while the method return type may or may not be different, which allows us to reuse the same method name. However please note that when overloading a method just changing the return type is not enough, you must change the parameters in some way, even if it is changing the order they are added.

```java
public class huhkay{

public String getHuh(String huh){
return huh;
}

public String getHuh(String huh, int kay){
return huh + kay;
}

public String getHuh(int kay, String huh){
return huh + kay;
}

public int getHuh(int huh){
return huh;
}

}
```

## Method Overriding
Method overriding means defining a method in a child class that is already defined in the parent class with the same method signature, same name, arguments, and return type
```java

// A Simple Java program to demonstrate
// method overriding in java
  
// Base Class
class Parent {
    void show()
    {
        System.out.println("Parent's show()");
    }
}
  
// Inherited class
class Child extends Parent {
    // This method overrides show() of Parent
    @Override
    void show()
    {
        System.out.println("Child's show()");
    }
}
  
// Driver class
class Main {
    public static void main(String[] args)
    {
        // If a Parent type reference refers
        // to a Parent object, then Parent's
        // show is called
        Parent obj1 = new Parent();
        obj1.show();
  
        // If a Parent type reference refers
        // to a Child object Child's show()
        // is called. This is called RUN TIME
        // POLYMORPHISM.
        Parent obj2 = new Child();
        obj2.show();
    }
}
```