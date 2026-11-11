
Q1:
 newSingleThreadContext creates CoroutineDispatcher that confines
 all coroutines launched within it's context to a single dedicated
 thread.

 Dispatchers.Unconfined in Kotlin coroutines is a coroutine dispatcher
 that isnot confined to any specific thread.It offers a distinct
 execution model compared to other dispatchers like 
 Dispatchers.Default
 Dispatchers.IO
 Dispatchers.Main

 Q2:

 .launch() returns a Job handle.Use this handle to wait for 
 the launched coroutine to complete.For more information,see
 Cancellation and timeouts. join() suspends untill the job
 completes

 .async() corouutine builder function is an extension function
 on coroutineScope. it starts a concurrent computation inside 
 an existing coroutine scope and returns a Deferred handle 
 that represents an eventual result

   Q3:

   by marking functions with the suspend keyword,you allow 
   them to call other susoending functions and run concurrent
   code inside 

runBlocking()
   it blocks the thread on which it runs until its coroutine completes.


Q4:

with suspend as i told you can call other suspend functions in you cuttent function


Q5:

in concurrency , a parrent coroutine waits for children to complete 
before it finishes.If the parent coroutine fails or gets canceled too.
Keeping coroutines connected this way makes cancellation and error handling
predictable and safe 

parrallelism performs several tasks,operations at the same time


   
