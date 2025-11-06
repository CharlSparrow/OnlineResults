Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 51 / 48

Cohen's kappa:
- Strict (nominal): 0.6494
- Strict (quadratic-weighted): 0.8937
- Relaxed via acceptance sets (nominal): 0.8716
- Relaxed via acceptance sets (quadratic-weighted): 0.9461

Strict accuracy: 0.7692
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 0.7
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.1154  (95% CI: -0.0769, 0.3462)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4222, 0.8693)
- Strict (quadratic): (0.7558, 0.9736)
- Relaxed (nominal): (0.6905, 1.0000)
- Relaxed (quadratic): (0.8338, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        3        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        2       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        1        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        0       14

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.