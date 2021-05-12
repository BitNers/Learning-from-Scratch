# Operating Systems

## Prologue

    This section will talk about Operating System. You will learn about what are Processes, Memory Management, Bus, Hardware, Linux Shell, and et cetera.

-----


## 1. Intro

**What is Operating Systems?**

    A computer system has many resources (hardware and software), which may be require to complete a task. 
    The commonly required resources are input/output devices, memory, file storage space, CPU etc. 
    The operating system acts as a manager of the above resources and allocates them to specific programs and users, whenever necessary to perform a particular task. 
    Therefore operating system is the resource manager i.e. it can manage the resource of a computer system internally. 
    The resources are processor, memory, files, and I/O devices. In simple terms, an operating system is the interface between the user and the machine.

There's two views of Operating System:
 - User's View

        The user view of the computer refers to the interface being used. Such systems are designed for one user to monopolize its resources, to maximize the work that the user is performing. In these cases, the operating system is designed mostly for ease of use, with some attention paid to performance, and none paid to resource utilization.

 - System View

        Operating system can be viewed as a resource allocator also. A computer system consists of many resources like - hardware and software - that must be managed efficiently. The operating system acts as the manager of the resources, decides between conflicting requests, controls execution of programs etc.
 

The Tasks of an Operating System are:

    -> Processor management which involves putting the tasks into order and pairing them into manageable size before they go to the CPU.
    -> Memory management which coordinates data to and from RAM (random-access memory) and determines the necessity for virtual memory.
    -> Device management which provides interface between connected devices.
    -> Storage management which directs permanent data storage.
    -> Application which allows standard communication between software and your computer.
    -> User interface which allows you to communicate with your computer.


Functions of Operating System:

    1. It boots the computer
    2. It performs basic computer tasks e.g. managing the various peripheral devices e.g. mouse, keyboard
    3. It provides a user interface, e.g. command line, graphical user interface (GUI)
    4. It handles system resources such as computer's memory and sharing of the central processing unit(CPU) time by various applications or peripheral devices.
    5. It provides file management which refers to the way that the operating system manipulates, stores, retrieves and saves data.
    6. Error Handling is done by the operating system. It takes preventive measures whenever required to avoid errors.

-----

## 2. Evolution of Operating Systems

Evolution of Operating Systems.

The evolution of OS is directyl dependent on the development of computer systems and how users use them.
Here is a quick tour of computing systems through the past fifty years in the timeline.


**Early Evolution:**
    
    1945: ENIAC
    1949: EDVAC
    1952: IBM 701
    1956: The interrupt
    1957: FORTRAN was developed


**1950s:** By the late 1950s Operating systems were well improved and started supporting following usages:

        - It was able to perform Single stream batch processing.
        - It could use Common, standardized, input/output routines for device access.
        - Program transition capabilities to reduce the overhead of starting a new job was added.
        - Error recovery to clean up after a job terminated abnormally was added.
        - Job control languages that allowed users to specify the job definition and resource requirements were made possible.

**1960s:**

    1961: The dawn of minicomputers
    1962: Compatible Time-Sharing System (CTSS) from MIT
    1964: IBM System/360
    1960s: Disks became mainstream
    1966: Minicomputers got cheaper, more powerful, and really useful.
    1967-1968: Mouse was invented.
    1964 and onward: Multics
    1969: The UNIX Time-Sharing System from Bell Telephone Laboratories.

**1970s**

    Multi User and Multi tasking was introduced;
    Dynamic address translation hardware and Virtual machines came into picture;
    Modular architectures came into existence;
    Personal, interactive systems came into existence.

**After 1970s**

    1971: Intel announces the microprocessor
    1972: IBM comes out with VM: the Virtual Machine Operating System
    1973: Ethernet
    1976: Apple II
    1983 Microsoft begins work on MS-Windows
    1984 Apple Macintosh comes out
    1990 Microsoft Windows 3.0 comes out
    1991 GNU/Linux
    1992 The first Windows virus comes out
    1993 Windows NT
    2007: iOS
    2008: Android OS


And as the research and development work continues, we are seeing new 
operating systems being developed and existing ones getting improved and 
modified to enhance the overall user experience, making operating systems 
fast and efficient like never before.

-----

## 3. Types of Operating Systems


Following are some of the most widely used types of Operating system:

    1. Simple Batch System
    2. Multiprogramming Batch System
    3. Multiprocessor System
    4. Desktop System
    5. Distributed Operating System
    6. Clustered System


**Simple Batch Systems**

    In this type of system, there is no direct interaction between user and the computer.
    The user has to submit a job (written on cards or tape) to a computer operator.
    Then computer operator places a batch of several jobs on an input device.
    Jobs are batched together by type of languages and requirement.
    Then a special program, the monitor, manages the execution of each program in the batch.
    The monitor is always in the main memory and available for execution.

    Advantages of Simple Batch Systems
        - No interaction between user and computer.
        - No mechanism to prioritise the processes.



**Multiprogramming Batch Systems**

    In this the operating system picks up and begins to execute one of the jobs from memory.
    Once this job needs an I/O operation operating system switches to another job (CPU and OS always busy).
    Jobs in the memory are always less than the number of jobs on disk(Job Pool).
    If several jobs are ready to run at the same time, then the system chooses which one to run through the process of CPU Scheduling.
    In Non-multiprogrammed system, there are moments when CPU sits idle and does not do any work.
    In Multiprogramming system, CPU will never be idle and keeps on processing.
    Time Sharing Systems are very similar to Multiprogramming batch systems. In fact time sharing systems are an extension of multiprogramming systems.

    In Time sharing systems the prime focus is on minimizing the response time, while in multiprogramming the prime focus is to maximize the CPU usage.


**Multiprocessor Systems**
    
    A Multiprocessor system consists of several processors that share a common physical memory. 
    Multiprocessor system provides higher computing power and speed. 
    In multiprocessor system all processors operate under single operating system. 
    Multiplicity of the processors and how they do act together are transparent to the others.

    Advantages of Multiprocessor Systems
        - Enhanced performance
        - Execution of several tasks by different processors concurrently, increases the system's throughput without speeding up the execution of a single task.
        - If possible, system divides task into many subtasks and then these subtasks can be executed in parallel in different processors. 
            Thereby speeding up the execution of single tasks.


**Desktop Systems**

    Earlier, CPUs and PCs lacked the features needed to protect an operating system from user programs. 
    PC operating systems therefore were neither multiuser nor multitasking. 
    However, the goals of these operating systems have changed with time; instead of maximizing CPU and peripheral utilization, the systems opt for maximizing user convenience and responsiveness.
    These systems are called Desktop Systems and include PCs running Microsoft Windows and the Apple Macintosh.
    Operating systems for these computers have benefited in several ways from the development of operating systems for mainframes.

    Microcomputers were immediately able to adopt some of the technology developed for larger operating systems. 
    On the other hand, the hardware costs for microcomputers are sufficiently low that individuals have sole use of the computer, and CPU utilization is no longer a prime concern. 
    Thus, some of the design decisions made in operating systems for mainframes may not be appropriate for smaller systems.


**Distributed Operating System**

    The motivation behind developing distributed operating systems is the availability of powerful and inexpensive microprocessors and advances in communication technology.
    These advancements in technology have made it possible to design and develop distributed systems comprising of many computers that are inter connected by communication networks.
    The main benefit of distributed systems is its low price/performance ratio.


    Advantages Distributed Operating System
        - As there are multiple systems involved, user at one site can utilize the resources of systems at other sites for resource-intensive tasks.
        - Fast processing.
        - Less load on the Host Machine.Types of Distributed Operating Systems

    Following are the two types of distributed operating systems used:

        - Client-Server Systems 
        - Peer-to-Peer Systems (P2P)

        Client-Server Systems
            Centralized systems today act as server systems to satisfy requests generated by client systems. 
            Server Systems can be broadly categorized as: Compute Servers and File Servers.

                - Compute Server systems, provide an interface to which clients can send requests to perform an action, in response to which they execute the action and send back results to the client.
                - File Server systems, provide a file-system interface where clients can create, update, read, and delete files.

        Peer-to-Peer Systems
            The growth of computer networks - especially the Internet and World Wide Web (WWW) – has had a profound influence on the recent development of operating systems. 
            When PCs were introduced in the 1970s, they were designed for personal use and were generally considered standalone computers.
            With the beginning of widespread public use of the Internet in the 1990s for electronic mail and FTP, many PCs became connected to computer networks.

            In contrast to the Tightly Coupled systems, the computer networks used in these applications consist of a collection of processors that do not share memory or a clock. 
            Instead, each processor has its own local memory. The processors communicate with one another through various communication lines, such as high-speed buses or telephone lines. 
            These systems are usually referred to as loosely coupled systems ( or distributed systems).


**Clustered Systems**

    Like parallel systems, clustered systems gather together multiple CPUs to accomplish computational work.

    Clustered systems differ from parallel systems, however, in that they are composed of two or more individual systems coupled together.

    The definition of the term clustered is not concrete; the general accepted definition is that clustered computers share storage and are closely linked via LAN networking.

    Clustering is usually performed to provide high availability.

    A layer of cluster software runs on the cluster nodes. Each node can monitor one or more of the others. 
        If the monitored machine fails, the monitoring machine can take ownership of its storage, and restart the application(s) that were running on the failed machine. The failed machine can remain down, but the users and clients of the application would only see a brief interruption of service.

    Clustered technology is rapidly changing. Clustered system's usage and it's features should expand greatly as Storage Area Networks(SANs). 
    SANs allow easy attachment of multiple hosts to multiple storage units. 
    Current clusters are usually limited to two or four hosts due to the complexity of connecting the hosts to shared storage.         

-----

## 4. Processes and Threads

The Operating System is responsible to schedule the processes in the computer, but... what is a process?

To understand processes, we need to understand the program.
What exactly is a **program**?

    """
        #include <stdio.h>

        int main(void){
            printf("Hello World");
        }

    """

This an example in C how we print 'Hello World'.
Look how we have commons words that made us able to understand this code.

This is what we call the High Level Language, which we can write a set of instructions readable for humans.

There is another HLL such as Python or Javascript, to print with Python we use ONLY one line.

        print("Hello World")


Amazing don't ya? 
Therefore, you have talked about that computers only read/write binaries numbers (0-1). How the computer understand what I wrote? There is something between the User Interface and the Hardware?
There is, and his name is the Compiler and Interpreter.
We won't get deep into these guys for now, let's get back to understand what is a process.


Well, knowing what is a program, the process is just a program in execution.
The program is a **PASSIVE ENTITY**, that means, the program is stored in Disk, instead in RAM. The program doesn't have the a process stack, or program counter or registers to execute.


The Process is not as same as program, because it is an active entity that actions the purpose of the application.
    
The computer loads the program from Disk and store at RAM, making an active entity, including the program counter, process stack and registers in CPU. The Process Stack is the Cached RAM to provide an additional space if required. This memory is divided into four sections for efficient working:

    - Text sections -> Is made for compiled program code, where is Read-Only code stays when the program is launched.
    - Data sections -> Is made for global and static variables, allocated and initialized prior to executing the program.
    - Heap -> Is made for Dynamic Memory Allocation. 
    - Stack -> Is made for Local Variables. The space on the stack is reserved for local variables whey they are declared.

* In Programming Languages, Local Variables is the variable declared inside a function. 

* Variables declared outside the function, we can call Global Variables. 

* Static variables has your values preserved even after they are out of their scope.





Now that we know what is a process, we need to understand their differente states. Remember the processes are active entities, that means they can be in any of the following states:

        - NEW -> The process is being created. The OS is allocating resources. 
        - READY -> The process is ready to run, waiting to be assigned by the processor.
        - RUNNING -> The Program's Instructions are being executed.
        - WAITING -> The process is waiting for some event to occur (I/O completion or reception of a signal)
        - TERMINATED -> The process has finished execution.

But wait, we have rules to these states. The first obvious is that we can't have processes in READY RUNNING WAITING or TERMINATED states, if it the NEW state was never executed.

This graph will help to understand this. The states are linked, and we must respect these rules.


                 ____________                  
               /              \            
    NEW -> READY             WAITING
                \  RUNNING  /
                            \
                             TERMINATED

 
The process always going to start with NEW state, then the must next step is READY.

After that, they gonna be in RUNNING STATE, which can be TERMINATED or WAITING.
    The WAITING will wait for some event, and then, will return to the READY STATE.


As we talked before, the process is an active entity, which means they have a block control for attributes such as memory, and registers. Each process is a Data Structure which contains the following.

        - Process ID -> A.K.A PID, is the identification for Process in a System.
        - Process State -> It can be Running, or Ready, etc.
        - CPU Registers and Program Counter -> Holds the address of the next instruction to be executed for that process.
        - CPU Scheduling -> Priority information and pointers for scheduling queues (We gonna see this later)
        - Memory Management -> Pages/Segment Tables, Heap and Stack, etc.
        - Accounting Information -> User and Kernel CPU usage, limits, etc.
        - I/O Status information -> Devices allocated, open file tables, etc.

-----

## 5. Process Scheduling

As we seen before, the process is an active entity having attributes to manage it. Processes has states, that changes if needed. The act to change the process that is in the READY state to RUNNING state is known as Process Scheduling.

The prime idea of Process Scheduling is to keep the CPU busy all the time, to deliver the minimum response time for all programs. For achieving this, the schedular must apply appropriate rules for swapping processes IN and OUT of CPU.

**Scheduling will fell into two general categories:**
        
    - Pre-emptive -> When the currently executing process gives up the CPU voluntarily.
    - Non Pre-empetive -> When the OS decides to favour another process, pre-empting the currently executing process.



**What are Scheduling Queues?**

All processes, upon entering into the system, are stored in the Job Queue. Processes in the READY state are placed in the READY Queue. Processes waiting for a device to become available are placed in Device Queues. There are unique device queues available for each I/O device.

A new process is initially put in the READY queue. It waits in the READY queue until it is selected for execution(or dispatched). Once the process is assigned to the CPU and is executing, one of the following several events can occur:

    - The process could issue an I/O request, and then be placed in the I/O queue.
    - The process could create a new subprocess and wait for its termination.
    - The process could be removed forcibly from the CPU, as a result of an interrupt, and be put back in the READY queue.

In the first two cases, the process eventually switches from the waiting state to the READY state, and is then put back in the READY queue. A process continues this cycle until it terminates, at which time it is removed from all queues and has its PCB and resources deallocated.

**Types of Schedulers**
    

        - Long Term Scheduler
        - Short Term Scheduler
        - Medium Term Scheduler
    

**Long Term Scheduler**

        Long term scheduler runs less frequently. 
        Long Term Schedulers decide which program must get into the job queue.
        From the job queue, the Job Processor, selects processes and loads them into the memory for execution. 
        Primary aim of the Job Scheduler is to maintain a good degree of Multiprogramming. 
        An optimal degree of Multiprogramming means the average rate of process creation is equal to the average departure rate of processes from the execution memory.


**Short Term Scheduler**

        This is also known as CPU Scheduler and runs very frequently. 
        The primary aim of this scheduler is to enhance CPU performance and increase process execution rate.


**Medium Term Scheduler**

        This scheduler removes the processes from memory (and from active contention for the CPU), and thus reduces the degree of multiprogramming. 
        At some later time, the process can be reintroduced into memory and its execution van be continued where it left off. This scheme is called swapping. 
        The process is swapped out, and is later swapped in, by the medium term scheduler.

    
Swapping may be necessary to improve the process mix, or because a change in memory requirements has asovercommitted available memory, requiring memory to be freed up.

-----

## 6. Context Switch

**What is Context Switch?**

Switching the CPU to another process requires saving the state of the old process and loading the saved state for the new process. This task is known as a Context Switch.
        

    The context of a process is represented in the Process Control Block(PCB) of a process; it includes the value of the CPU registers, the process state and memory-management information. When a context switch occurs, the Kernel saves the context of the old process in its PCB and loads the saved context of the new process scheduled to run.Context switch time is pure overhead, because the system does no useful work while switching.

    Its speed varies from machine to machine, depending on the memory speed, the number of registers that must be copied, and the existence of special instructions(such as a single instruction to load or store all registers). Typical speeds range from 1 to 1000 microseconds.
    
Context Switching has become such a performance bottleneck that programmers are using new structures(threads) to avoid it whenever and wherever possible.