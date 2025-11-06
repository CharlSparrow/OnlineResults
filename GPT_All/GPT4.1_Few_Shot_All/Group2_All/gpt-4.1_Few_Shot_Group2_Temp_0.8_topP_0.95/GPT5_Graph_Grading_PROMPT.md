Correct matches: 18 out of 26 students
Total marks Assigned / Total marks Expected: 53 / 45

Cohen's kappa:
- Strict (nominal): 0.5398
- Strict (quadratic-weighted): 0.7577
- Relaxed via acceptance sets (nominal): 0.7719
- Relaxed via acceptance sets (quadratic-weighted): 0.8354

Strict accuracy: 0.6923
Relaxed accuracy: 0.8462
Strict accuracy 95% CI: (0.5001, 0.8350)
Relaxed accuracy 95% CI: (0.6647, 0.9385)

temperature: 0.8
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.3077  (95% CI: 0.0000, 0.6154)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3004, 0.7668)
- Strict (quadratic): (0.5542, 0.9094)
- Relaxed (nominal): (0.5702, 0.9413)
- Relaxed (quadratic): (0.6445, 0.9843)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        2        3        0
Teacher=1        0        0        0        0
Teacher=2        1        0        3        2
Teacher=3        0        0        0       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        1        3        0
Teacher=1        0        0        0        0
Teacher=2        0        0        6        0
Teacher=3        0        0        0       11

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.