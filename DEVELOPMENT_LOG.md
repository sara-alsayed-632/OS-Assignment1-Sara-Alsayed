# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry 1 - [March 27, 2026, 3:00 PM]
**What I did**: Forked the repository ,set up my student ID and Installed Visual Studio Code

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (444052896)
- Installed Visual Studio Code and required extensions

**Challenges**: 
Had to install visual studio and GitHub integration in VS Code
I needed to install Git to be able to clone the repository and work on it locally
**Solution**: 
watched video to know how to sign in and integrate VS with github and install Git
**Time spent**: 50 min

---

### Entry 2 - [March 28, 2026, 8:50 PM]
**What I did**: Understood the starter code and program flow

**Details**: 
- Read through Process class and SchedulerSimulation class
- Analyzed how Round-Robin scheduling works in the code
- Traced execution of threads and queue behavior

**Challenges**: Understanding how threads interact with the queue and when processes re-enter the queue

**Solution**: Carefully followed the run() method and reread the code many times

**Time spent**: 1 hour

---

### Entry 3 - [March 29, 2026, 6:30 PM]
**What I did**: Implemented Feature 1 (Process Priority) and Implemented Feature 2 (Context Switch Counter) 

**Details**: 
- Installed Java Coding Pack to ensure full Java support
- Verified that the program can compile and run
- Added priority field to Process class (1–5)
- Generated random priority for each process
- Modified output to display priority when process enters queue
- Added static counter variable
- Incremented counter whenever a new process starts execution
- Displayed total context switches at the end
- commit the changes

**Challenges**: 
Java was not fully configured initially, which affected running the code
Making sure the new feature does not affect the existing scheduling logic
Determining the correct place to increment the counter

**Solution**: 
Installed Java Coding Pack and ensured JDK is properly configured
Carefully updated constructor and print statements and tested multiple runs
Added the increment inside the scheduler loop before starting each thread

**Time spent**:  1h and 30 min  

---

### Entry 4 - [March 29, 2026, 10:00 PM]
**What I did**: Implemented Feature 3 (Waiting Time Tracking) , Testing and final adjustments

**Details**: 
- Added fields for creation time and waiting time
- Used System.currentTimeMillis() to track timing
- Calculated waiting time for each process
- Displayed results in a summary table
- commit the changes
- Ran the program 
- Verified all features are working correctly
- Checked formatting and output clarity
- Reviewed commits 
**Challenges**: ensure the final output is correct
**Solution**: - Ran the program multiple times

**Time spent**: 30 min

---

### Entry 5 - [March 30, 2026, 8:43 PM]
**What I did**: Documentation and Reflect what I learned

**Details**: 
- Completed DEVELOPMENT_LOG.md with all development steps
- Answered reflection questions in REFLECTION.md
- Wrote answers to technical questions in ANSWERS.md
- Reviewed my code and connected concepts (threads, scheduling, queue behavior) to what I implemented
- Reflected on how multithreading works in real-world applications

**Challenges**: Writing clear explanations and answers

**Solution**: wrote in simple words and arranged my words

**Time spent**: 2 hours

---

## Summary

**Total time spent on assignment**: [12 hours]

**Most challenging part**: understanding the code and Setting up the environment (Github, Java, and VS Code)

**Most interesting learning**: Understanding how Round-Robin scheduling works with threads and how context switching happens

**What I would do differently next time**: Prepare the development environment earlier and test each feature step by step
