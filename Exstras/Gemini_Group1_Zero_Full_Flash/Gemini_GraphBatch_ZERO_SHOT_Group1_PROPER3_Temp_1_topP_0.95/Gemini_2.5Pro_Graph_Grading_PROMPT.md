Correct matches: 23 out of 26 students
Total marks Assigned / Total marks Expected: 41 / 48

Cohen's kappa:
- Strict (nominal): 0.8102
- Strict (quadratic-weighted): 0.8130
- Relaxed via acceptance sets (nominal): 0.8700
- Relaxed via acceptance sets (quadratic-weighted): 0.8251

Strict accuracy: 0.8846
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.7102, 0.9600)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 1
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.2692  (95% CI: -0.6154, 0.0000)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.5761, 1.0000)
- Strict (quadratic): (0.5452, 1.0000)
- Relaxed (nominal): (0.6613, 1.0000)
- Relaxed (quadratic): (0.5591, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        2        0        1       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        2        0        0       12

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the students graphs.