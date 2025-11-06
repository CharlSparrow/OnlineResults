Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 48 / 48

Cohen's kappa:
- Strict (nominal): 0.6268
- Strict (quadratic-weighted): 0.7197
- Relaxed via acceptance sets (nominal): 0.7482
- Relaxed via acceptance sets (quadratic-weighted): 0.7684

Strict accuracy: 0.7692
Relaxed accuracy: 0.8462
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.6647, 0.9385)

temperature: 1
top_p: 0.9
seed: 42424242

Bias (model - expected): 0.0000  (95% CI: -0.3846, 0.3846)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3764, 0.8579)
- Strict (quadratic): (0.4285, 0.9148)
- Relaxed (nominal): (0.5155, 0.9356)
- Relaxed (quadratic): (0.4800, 0.9556)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        0        3        0
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        1        0        1       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        0        3        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        1        0        0       13

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
    Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
    Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
    Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.