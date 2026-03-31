# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[A process is a complete program in execution, and it has its own memory and system resources. A thread is a smaller unit inside a process, and multiple threads can exist within the same process while sharing the same memory. The main difference is that processes are heavier and take more time and resources to create, while threads are lighter and faster. Threads also communicate more easily because they share memory, unlike processes which need special communication methods. In this assignment, we used threads because they are more efficient for simulating multiple processes running at the same time. Using separate processes would be slower and more complex for this type of simulation.]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

[In Round-Robin scheduling, if a process does not finish within its time quantum, it is removed from the CPU and placed back at the end of the ready queue. This allows other processes to get a chance to run, which ensures fairness. The process will run again when its turn comes in the queue. This cycle continues until the process finishes its execution. This behavior prevents any single process from taking too much CPU time.]

Example from my output:
```
[▶ P11 executing quantum [5000ms] ⚡ Quantum progress: [███████████████] 100% ⏸ P11 completed quantum 5000ms │ Overall progress: [███████████░░░░░░░░░] 57% Remaining time: 3717ms ↻ P11 yields CPU for context switch ➕ P11 (Priority: 1) added to ready queue │ Burst time: 8717ms ┌─ Ready Queue ───────────────────────── │ [P1 → P3 → P5 → P6 → P11]]
```

**Explanation of example:**
[In this example, process P11 did not finish its execution after using its full time quantum (5000ms), and it still had remaining time (3717ms). Because of that, it stopped and yielded the CPU. Then it was added again to the end of the ready queue, which means other processes (P1, P3, P5, P6) will run before it. After its turn comes again, P11 will continue execution until it finishes. This shows how Round-Robin scheduling ensures fairness between all processes.]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: [P1 is in the New state when the thread is created but before calling Thread.start(). At this point, it has not started execution yet.]

2. **Runnable**: [P1 enters the Runnable state after calling Thread.start(), where it is ready to run and waiting for CPU scheduling.]

3. **Running**: [P1 is in the Running state when it is actually executing on the CPU, which is shown in the output like:
"▶ P1 executing quantum [5000ms]"]

4. **Waiting**: [P1 goes into a waiting-like state when it finishes its time quantum but still has remaining time, and it is placed back in the ready queue, for example:
"↻ P1 yields CPU for context switch"]

5. **Terminated**: [P1 reaches the Terminated state when it finishes execution completely, shown in the output as:
"✓ P1 finished execution!"]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Web Browser]

**Description**: 
[A web browser loads different parts of a webpage like images, text, and videos at the same time using multiple threads.]

**Why Round-Robin works well here**: 
[Round-Robin scheduling ensures that each task gets a fair share of CPU time, so no part of the webpage blocks others. This improves responsiveness and makes the page load smoot]

### Example 2: [Operating System Task Scheduling]

**Description**: 
[Operating systems run multiple applications at the same time, such as browsers, music players, and background processes.]

**Why Round-Robin works well here**: 
[Round-Robin scheduling ensures that each application gets a fair turn to use the CPU. This prevents one program from taking all the resources and keeps the system responsive.]

---

## Summary

**Key concepts I understood through these questions:**
1. The difference between threads and processes
2. How Round-Robin scheduling works and manages the ready queue
3. The lifecycle of a thread and its different states
 
**Concepts I need to study more:**
1. Thread synchronization
2. Problems like deadlock and race conditions
