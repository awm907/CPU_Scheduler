# CPU_Scheduler
Process Scheduling Algorithms
This program consists of two process scheduling alogrithms:
* First Come First Served Scheduling
* Round Robin Scheduling

#To Run:
* From command line, provide the text file name containing processes.
* Time Slice for Round Robin

#Example:
java CPUScheduler.java text.txt 2

#Text-File-Format:
It consists of three columns separated by a single space and every single row represents a process:
* The first column contains the process ID 
* The second column is the arrival time
* The third column is the CPU burst time

#Sample Input: 
P0 0 3
P1 1 6
P2 5 4
P3 7 3

Sample Output:
-------------------------------------------------
                CPU Scheduling Simulator
-------------------------------------------------

-------------------------------------------------
        First come first served scheduling
-------------------------------------------------

[0-3]   P0 running
[3-9]   P1 running
[9-13]  P2 running
[13-16] P3 running

Turnaround times:
        P0: 3
        P1: 8
        P2: 8
        P3: 9
Wait times:
        P0: 0
        P1: 2
        P2: 4
        P3: 6
Response times:
        P0: 0
        P1: 2
        P2: 4
        P3: 6

Average Turn around time: 7.0
Average Wait time: 3.0
Average Response time: 3.0

-------------------------------------------------
                Round Robin Scheduling
-------------------------------------------------

[0-2]   P0 running
[2-4]   P1 running
[4-5]   P0 running
[5-7]   P1 running
[7-9]   P2 running
[9-11]  P3 running
[11-13] P1 running
[13-15] P2 running
[15-16] P3 running

Turnaround times:
        P0: 5
        P1: 12
        P2: 10
        P3: 9
Wait times:
        P0: 2
        P1: 6
        P2: 6
        P3: 6
Response times:
        P0: 0
        P1: 1
        P2: 2
        P3: 2

Average Turn around time: 9.0
Average Wait time: 5.0
Average Response time: 1.25

-------------------------------------------------
Project done by [Abdul Wahab Malik]
-------------------------------------------------
