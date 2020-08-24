<h1>Introduction</h1>

<p>
First Come First Serve (FCFS) is an operating system scheduling algorithm that automatically executes queued requests and processes in order of their arrival. It is the easiest and simplest CPU scheduling algorithm. In this type of algorithm, processes which request the CPU first get the CPU allocation. This is managed with a FIFO queue. The full form of FCFS is First Come First Serve. However, Round-robin (RR) is one of the algorithms employed by process and network schedulers in computing. As the term is generally used, time slices (also known as time quanta) are assigned to each process in equal portions and circular order, handling all processes without priority (also known as cyclic executive). Round-robin scheduling is simple, easy to implement, and starvation-free. Round-robin scheduling can be applied to other scheduling problems, such as data packet scheduling in computer networks. It is an operating system concept. Nevertheless, Shortest remaining time, also known as the shortest remaining time first (SRTF), is a scheduling method that is a preemptive version of the shortest job next schedule. In this scheduling algorithm, the process with the smallest amount of time remaining until completion is selected to execute. Since the currently executing process is the one with the shortest amount of time remaining by definition, and since that time should only reduce as execution progresses, processes will always run until they complete or a new process is added that requires a smaller amount of time.</p>
<br>

<h1>Consideration</h1>
<h2><li>FCFS</h2>
<p>
First Come First Served (FCFS) is the simplest and non-preemptive scheduling algorithm. In First Come First Served (FCFS), the process is allocated to the CPU in the order of their arrival. A queue data structure is used to implement the FCFS scheduling algorithm. The process which is at the head of the ready queue is allocated to the CPU, when CPU is free. Then the process which is running is removed from the queue. When a new process enters into the ready queue, it is placed onto the tail of the ready queue. 
</p>

<h2><li>RR</h2>
<p>
Round Robin (RR) Scheduling Algorithm is design for the time sharing system. This algorithm is the preemptive scheduling algorithm. In Round Robin Scheduling Algorithm a small unit of time called as time quantum or time slice for which the CPU is provided to each job. CPU is allocated to the each job for the duration equal to the time quantum in cyclic order. This time quantum, time slice or time interval is generally of the order of 10 to 100 milliseconds. Ready queue in the Round Robin Scheduling Algorithm is treated as the circular queue.
<p>

<h2><li>SRTF</h2>
<p>
In the Shortest Remaining Time First (SRTF) scheduling algorithm, the process with the smallest amount of time remaining until completion is selected to execute. Since the currently executing process is the one with the shortest amount of time remaining by definition, and since that time should only reduce as execution progresses, processes will always run until they complete or a new process is added that requires a smaller amount of time.
<p>
<br>

<h1>Analysis AND Comparison</h1>

<table style="width:100%">
  <tr>
    <th>FCFS</th>
    <th>RR</th>
    <th>SRTF</th>
  </tr>
  <tr>
    <td>FCFS algorithm doesn't include any complex logic, it just puts the process requests in a queue and executes it one by one. Hence, FCFS is pretty simple and easy to implement.</td>
    <td>Each process is served by the CPU for a fixed time quantum, so all processes are given the same priority.</td>
    <td>According to the definition, short processes are executed first and then followed by longer processes.</td>
  </tr>
  <tr>
    <td>Every process will get a chance to run, so starvation doesn't occur.</td>
    <td>Starvation doesn't occur because for each round robin cycle, every process is given a fixed time to execute. No process is left behind.</td>
    <td>The throughput is increased because more processes can be executed in less amount of time.</td>
  </tr>
  <tr>
    <td>There is no option for pre-emption of a process. If a process is started, then CPU executes the process until it ends.</td>
    <td>The throughput in RR largely depends on the choice of the length of the time quantum. If time quantum is longer than needed, it tends to exhibit the same behavior as FCFS.</td>
    <td>The time taken by a process must be known by the CPU beforehand, which is not possible.</td>
  </tr>
  <tr>
    <td>Because there is no pre-emption, if a process executes for a long time, the processes in the back of the queue will have to wait for a long time before they get a chance to be executed.</td>
    <td>If time quantum is shorter than needed, the number of times that CPU switches from one process to another process, increases. This leads to decrease in CPU efficiency.</td>
    <td>Longer processes will have more waiting time, eventually they'll suffer starvation.</td>
  </tr>
</table>



<br>
