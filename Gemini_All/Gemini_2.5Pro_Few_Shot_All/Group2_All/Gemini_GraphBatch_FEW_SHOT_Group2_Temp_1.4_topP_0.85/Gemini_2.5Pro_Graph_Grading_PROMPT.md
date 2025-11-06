Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 45 / 48

Cohen's kappa:
- Strict (nominal): 0.7065
- Strict (quadratic-weighted): 0.9450
- Relaxed via acceptance sets (nominal): 0.9352
- Relaxed via acceptance sets (quadratic-weighted): 0.9897

Strict accuracy: 0.8077
Relaxed accuracy: 0.9615
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.8111, 0.9932)

temperature: 1.4
top_p: 0.85
seed: 42424242

Bias (model - expected): -0.1154  (95% CI: -0.2692, 0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4800, 0.9270)
- Strict (quadratic): (0.8775, 0.9860)
- Relaxed (nominal): (0.7892, 1.0000)
- Relaxed (quadratic): (0.9617, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        4       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        1       13

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
    Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
    Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
    Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.