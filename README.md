1. What is an operating system? What does it do? Operating system is  the body of the software. Moreover, it makes programs to run easily. 
2. What is virtualization? The primary way the OS does this is through a general technique that we call virtualization. That is, the OS takes a physical resource (such as the processor, or memory, or a disk) and transforms it into a more gen- eral, powerful, and easy-to-use virtual form of itself. 
3. How does an OS provide access to its features? in order to allow users to tell the OS what to do and thus make use of the features of the virtual machine (such as running a pro- gram, or allocating memory, or accessing a file), the OS also provides some interfaces (APIs) that you can call. 
4. What illusion does a virtualized CPU provide?  CPU provides program to deal with each other 
    * How does this affect the user experience? It will not have  a bugs. Operating systems may have limit for something, CPU provides computer not to freeze, It makes illusion  like it is alone.
    * How does this affect the developer experience? It will saves time for developer 
    * What if the CPU were not virtualized?  It can not work normally , you will lose your time. Moreover, It may stop working
5. What is a memory address?  Memory is just an array of bytes; to read memory, one must specify an address to be able to access the data stored there; to write (or update) memory, one must also specify. Each process accesses its own private virtual address space (sometimes just called its address space), which the OS somehow maps onto the physical memory of the machine Why would we want this? 
   6. What is memory virtualization? Each process accesses its own private virtual address space, which the OS somehow maps onto the physical memory of the machine.
    - Why would we want this? It allows us to run programs in memory even if there is insufficient memory to begin with. This is the principle behind virtual memory  
   7. What happens if you write a C/C++ program that writes past the end of an array?  
     It depends if the buffer was allocated on the stack or on the heap. It also depends on the computer architecture and it depends on the values that were written.
      - Can this affect other programs? The standard says that undefined behavior can mean anything, so you can't really have any expectations, not even with the same compiler. 
   8. What is a thread? A thread is a part of the operating system, which is responsible for execution of only one instruction.
  9. Why would we ever write a multi-threaded program? A multi-threaded application takes advantage of running multiple tasks at the same time to speed things up. Multithreading can also take advantage of multiple CPU machines.
   10. What is atomicity? Atomic means that an operation is done without the chance for another thread to interrupt it and do something in the middle of it.
    - Is a C/C++ statement atomic? The C standard does not define whether it is atomic or not. In practice it shows it isn't.
    - Is a Java statement atomic? Most operations are indeed atomic. Operations involving 64 bit structures like double / long are not atomic by themselves. The 64 bit operation can be split into 2 32 bit operations.
    - Is an assembler statement atomic? You cannot assume one machine code will execute atomically. 
  11. What does persistence mean? In system memory, data can be easily lost, as devices such as DRAM store values in a volatile manner; when power goes away or the system crashes, any data in memory is lost. Thus, we need hardware and software to be able to store data persistently.
   12. How does OS hard drive virtualization differ from CPU & memory virtualization? The OS does not create a private, virtualized disk for each application. Rather, it is assumed that often times, users will want to share information that is in files. 
   13. How does running multiple programs at the same time increase CPU efficiency? 
Instead of just running one task at a time, the OS would load a lot of tasks into memory and switch between them, which improves CPU utilization. 
  14. What is multiprogramming? Multiprogramming is a parallel processing in which several programs are run at the same time on a single processor.
