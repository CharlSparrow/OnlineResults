Correct matches: 13 out of 26 students
Total marks Assigned / Total marks Expected: 49 / 48

Cohen's kappa:
- Strict (nominal): 0.2636
- Strict (quadratic-weighted): 0.1317
- Relaxed via acceptance sets (nominal): 0.3410
- Relaxed via acceptance sets (quadratic-weighted): 0.2093

Strict accuracy: 0.5000
Relaxed accuracy: 0.5769
Strict accuracy 95% CI: (0.3206, 0.6794)
Relaxed accuracy 95% CI: (0.3895, 0.7446)

temperature: 1.2
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0385  (95% CI: -0.6154, 0.6538)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.0122, 0.5262)
- Strict (quadratic): (-0.2892, 0.5259)
- Relaxed (nominal): (0.0433, 0.6071)
- Relaxed (quadratic): (-0.1934, 0.5823)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        1        1        4
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        2        3        2        7

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        1        1        4
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        2        2        1        9

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
    Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
    Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
    Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.