# Problem-Solving---Python-Projects
[Algorithm of Longest Proceeessing Time First - Scheduling to Minimize Makespan.txt](https://github.com/jasonchenuk/Problem-Solving---Python-Projects/files/8229063/Algorithm.of.Longest.Proceeessing.Time.First.-.Scheduling.to.Minimize.Makespan.txt)

This project is to solving a scheduling problem to minimize makespan
* There are m machines in a factory.
* There are n jobs to be processed.
* Job j has a given processing time Pj.
   - For a machine to complete job j, it needs to spend Pj amount of time.
   - We say job j is completed at its completion time Cj if Cj = Sj + Pj, where Sj is its starting time (the time that it starts to be processed).
* I want to schedule these jobs to machines to minimize the makespan, i.e., the lastest completion time among all jobs.

* There are 10 jobs with processing times: 3 3 3 4 4 5 5 6 7 8
* There are 3 machines.

* Makespan minimization is also load balancing
   - to fairly allocate jobs.
   - to save utility fees.
   - to go home as early as possible

* I developed a heuristic algorithm.
   - easy to implement, and time efficient.
   - close to the optimal

* This algorithm is call Longest Processing Time First (LPT).
   - first, sort jobs in a descending order of their processing times.
   - then, in each iteration schedule a job to the machine that is currently the least loaded machine (having the earliest completion time).
