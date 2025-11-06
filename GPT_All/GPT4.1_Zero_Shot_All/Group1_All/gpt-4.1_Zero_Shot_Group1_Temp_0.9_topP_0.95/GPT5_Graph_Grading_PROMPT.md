Correct matches: 8 out of 26 students
Total marks Assigned / Total marks Expected: 62 / 48

Cohen's kappa:
- Strict (nominal): -0.1471
- Strict (quadratic-weighted): -0.0854
- Relaxed via acceptance sets (nominal): -0.1134
- Relaxed via acceptance sets (quadratic-weighted): -0.0560

Strict accuracy: 0.3077
Relaxed accuracy: 0.3462
Strict accuracy 95% CI: (0.1650, 0.4999)
Relaxed accuracy 95% CI: (0.1941, 0.5378)

temperature: 0.9
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.5385  (95% CI: -0.1538, 1.1923)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.3198, 0.0319)
- Strict (quadratic): (-0.3762, 0.2346)
- Relaxed (nominal): (-0.2919, 0.0663)
- Relaxed (quadratic): (-0.3452, 0.2624)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        0        2        1        6
Teacher=1        0        0        0        0
Teacher=2        0        0        0        3
Teacher=3        2        1        3        8

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        0        2        1        6
Teacher=1        0        0        0        0
Teacher=2        0        0        0        3
Teacher=3        2        1        2        9

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.