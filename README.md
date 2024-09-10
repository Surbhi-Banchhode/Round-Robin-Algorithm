# Round-Robin Algorithm

The Round Robin (RR) algorithm is a widely used process scheduling method in operating systems, particularly in time-sharing systems. It ensures that every process gets an equal share of the CPU's time, preventing any single process from monopolizing resources.

## How it Works

1. **Fair Time Sharing**: Each process is assigned a fixed time slice, or "quantum," to execute. If a process doesn't finish within this quantum, it's moved to the back of the queue, and the next process gets its turn.
  
2. **Process Queue**: Processes are organized in a queue, with the first process in line getting to run for the designated time slice.

3. **Cyclic Execution**: This scheduling continues in a circular manner, ensuring that every process gets its fair share of CPU time.

4. **Efficiency**: The Round Robin algorithm is simple to implement and ensures fairness by treating all processes equally. This makes it ideal for time-sharing systems where multiple users or tasks need to be managed simultaneously.
![image](https://github.com/user-attachments/assets/67581a8c-91a8-4d33-aa4c-57ef4ca30cdb)
## Time Complexity
- `O(n log n + n * m)`  
  - where **n** = number of processes, and  
  - **m** = number of rounds

## Space Complexity
- `O(n)`  
  - This accounts for storing the remaining burst time of each process.
