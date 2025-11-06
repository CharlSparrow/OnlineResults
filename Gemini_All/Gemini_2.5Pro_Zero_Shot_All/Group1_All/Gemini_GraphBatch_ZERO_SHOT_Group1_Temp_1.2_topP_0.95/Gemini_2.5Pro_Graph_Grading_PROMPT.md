Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 39 / 48

Cohen's kappa:
- Strict (nominal): 0.6725
- Strict (quadratic-weighted): 0.7477
- Relaxed via acceptance sets (nominal): 0.8020
- Relaxed via acceptance sets (quadratic-weighted): 0.7931

Strict accuracy: 0.8077
Relaxed accuracy: 0.8846
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.7102, 0.9600)

temperature: 1.2
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.3462  (95% CI: -0.7692, 0.0000)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4196, 0.8805)
- Strict (quadratic): (0.4880, 0.9527)
- Relaxed (nominal): (0.5687, 1.0000)
- Relaxed (quadratic): (0.5360, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        2        0        1        0
Teacher=3        2        0        0       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        2        0        0       12

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.