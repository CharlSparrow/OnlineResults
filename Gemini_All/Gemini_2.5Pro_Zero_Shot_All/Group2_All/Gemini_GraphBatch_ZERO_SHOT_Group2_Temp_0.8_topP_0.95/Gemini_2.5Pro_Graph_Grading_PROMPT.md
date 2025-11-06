Correct matches: 22 out of 26 students
Total marks Assigned / Total marks Expected: 44 / 48

Cohen's kappa:
- Strict (nominal): 0.7463
- Strict (quadratic-weighted): 0.8995
- Relaxed via acceptance sets (nominal): 0.8741
- Relaxed via acceptance sets (quadratic-weighted): 0.9476

Strict accuracy: 0.8462
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.6647, 0.9385)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 0.8
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.1538  (95% CI: -0.3846, 0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.5272, 0.9312)
- Strict (quadratic): (0.7535, 0.9905)
- Relaxed (nominal): (0.6782, 1.0000)
- Relaxed (quadratic): (0.8298, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        1        1        1        0
Teacher=3        0        1        0       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        1        0       13

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.