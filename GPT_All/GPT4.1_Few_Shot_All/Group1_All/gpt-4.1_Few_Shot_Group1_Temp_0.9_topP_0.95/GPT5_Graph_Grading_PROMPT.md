Correct matches: 11 out of 26 students
Total marks Assigned / Total marks Expected: 60 / 45

Cohen's kappa:
- Strict (nominal): 0.0888
- Strict (quadratic-weighted): -0.0443
- Relaxed via acceptance sets (nominal): 0.3318
- Relaxed via acceptance sets (quadratic-weighted): 0.0037

Strict accuracy: 0.4231
Relaxed accuracy: 0.5769
Strict accuracy 95% CI: (0.2554, 0.6105)
Relaxed accuracy 95% CI: (0.3895, 0.7446)

temperature: 0.9
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.5769  (95% CI: -0.0779, 1.2308)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.2044, 0.3701)
- Strict (quadratic): (-0.4033, 0.3354)
- Relaxed (nominal): (0.0109, 0.6062)
- Relaxed (quadratic): (-0.3679, 0.3947)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        0        0        7
Teacher=1        0        0        0        0
Teacher=2        0        0        3        3
Teacher=3        2        0        3        6

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        0        0        7
Teacher=1        0        0        0        0
Teacher=2        0        0        5        1
Teacher=3        2        0        1        8

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.