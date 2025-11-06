Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 43 / 48

Cohen's kappa:
- Strict (nominal): 0.7052
- Strict (quadratic-weighted): 0.8833
- Relaxed via acceptance sets (nominal): 0.8182
- Relaxed via acceptance sets (quadratic-weighted): 0.9065

Strict accuracy: 0.8077
Relaxed accuracy: 0.8846
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.7102, 0.9600)

temperature: 1.2
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.1923  (95% CI: -0.4615, 0.0000)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4961, 0.8832)
- Strict (quadratic): (0.7315, 0.9802)
- Relaxed (nominal): (0.6111, 1.0000)
- Relaxed (quadratic): (0.7564, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        1        2        0
Teacher=3        0        2        1       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        2        1       11

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3. The memorandum shows an example of a perfect 3/3 graph.
    Student 1 is an example of a 2/3 graph, the shape of this graph is considered incorrect.
    Student 6 is an example of a 0/3 graph, the student drew an exponential graph, which is not a log graph as required, thus receiving zero out of three.
    Use these examplars to guide you in your assessment of all the student graphs from student 1 to student 26.