Correct matches: 13 out of 26 students
Total marks Assigned / Total marks Expected: 34 / 48

Cohen's kappa:
- Strict (nominal): 0.3240
- Strict (quadratic-weighted): 0.8231
- Relaxed via acceptance sets (nominal): 0.7025
- Relaxed via acceptance sets (quadratic-weighted): 0.9469

Strict accuracy: 0.5000
Relaxed accuracy: 0.8077
Strict accuracy 95% CI: (0.3206, 0.6794)
Relaxed accuracy 95% CI: (0.6212, 0.9149)

temperature: 0.7
top_p: 0.85
seed: 42424242

Bias (model - expected): -0.5385  (95% CI: -0.7692, -0.3462)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.1195, 0.5218)
- Strict (quadratic): (0.6844, 0.9091)
- Relaxed (nominal): (0.4694, 0.9144)
- Relaxed (quadratic): (0.8791, 0.9855)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        1        2        0        0
Teacher=3        0        0       10        4

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        1        2        0
Teacher=3        0        0        4       10

Tolerated off-diagonal hits (count): 8
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.