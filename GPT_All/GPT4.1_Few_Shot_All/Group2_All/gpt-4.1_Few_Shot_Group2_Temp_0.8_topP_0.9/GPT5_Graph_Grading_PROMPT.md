Correct matches: 9 out of 26 students
Total marks Assigned / Total marks Expected: 56 / 45

Cohen's kappa:
- Strict (nominal): -0.0161
- Strict (quadratic-weighted): 0.0259
- Relaxed via acceptance sets (nominal): 0.2744
- Relaxed via acceptance sets (quadratic-weighted): 0.1026

Strict accuracy: 0.3462
Relaxed accuracy: 0.5385
Strict accuracy 95% CI: (0.1941, 0.5378)
Relaxed accuracy 95% CI: (0.3546, 0.7124)

temperature: 0.8
top_p: 0.9
seed: 42424242

Bias (model - expected): 0.4231  (95% CI: -0.2308, 1.0769)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.3120, 0.2669)
- Strict (quadratic): (-0.3935, 0.4192)
- Relaxed (nominal): (-0.0574, 0.5550)
- Relaxed (quadratic): (-0.3074, 0.4909)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        0        0        6
Teacher=1        0        0        0        0
Teacher=2        0        0        2        4
Teacher=3        2        0        5        4

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        0        0        6
Teacher=1        0        0        0        0
Teacher=2        0        0        4        2
Teacher=3        2        0        2        7

Tolerated off-diagonal hits (count): 5
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.