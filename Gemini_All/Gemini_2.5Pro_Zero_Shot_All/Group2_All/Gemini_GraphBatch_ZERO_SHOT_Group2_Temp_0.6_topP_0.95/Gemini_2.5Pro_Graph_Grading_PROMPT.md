Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 48 / 48

Cohen's kappa:
- Strict (nominal): 0.6471
- Strict (quadratic-weighted): 0.8648
- Relaxed via acceptance sets (nominal): 0.7581
- Relaxed via acceptance sets (quadratic-weighted): 0.8898

Strict accuracy: 0.7692
Relaxed accuracy: 0.8462
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.6647, 0.9385)

temperature: 0.6
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0000  (95% CI: -0.2692, 0.2692)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4335, 0.8639)
- Strict (quadratic): (0.6916, 0.9686)
- Relaxed (nominal): (0.5357, 0.9384)
- Relaxed (quadratic): (0.7151, 0.9890)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        2        1        0
Teacher=1        0        0        0        0
Teacher=2        0        1        2        0
Teacher=3        0        1        1       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        1        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        1        1       12

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.