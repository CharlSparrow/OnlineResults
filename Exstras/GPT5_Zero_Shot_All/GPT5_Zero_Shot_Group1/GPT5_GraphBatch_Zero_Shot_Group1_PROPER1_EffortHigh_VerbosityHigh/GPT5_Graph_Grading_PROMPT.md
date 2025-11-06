Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 49 / 48

Cohen's kappa:
- Strict (nominal): 0.6381
- Strict (quadratic-weighted): 0.9001
- Relaxed via acceptance sets (nominal): 0.8060
- Relaxed via acceptance sets (quadratic-weighted): 0.9380

Strict accuracy: 0.7692
Relaxed accuracy: 0.8846
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.7102, 0.9600)

temperature: 0.7
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0385  (95% CI: -0.1923, 0.2308)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3967, 0.8602)
- Strict (quadratic): (0.7604, 0.9719)
- Relaxed (nominal): (0.5873, 1.0000)
- Relaxed (quadratic): (0.8148, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        3        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        1        1       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        1        0       13

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.