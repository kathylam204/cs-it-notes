# Operating Systems

## Operating System (OS) Defined:
- Abstracts hardware details
- Provides API to users
- Manages resources efficiently
- Facilitates user-hardware interaction

## Key Concepts:
- Program Counter (PC): Holds the address of the next instruction.
- Stack Pointer (SP): Points to the top of the current stack.

## Modes:
### Kernel Mode: CPU can execute any instruction; OS resides here.
- Example: Kernel mode is executed by device drivers so a hardware device (e.g a graphics card or printer) can access the OS.
### User Mode: CPU can execute limited instructions; user applications run here.
- Example: Web browsers are an example of user mode because it has a limited amount of access to the OS.

### System Call: A request from a user application for the OS to perform operations on its behalf.

## Interrupt Processing:
- Save the state of the current process.
- Switch to kernel mode.
- Execute the Interrupt Service Routine (ISR).
- Return to user mode.

## Memory Allocation:
- Base Register: Start location in memory.
- Limit Register: Range of accessible memory.

## I/O Devices:
- Controller: Manages device operations.
- Device Driver: Software that communicates with the controller.

## Device Actions:
- Busy Wait: Ties up the processor.
- Hardware Interrupt: Signals completion or failure.
- DMA (Direct Memory Access): Allows devices to write to memory directly.

## Processes:
- Definition: An executing program.
- Multiprogramming: Involves program, input, output, and state.

## Process Creation:
- System initialization.
- System call by a running process.
- User request.
- Batch job initiation.

## Process Termination:
- Normal exit
- Error exit
- Fatal error
- Killed by another process

## Process States:
- Running: Using CPU.
- Ready: Runnable but no CPU available.
- Blocked: Waiting for an external event.

### Process Control Block (PCB): Contains process state, registers, memory, etc.

## Scheduling:
- Preemptive: Requires clock interrupt, ensures fairness.
- Non-preemptive: Process runs to completion or yields.

## Scheduler Goals:
- Fairness
- Policy enforcement
- Utilization balance
- Maximize job throughput
- Minimize turnaround

## Metrics:
- Throughput: Jobs completed per unit time.
- Utilization: Fraction of time devices are busy.
- Turnaround Time: Time from job arrival to completion.
- Wait Time: Time job is ready but not running.
- Response Time: Time from job arrival to start of output.

## Scheduling Algorithms:
- FIFO (First In, First Out): Non-preemptive, fair, low throughput, high turnaround.
- Shortest Job First: Non-preemptive, high throughput, low turnaround, possible starvation.
- Shortest Remaining Time Next (SRTN): Preemptive, high turnaround, unfair for large jobs.

### Round Robin: Preemptive, uses a time quantum, fair, controls process execution order.

## Priority Scheduling:
- Non-preemptive: Highest priority process runs first.
- Preemptive: Highest priority process can interrupt lower priority processes.

## Example Calculations:
- Turnaround Time: Exit time - Arrival time
- Wait Time: Turnaround time - Execution time
- Response Time: First execution time - Arrival time

## Round Robin (RR)
- Time quantum: Each process gets executed for a fixed time slice.
- Context switches occur frequently.

## Preemptive Priority Scheduling
- Processes are assigned priorities.
- Higher priority processes preempt lower priority ones.

## User-Level Threads
### Managed by runtime libraries, not the kernel.
### Advantages:
- Cheap to create and manage.
- Flexible for the application’s needs.
### Disadvantages:
- Kernel is unaware of user-level threads.
- Blocking system calls can block the entire process.

## Kernel-Level Threads
### Managed by the kernel.
### Advantages:
- Can take advantage of multiple CPUs.
- Correct scheduling by the kernel.
### Disadvantages:
- Expensive to create and manage.
- Performance is generally worse than user-level threads.

## Scheduler Activations
### Bridges the gap between user-level and kernel-level threads.
### Kernel notifies user-level schedulers of scheduling events via upcalls.
### Example:
- A new scheduler activation (SA) is created when a thread blocks.

## Mutual Exclusion
- Ensures only one process can enter its critical section at a time.
- Solutions include disabling interrupts, lock variables, and more complex algorithms like Peterson’s algorithm and Test-and-Set locks.

## Semaphores
- Used for signaling between processes.
- down() decreases the semaphore value or blocks if it's zero.
- up() increases the semaphore value and wakes up a waiting process.

## Deadlock
### A situation where processes wait indefinitely for resources held by each other.
### Four necessary conditions:
- Mutual exclusion
- Hold and wait
- No preemption
- Circular wait

## Paging
- Divides memory into fixed-size pages.
- Virtual memory is mapped to physical memory via page tables.
- Page faults occur when a page is not in physical memory.

## Page Table Calculations
- Virtual Address: Divided into page number and offset.
- Page Table Size: Determined by the number of pages and the frame size.

## Example Calculation:
- Virtual Memory: 4GB (32 bits)
- Page Size: 4KB (12 bits)
- Physical Memory: 2MB (21 bits)

## Protection and Relocation
- Ensures that processes do not interfere with each other.
- Address translation allows relocation.

## Fragmentation
- External: Free memory is non-contiguous.
- Internal: Allocated memory may be larger than requested.

### Two-Phase Locking: A technique to ensure that all locks are acquired before any work is done.

## Summary of Key Terms
- Semaphore: Synchronization tool for managing access to a shared resource.
- Mutex: Mutual exclusion lock.
- Deadlock: A state where processes are unable to proceed due to resource contention.
- Paging: Memory management scheme that eliminates the need for contiguous allocation of physical memory.
- Page Fault: An event that occurs when a requested page is not in memory.

