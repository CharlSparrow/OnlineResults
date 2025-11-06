Correct matches: 17 out of 26 students
Total marks Assigned / Total marks Expected: 56 / 48

Cohen's kappa:
- Strict (nominal): 0.4236
- Strict (quadratic-weighted): 0.4268
- Relaxed via acceptance sets (nominal): 0.4236
- Relaxed via acceptance sets (quadratic-weighted): 0.4268

Strict accuracy: 0.6538
Relaxed accuracy: 0.6538
Strict accuracy 95% CI: (0.4622, 0.8059)
Relaxed accuracy 95% CI: (0.4622, 0.8059)

temperature: 1.2
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.3077  (95% CI: -0.2308, 0.8462)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.1229, 0.6934)
- Strict (quadratic): (0.0358, 0.7489)
- Relaxed (nominal): (0.1229, 0.6934)
- Relaxed (quadratic): (0.0358, 0.7489)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        0        2        3
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        1        1        1       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        0        2        3
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        1        1        1       11

Tolerated off-diagonal hits (count): 0
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.