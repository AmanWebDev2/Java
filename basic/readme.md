# Basic

```
class Launch {
    public static void main(String []args) {
        System.out.println("Hello"); //Hellos
    }
}
```
* file must be saved as Launch.java
* then execute :
```
javac <file_name>
java <file_name>
``` 
javac convert the program to bytes code which is not a HLL(High level language) nor LLL(Low level language)

* A .class file will be generate
* byte code is platform independent
* JVM (java virtual machine) is platform dependent, which converts the byte code / .class file into Machine level language
* WORA -> write once run anywhere

* JVM looks for main method.
* public -> outside the class method is visible.
* static -> can access method without creating an instance.
* void -> return type of a function.

### Passing command line arguments

```
java Launch AMAN
```
where aman is passed as a argument which we can access in args

```
class Launch {
    public static void main (String []args) {
        System.out.println(args[0]); // AMAN
    }
}
```

### Ways to write a program.

* public and static are interchangable.
```
 public static void main(String []args) { }
 static public void main(String []args) { }

 static public void main(String args[]) { }
 public static void main(String ...args) { }

```

# Intro to OOPs

* consider everything as an object like pen,paper,mouse,laptop etc.
### steps to create a class

1. Identify object.
2. What its properties and behaviour.
3. Now create a blue print.

eg. Student
Properties: A student has a name, age, gender, etc <br>
Behaviours : A student can sleep, eat, play, study etc.

```
// A blue print

class Student {

    String name;
    int age;
    String gender;

    void sleep() { };
    void eat() { };
    void play() { };

}
//creating a instance
Student a = new Student();
a.play();
```


