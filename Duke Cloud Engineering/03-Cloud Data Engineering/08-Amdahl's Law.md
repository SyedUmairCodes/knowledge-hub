# Amdahl's Law
Amdahl's Law addresses the limitations of parallelization, highlighting that there are diminishing returns as you increase the number of processors or cores working on a task. This law emphasizes that the speedup achievable through parallelization is constrained by the portion of the task that must be executed sequentially.

Even with code that is highly parallelizable, like deep learning operations, there is a limit to the speed improvement you can achieve. This is because some parts of the code will always need to be executed sequentially.

As you increase the number of cores used for parallel processing, the impact of the sequential portion becomes more pronounced. This results in a gradual decrease in the rate of speedup. Eventually, adding more cores yields negligible performance improvements.

> Real-world code often includes elements that are not purely parallel, such as sleep functions, timeouts, network waiting, or disk I/O operations.These sequential elements further limit the effectiveness of parallelization, making it less useful for everyday tasks.

Amdahl's Law arises from the overheads associated with parallelization. These overheads include:

- The need to coordinate and synchronize tasks across multiple cores.
- The communication overhead required to share data between cores.
- The time spent distributing the workload across the cores.

These overheads consume processing time and resources, offsetting some of the gains achieved through parallel execution. Therefore, while parallelization can significantly improve performance for specific tasks, it's essential to be aware of its limitations and the diminishing returns associated with increasing the number of cores.

## Mathematical Equation

$$
S = 1 / ( (1 - P) + (P / N) )
$$
Where:
- S is the maximum speedup achievable.
- P is the proportion of the task that can be parallelized.
- N is the number of processors or cores.

This formula demonstrates that as N (the number of cores) increases, the overall impact on speedup (S) decreases, particularly if P (the parallelizable portion) is significantly less than.