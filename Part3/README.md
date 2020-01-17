# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to a repository to complete the task. Remember to also submit your answers to Blackboard

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency is when you have the ability to complete to tasks in the same overlapping timespace. This does not mean that the tasks are handled simultaneously but rather that parts of the first task is done while the second one is paused and vice a versa.
 
 > Parallelism is similarily to concurrency about two tasks being completed in the same overlapping timespace. However now they are being completed simultaneously.
 
 > The difference can be seen through an analogy. You have to clean your house. This consists of doing the dishes and vacuuming the floors. Concurrency would mean in practice that you would do some of the dishes, stop and start vacuuming the living room, do some more dishes, then vacuum the kitchen, do some more dishes, vacuum the attic and so on. Parallellism however would mean you are doing the dishes WHILE vacuuming the house. Both tasks are done simultaneously.
 
 ### Why have machines become increasingly multicore in the past decade?
 > Due to oower limitations we cannot increase clock speed in CPUs so we have to work around this by increasing the number of cores instead.
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > Concurrency lets you do tasks while waiting for certain other tasks to finish. This is useful in decoupled routines.
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > Both. You can do stuff independently very easy, but it becomes a hassle to share common resources between threads.
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > Process: an instance of a program that is independent from the rest of the program. It has it's own location in memory
 
 > Thread: A sequence of instructions. These are scheduled by the OS
 
 > Green Thread: A Thread scheduled not by the OS, but by a third oarty app.
 
 > Coroutines: These are the same as threads but has the ability to work together to multitask and are not managed by the OS.
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > in that order:
 
  > pthread_create() creates a new thread.
  > threading.Thread() creates a new thread using pthread_create()
  > go creates a green thread.
  
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > *Your answer here*
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > *Your answer here*
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > *Your answer here*
