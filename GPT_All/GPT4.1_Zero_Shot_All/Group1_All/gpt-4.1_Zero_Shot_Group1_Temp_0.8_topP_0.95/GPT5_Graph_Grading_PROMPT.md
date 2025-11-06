Correct matches: 15 out of 26 students
Total marks Assigned / Total marks Expected: 49 / 48

Cohen's kappa:
- Strict (nominal): 0.4269
- Strict (quadratic-weighted): 0.8554
- Relaxed via acceptance sets (nominal): 0.5574
- Relaxed via acceptance sets (quadratic-weighted): 0.9033

Strict accuracy: 0.5769
Relaxed accuracy: 0.6923
Strict accuracy 95% CI: (0.3895, 0.7446)
Relaxed accuracy 95% CI: (0.5001, 0.8350)

temperature: 0.8
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0385  (95% CI: -0.1923, 0.2692)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.2325, 0.6360)
- Strict (quadratic): (0.7570, 0.9191)
- Relaxed (nominal): (0.3398, 0.7729)
- Relaxed (quadratic): (0.8227, 0.9567)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        6        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        5        9

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        4        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        4       10

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.