Correct matches: 12 out of 26 students
Total marks Assigned / Total marks Expected: 48 / 48

Cohen's kappa:
- Strict (nominal): 0.1689
- Strict (quadratic-weighted): 0.2565
- Relaxed via acceptance sets (nominal): 0.4150
- Relaxed via acceptance sets (quadratic-weighted): 0.3599

Strict accuracy: 0.4615
Relaxed accuracy: 0.6538
Strict accuracy 95% CI: (0.2876, 0.6454)
Relaxed accuracy 95% CI: (0.4622, 0.8059)

temperature: 1.4
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0000  (95% CI: -0.5769, 0.6154)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.0995, 0.4307)
- Strict (quadratic): (-0.1487, 0.5978)
- Relaxed (nominal): (0.1165, 0.6790)
- Relaxed (quadratic): (-0.0410, 0.6910)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        0        1        4
Teacher=1        0        0        0        0
Teacher=2        2        0        1        0
Teacher=3        1        1        5        7

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        0        1        4
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        1        1        1       11

Tolerated off-diagonal hits (count): 5
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
    Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
    Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
    Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.