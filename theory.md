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
 > *Your answer here*
 
 ### What is the conceptual difference between threads and processes?
 > *Your answer here*
 
 ### Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they?
 > *Your answer here*
 
 ### What is the Go-language's "goroutine"? A C/POSIX "pthread"?
 > *Your answer here*
 
 ### In Go, what does `func GOMAXPROCS(n int) int` change? 
 > *Your answer here*



 
 
 
 
