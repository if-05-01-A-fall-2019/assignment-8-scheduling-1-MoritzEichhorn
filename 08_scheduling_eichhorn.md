# Basics of Scheduling, Eichhorn Moritz 3AHIF

## 1 Scheduling -- Process Selection
When an important process A blocks, it is waiting for something. So it would be good that the process B, which for example has to finish in order to let A continue, will be done before the other unimportant processes.

For example when one process(A) calculates the average grades from a test. A has high priority. This process needs all the grades from the students which it gets from process B. Process B hasn't finished grading the test results yet. So process A switches into blocked and waits for B to finish. Now it would be good that before A switches to blocked it tells the scheduler that B should be the next process that gets runtime. Because process A can't continue without B finishing.

## 2 Minimizing Turn Around time
| Process |A | B | C | D | E | F | G | H |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
Expected run time (msec) | 8 | 5 | 16 | 12 | 55 | 21 | 2 | 34

To minimize average turn around time the scheduler should order these process by their expected runtime ascending:

| Process |A | B | C | D | E | F | G | H |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
Expected run time (msec) | 2 | 5 | 8 | 12 | 16 | 21 | 34 | 55

Sum: 409 

(minimal) average turn around time: 51.125  


