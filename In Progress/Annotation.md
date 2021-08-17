## Built-in annotations

Java defines a set of annotations that are built into the language. Of the seven standard annotations, three are part of [java.lang](https://en.wikipedia.org/wiki/Java.lang "Java.lang"), and the remaining four are imported from java.lang.annotation.[[5]](https://en.wikipedia.org/wiki/Java_annotation#cite_note-5)[[6]](https://en.wikipedia.org/wiki/Java_annotation#cite_note-6)

**Annotations applied to Java code:**

-   `@Override` - Checks that the method is an [override](https://en.wikipedia.org/wiki/Method_overriding "Method overriding"). Causes a [compilation error](https://en.wikipedia.org/wiki/Compilation_error "Compilation error") if the method is not found in one of the [parent classes](https://en.wikipedia.org/wiki/Parent_class "Parent class") or implemented [interfaces](https://en.wikipedia.org/wiki/Interface_(Java) "Interface (Java)").
-   `@Deprecated` - Marks the method as obsolete. Causes a compile warning if the method is used.
-   `@SuppressWarnings` - Instructs the compiler to suppress the [compile time](https://en.wikipedia.org/wiki/Compile_time "Compile time") warnings specified in the annotation parameters.

**Annotations applied to other annotations (also known as "Meta Annotations"):**

-   `@Retention` - Specifies how the marked annotation is stored, whether in code only, compiled into the class, or available at runtime through reflection.
-   `@Documented` - Marks another annotation for inclusion in the documentation.
-   `@Target` - Marks another annotation to restrict what kind of Java elements the annotation may be applied to.
-   `@Inherited` - Marks another annotation to be inherited to subclasses of annotated class (by default annotations are not inherited by subclasses).

Since Java 7, three additional annotations have been added to the language.

-   `@SafeVarargs` - Suppress warnings for all callers of a method or constructor with a [generics](https://en.wikipedia.org/wiki/Generics_in_Java "Generics in Java") [varargs](https://en.wikipedia.org/wiki/Variadic_function "Variadic function") parameter, since Java 7.
-   `@FunctionalInterface` - Specifies that the [type declaration](https://en.wikipedia.org/wiki/Declaration_(computer_programming) "Declaration (computer programming)") is intended to be a [functional interface](https://en.wikipedia.org/wiki/Anonymous_function "Anonymous function"), since Java 8.
-   `@Repeatable` - Specifies that the annotation can be applied more than once to the same declaration, since Java 8.