Correct matches: 22 out of 26 students
Total marks Assigned / Total marks Expected: 41 / 48

Cohen's kappa:
- Strict (nominal): 0.7541
- Strict (quadratic-weighted): 0.8494
- Relaxed via acceptance sets (nominal): 0.8143
- Relaxed via acceptance sets (quadratic-weighted): 0.8585

Strict accuracy: 0.8462
Relaxed accuracy: 0.8846
Strict accuracy 95% CI: (0.6647, 0.9385)
Relaxed accuracy 95% CI: (0.7102, 0.9600)

temperature: 1.2
top_p: 0.85
seed: 42424242

Bias (model - expected): -0.2692  (95% CI: -0.5769, -0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.5357, 0.9363)
- Strict (quadratic): (0.6225, 0.9897)
- Relaxed (nominal): (0.5969, 1.0000)
- Relaxed (quadratic): (0.6278, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        1        2        0
Teacher=3        1        1        1       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        1        1        1       11

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.