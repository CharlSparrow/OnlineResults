Correct matches: 8 out of 26 students
Total marks Assigned / Total marks Expected: 55 / 48

Cohen's kappa:
- Strict (nominal): -0.0331
- Strict (quadratic-weighted): 0.0375
- Relaxed via acceptance sets (nominal): 0.1100
- Relaxed via acceptance sets (quadratic-weighted): 0.1462

Strict accuracy: 0.3077
Relaxed accuracy: 0.4615
Strict accuracy 95% CI: (0.1650, 0.4999)
Relaxed accuracy 95% CI: (0.2876, 0.6454)

temperature: 1
top_p: 0.85
seed: 42424242

Bias (model - expected): 0.2692  (95% CI: -0.3846, 0.8846)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.2768, 0.2000)
- Strict (quadratic): (-0.3404, 0.3917)
- Relaxed (nominal): (-0.1685, 0.3676)
- Relaxed (quadratic): (-0.2279, 0.4867)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        0        3        4
Teacher=1        0        0        0        0
Teacher=2        0        0        1        2
Teacher=3        2        0        7        5

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        0        3        4
Teacher=1        0        0        0        0
Teacher=2        0        0        1        2
Teacher=3        2        0        3        9

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
    Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
    Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
    Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.