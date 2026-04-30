# Job-Scheduling-deadlines-
This program uses a greedy strategy to schedule jobs in available time slots before deadlines to achieve maximum profit.
OVERVIEW
This project implements the Job Sequencing with Deadlines problem using a greedy approach. Each job has a deadline and a profit, and the objective is to schedule jobs in a way that maximizes total profit while ensuring that each job is completed before its deadline.
PROBLEM STATEMENT
Given a set of jobs where each job has:
an identifier (Job ID)
a deadline (integer)
a profit (integer)
Schedule the jobs such that:
No two jobs overlap (only one job per time slot)
Each job is completed before or on its deadline
Total profit is maximized
APPROACH
The solution follows a greedy strategy:
Sort all jobs in descending order of profit
Iterate through the sorted jobs
For each job, place it in the latest available time slot before its deadline
If no slot is available, discard the job
ALGORITHM
Input the number of jobs
Store job details (ID, deadline, profit)
Find the maximum deadline
Sort jobs by profit (descending)
Initialize a slot array to track free/occupied slots
Assign jobs to slots greedily
Compute total profit
TIME COMPLEXITY
Sorting: O(n log n)
Scheduling: O(n × d)
Where:
n = number of jobs
d = maximum deadline
KEY IDEA
Always schedule the highest-profit job first and assign it to the latest available slot before its deadline.
APPLICATIONS
CPU scheduling
Task scheduling systems
Resource allocation problems
