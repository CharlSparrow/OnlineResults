Correct matches: 23 out of 26 students
Total marks Assigned / Total marks Expected: 51 / 48

Cohen's kappa:
- Strict (nominal): 0.8035
- Strict (quadratic-weighted): 0.9683
- Relaxed via acceptance sets (nominal): 0.8660
- Relaxed via acceptance sets (quadratic-weighted): 0.9795

Strict accuracy: 0.8846
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.7102, 0.9600)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 0.7
top_p: 0.9
seed: 42424242

Bias (model - expected): 0.1154  (95% CI: 0.0000, 0.2308)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.6035, 1.0000)
- Strict (quadratic): (0.9264, 1.0000)
- Relaxed (nominal): (0.6814, 1.0000)
- Relaxed (quadratic): (0.9440, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        2        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        0        0       14

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        0        0       14

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.