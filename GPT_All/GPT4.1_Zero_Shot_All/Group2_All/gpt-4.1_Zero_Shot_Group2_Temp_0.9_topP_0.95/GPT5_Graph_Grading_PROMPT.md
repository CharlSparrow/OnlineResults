Correct matches: 6 out of 26 students
Total marks Assigned / Total marks Expected: 39 / 48

Cohen's kappa:
- Strict (nominal): 0.0796
- Strict (quadratic-weighted): 0.6027
- Relaxed via acceptance sets (nominal): 0.4606
- Relaxed via acceptance sets (quadratic-weighted): 0.8019

Strict accuracy: 0.2308
Relaxed accuracy: 0.6154
Strict accuracy 95% CI: (0.1103, 0.4205)
Relaxed accuracy 95% CI: (0.4253, 0.7757)

temperature: 0.9
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.3462  (95% CI: -0.7308, 0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.0648, 0.2268)
- Strict (quadratic): (0.3939, 0.7516)
- Relaxed (nominal): (0.2607, 0.6766)
- Relaxed (quadratic): (0.6142, 0.9174)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        5        1        0
Teacher=1        0        0        0        0
Teacher=2        1        2        0        0
Teacher=3        0        1       10        3

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        4        1        0
Teacher=1        0        0        0        0
Teacher=2        0        1        2        0
Teacher=3        0        1        3       10

Tolerated off-diagonal hits (count): 10
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.