Correct matches: 13 out of 26 students
Total marks Assigned / Total marks Expected: 70 / 48

Cohen's kappa:
- Strict (nominal): 0.3860
- Strict (quadratic-weighted): 0.4848
- Relaxed via acceptance sets (nominal): 0.4619
- Relaxed via acceptance sets (quadratic-weighted): 0.5231

Strict accuracy: 0.5000
Relaxed accuracy: 0.5385
Strict accuracy 95% CI: (0.3206, 0.6794)
Relaxed accuracy 95% CI: (0.3546, 0.7124)

temperature: 0.6
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.8462  (95% CI: 0.0385, 1.6923)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.0657, 0.7062)
- Strict (quadratic): (0.0493, 0.8493)
- Relaxed (nominal): (0.1169, 0.7912)
- Relaxed (quadratic): (0.0810, 0.8714)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        2        2        0        1
Teacher=1        0        0        0        0
Teacher=2        1        0        1        1
Teacher=3        2        0        0       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        1        0        1
Teacher=1        0        0        0        0
Teacher=2        1        0        1        1
Teacher=3        2        0        0       10

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.