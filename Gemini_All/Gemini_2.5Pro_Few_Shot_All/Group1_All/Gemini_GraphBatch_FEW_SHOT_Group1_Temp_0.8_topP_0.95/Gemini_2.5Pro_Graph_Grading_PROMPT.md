Correct matches: 18 out of 26 students
Total marks Assigned / Total marks Expected: 47 / 48

Cohen's kappa:
- Strict (nominal): 0.5408
- Strict (quadratic-weighted): 0.8056
- Relaxed via acceptance sets (nominal): 0.6355
- Relaxed via acceptance sets (quadratic-weighted): 0.8657

Strict accuracy: 0.6923
Relaxed accuracy: 0.7692
Strict accuracy 95% CI: (0.5001, 0.8350)
Relaxed accuracy 95% CI: (0.5795, 0.8897)

temperature: 0.8
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.0385  (95% CI: -0.3846, 0.2692)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3016, 0.7582)
- Strict (quadratic): (0.5888, 0.9334)
- Relaxed (nominal): (0.3988, 0.8571)
- Relaxed (quadratic): (0.6884, 0.9680)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        2        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        2        2       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        2        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        1        1       12

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
    Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
    Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
    Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.