Correct matches: 13 out of 26 students
Total marks Assigned / Total marks Expected: 57 / 45

Cohen's kappa:
- Strict (nominal): 0.2620
- Strict (quadratic-weighted): 0.1916
- Relaxed via acceptance sets (nominal): 0.3755
- Relaxed via acceptance sets (quadratic-weighted): 0.2177

Strict accuracy: 0.5000
Relaxed accuracy: 0.5769
Strict accuracy 95% CI: (0.3206, 0.6794)
Relaxed accuracy 95% CI: (0.3895, 0.7446)

temperature: 0.8
top_p: 0.85
seed: 42424242

Bias (model - expected): 0.4615  (95% CI: -0.1154, 1.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.0020, 0.5118)
- Strict (quadratic): (-0.2110, 0.5634)
- Relaxed (nominal): (0.1186, 0.6304)
- Relaxed (quadratic): (-0.1840, 0.5924)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        1        2        4
Teacher=1        0        0        0        0
Teacher=2        0        0        4        2
Teacher=3        1        1        2        7

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        1        2        4
Teacher=1        0        0        0        0
Teacher=2        0        0        5        1
Teacher=3        1        1        1        8

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.