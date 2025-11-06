Correct matches: 8 out of 26 students
Total marks Assigned / Total marks Expected: 57 / 45

Cohen's kappa:
- Strict (nominal): -0.0541
- Strict (quadratic-weighted): -0.0162
- Relaxed via acceptance sets (nominal): 0.2301
- Relaxed via acceptance sets (quadratic-weighted): 0.0636

Strict accuracy: 0.3077
Relaxed accuracy: 0.5000
Strict accuracy 95% CI: (0.1650, 0.4999)
Relaxed accuracy 95% CI: (0.3206, 0.6794)

temperature: 0.6
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.4615  (95% CI: -0.1923, 1.1154)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.3302, 0.2140)
- Strict (quadratic): (-0.4140, 0.3708)
- Relaxed (nominal): (-0.0773, 0.5074)
- Relaxed (quadratic): (-0.3330, 0.4466)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        1        0        6
Teacher=1        0        0        0        0
Teacher=2        0        0        2        4
Teacher=3        2        0        5        4

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        1        0        6
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