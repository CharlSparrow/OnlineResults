Correct matches: 24 out of 26 students
Total marks Assigned / Total marks Expected: 48 / 48

Cohen's kappa:
- Strict (nominal): 0.8667
- Strict (quadratic-weighted): 0.9190
- Relaxed via acceptance sets (nominal): 0.9343
- Relaxed via acceptance sets (quadratic-weighted): 0.9581

Strict accuracy: 0.9231
Relaxed accuracy: 0.9615
Strict accuracy 95% CI: (0.7586, 0.9786)
Relaxed accuracy 95% CI: (0.8111, 0.9932)

temperature: 0.7
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0000  (95% CI: -0.2308, 0.2308)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.6837, 1.0000)
- Strict (quadratic): (0.7846, 1.0000)
- Relaxed (nominal): (0.7931, 1.0000)
- Relaxed (quadratic): (0.8527, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        1        0
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        0        0        0       14

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        0       14

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.