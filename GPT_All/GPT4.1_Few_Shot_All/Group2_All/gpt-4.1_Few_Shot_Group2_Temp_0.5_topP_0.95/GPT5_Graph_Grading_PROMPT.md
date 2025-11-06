Correct matches: 11 out of 26 students
Total marks Assigned / Total marks Expected: 59 / 45

Cohen's kappa:
- Strict (nominal): 0.0993
- Strict (quadratic-weighted): -0.0028
- Relaxed via acceptance sets (nominal): 0.2710
- Relaxed via acceptance sets (quadratic-weighted): 0.0517

Strict accuracy: 0.4231
Relaxed accuracy: 0.5385
Strict accuracy 95% CI: (0.2554, 0.6105)
Relaxed accuracy 95% CI: (0.3546, 0.7124)

temperature: 0.5
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.5385  (95% CI: -0.1154, 1.1923)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.1932, 0.3714)
- Strict (quadratic): (-0.3716, 0.3835)
- Relaxed (nominal): (-0.0352, 0.5388)
- Relaxed (quadratic): (-0.3165, 0.4363)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        0        1        6
Teacher=1        0        0        0        0
Teacher=2        0        0        3        3
Teacher=3        2        0        3        6

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        0        1        6
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