# CECS 326 Reading Assignment: Introduction to Operating Systems

### Assignment Description
Answer the following questions from the Chapter 1 reading from your textbook. Be thorough and complete with your answers. You may work on these questions with one or two other partners, but *all* students must submit the document individually in their own repositories along with each student's name documented with the submission.

1. What are the two main functions of an operating system?

- Two main functions of an operating system is manage computer's hardware and software resources; provides a convenient user interface for users and applications to interact with hardware.

2. What is the difference between timesharing and multiprogramming systems?

- Timesharing allow many users to interact cuncurrently with a single computer since multiprogramming allow multi-tasks are performed during the same period of time.

3. The family-of-computers idea was introduced in the 1960s with the IBM System/360 mainframes. Is this idea now dead as a doornail or does it live on?

- The family-of-computers concept, where different models share an architecture and run the same software, is very much alive and fundamental to modern computing.

4. What is the difference between kernel and user mode? Explain how having two distinct modes aids in designing an operating system.

- Kenrel mode offers full hardware access for OS function, while user mode restricts applications to liminted, forcing them to use system calls for resources.

5. On early computers, every byte of data read or written was handled by the CPU (i.e., there was no DMA). What implications does this have for multiprogramming?

- It makes multiprogramming less favorable since it is no longer the case that when one process does I/O the CPU is completele free to work on other processes.

6. There are several design goals in building an operating system, for example, resource utilization, timeliness, robustness, and so on. Give an example of two design goals that may contradict one another.

- That is timeliness and fairness. To ensure a critical task meets its deadline (timeliness), the operating system may need to preept to lower-priority process, thus violating fairness.

7. Which of the following instructions should be allowed only in kernel mode?
    (a) Disable all interrupts.
    (b) Read the time-of-day clock.
    (c) Set the time-of-day clock. (d) Change the memory map.

- Those are (a) Disable all interrupts, (c) Set the time-of-day clock, (d) Change the memory map.

8. Consider a system that has two CPUs, each CPU having two threads (hyperthreading). Suppose three programs, P0, P1, and P2, are started with run times of 5, 10 and 20 msec, respectively. How long will it take to complete the execution of these programs? Assume that all three programs are 100% CPU bound, do not block during execution, and do not change CPUs once assigned.

- Either 20, 25 or 30 msec depending on how they scheduled. The total time to finishh it all is the time it takes for the core with the longest time to finish. Worst case is one core get 5 msec, the other gets the 20ms and the 10 (30 msec)

9. What is a trap instruction? Explain its use in operating systems.

- It is a synchronous software-generated interrupt or exception, that causes the CPU to pause current execution, switch from user mode to kernel mode, and transfer control to the operating system's kernel handler.

10. Modern operating systems decouple a process address space from the machine’s physical memory. List two advantages of this design.

- Allows for efficient memory management and increased system security.
