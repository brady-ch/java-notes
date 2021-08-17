# Concurrency and Threads

## Key Terms

| Key Terms | description |
|---|---|
| [[#Process]] | A process is a unit of execution that has its own memory space. Each instance of a JVM runs as a process (this isn't true for all JVM implementations but for most of them. Process and application are often used interchangeably.|
| [[#Heap]] | Each Java application has it's own memory space known as a heap, Java applications cannot access the heap of another |
| [[#Threads  \| Thread]] | A thread is a unit of execution within a process. Each process can have multiple threads. In Java, every process has at least one thread (the **main** thread). Nearly every Java process has multiple threads even when we do no create them explicitly, they do things like memory management and I/O. |
| [[#Concurrency]] | The application is making progress on more than one task. One task does not have to complete before making progress on another task. However this does not mean that it is doing multiple tasks at the same time. |

## Keywords

| Keywords | Description |
|---|---|
| synchronized | TODO |
| volatile | TODO |

## Process
- Every Java application runs as a single process, and each process can have multiple threads. Every process has a heap, and every thread has a thread stack.



## Threads
- Creating a thread doesn't require as many resources as creating a process. Every thread created by a process shares the process's memory and files. This can create problems.
- Each thread has  a thread stack, which is memory that only a thread can access. We can run into issues because of this when multiple threads try to access and update a resource at the same time but the data is cached within the thread so when the value of the resource in the main memory is reassigned only one of the updates will have occurred.
- Advantages of multi-threading
	- Allows you to perform asynchronous operations, ones that will take a while like querying a database, or fetching data from the internet. So you will not hold up the main thread while waiting for the completion of the other calls.
	-  An API may require us to provide one.
- Cannot guarantee the order of execution on a thread, it is scheduled by the system

```java
public class ClassName extends Thread{
  public void run(){
    super.run(); // Place the code you want executed here
    //Your Code
  }
}

public class Main{
  public static void main(String[] args){
    ClassName thread = new ClassName();
    thread.start();
  }
}
```

Anonymous Thread Example
```java

public class Main {
	public static void main(String[] args){
	
	new Thread() {
	public void run(){
	// Your code here
		}
	}.start();
	
	}
}

```

