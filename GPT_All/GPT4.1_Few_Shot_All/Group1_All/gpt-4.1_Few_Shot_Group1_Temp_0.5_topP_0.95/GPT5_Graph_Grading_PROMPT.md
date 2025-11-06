Correct matches: 11 out of 26 students
Total marks Assigned / Total marks Expected: 57 / 45

Cohen's kappa:
- Strict (nominal): 0.1236
- Strict (quadratic-weighted): 0.2019
- Relaxed via acceptance sets (nominal): 0.3067
- Relaxed via acceptance sets (quadratic-weighted): 0.2237

Strict accuracy: 0.4231
Relaxed accuracy: 0.5385
Strict accuracy 95% CI: (0.2554, 0.6105)
Relaxed accuracy 95% CI: (0.3546, 0.7124)

temperature: 0.5
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.4615  (95% CI: -0.1538, 1.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.1383, 0.3769)
- Strict (quadratic): (-0.1928, 0.5672)
- Relaxed (nominal): (0.0369, 0.5694)
- Relaxed (quadratic): (-0.1709, 0.6053)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        2        1        4
Teacher=1        0        0        0        0
Teacher=2        0        0        2        4
Teacher=3        2        0        2        7

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        2        1        4
Teacher=1        0        0        0        0
Teacher=2        0        0        4        2
Teacher=3        2        0        1        8

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.