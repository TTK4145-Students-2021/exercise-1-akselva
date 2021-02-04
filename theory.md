Exercise 1 - Theory questions
-----------------------------
 
 ### What is the difference between concurrency and parallelism?
 > Concurrency means working on different tasks in the same timespan, i.e. starting on a task before another one is finished, and switching between them.
 This allows us to make progress in different tasks in the same time peried. However, only one task may be processed at one exact time.
 
 > Parallelism means working on different tasks simultaneously, i.e. at the same exact time. For instance can an application split a single task into subtask that separate
 cores can execute in parallell
 
 ### Why have machines become increasingly multicore in the past decade?
 > Running large multi-thread programs on a single core is possible, however when the complexity and number of threads increase, there becomes a sizeable overhead in terms of
 OS logic. Multi-core machines can therefore greatly increase the efficiency of running multi-threaded programs.
 
 ### Why do we divide software (programs) into concurrently executing parts (like threads or processes)?
 (Or phrased differently: What problems do concurrency help in solving?)
 > Concurrency increases efficiency by maximizing the amount of time the CPU is fully utilized, as different programs can run ~at the same time on the same processor
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > Concurrency increases efficiency, but it also increases the complexity of a program beacause it has to be written in such a way as to maintain data integrity, i.e. making sure that multiple threads are not trying to read from an write to the same memory block at the same time.
 
 ### What is the conceptual difference between threads and processes?
 > Processes cannot share memory with other processes, while threads can. A single process typically contains many threads.
 
 ### Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they?
 > Fibers are threads that use "cooperative scheduling" instead of "pre-emptive scheduling". This means that instead of having a scheduler decide which threads to run at
 specific times, the fibers "take" and "yield" control over resources themselves, essentially cooperating between eachother to produce a functional scheduling system.
 
 ### What is the Go-language's "goroutine"? A C/POSIX "pthread"?
 > Goroutines are GO-functions -and methods that can run concurrently with eachother, i.e. very lightweight threads. 
 
 ### In Go, what does `func GOMAXPROCS(n int) int` change? 
 > GOMAXPROCS sets a limit to the number of OS threads that can execute simultaneously.



 
 
 
 
