Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 36 / 48

Cohen's kappa:
- Strict (nominal): 0.6303
- Strict (quadratic-weighted): 0.7526
- Relaxed via acceptance sets (nominal): 0.8729
- Relaxed via acceptance sets (quadratic-weighted): 0.8703

Strict accuracy: 0.7692
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 1
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.4615  (95% CI: -0.8462, -0.1538)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3966, 0.8560)
- Strict (quadratic): (0.5111, 0.9240)
- Relaxed (nominal): (0.6790, 1.0000)
- Relaxed (quadratic): (0.6389, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        2        0        1        0
Teacher=3        1        2        1       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        1        1        0       12

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.