Correct matches: 10 out of 26 students
Total marks Assigned / Total marks Expected: 34 / 48

Cohen's kappa:
- Strict (nominal): 0.2180
- Strict (quadratic-weighted): 0.7395
- Relaxed via acceptance sets (nominal): 0.6526
- Relaxed via acceptance sets (quadratic-weighted): 0.9024

Strict accuracy: 0.3846
Relaxed accuracy: 0.7692
Strict accuracy 95% CI: (0.2243, 0.5747)
Relaxed accuracy 95% CI: (0.5795, 0.8897)

temperature: 0.5
top_p: 0.85
seed: 42424242

Bias (model - expected): -0.5385  (95% CI: -0.8462, -0.2692)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.0476, 0.3953)
- Strict (quadratic): (0.5616, 0.8516)
- Relaxed (nominal): (0.4273, 0.8677)
- Relaxed (quadratic): (0.7617, 0.9761)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        2        0        0
Teacher=1        0        0        0        0
Teacher=2        1        2        0        0
Teacher=3        0        1       10        3

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        1        2        0
Teacher=3        0        1        3       10

Tolerated off-diagonal hits (count): 10
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.