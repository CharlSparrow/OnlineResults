Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 48 / 48

Cohen's kappa:
- Strict (nominal): 0.6119
- Strict (quadratic-weighted): 0.8140
- Relaxed via acceptance sets (nominal): 0.7432
- Relaxed via acceptance sets (quadratic-weighted): 0.8598

Strict accuracy: 0.7692
Relaxed accuracy: 0.8462
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.6647, 0.9385)

temperature: 1.4
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0000  (95% CI: -0.3077, 0.3077)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3735, 0.8506)
- Strict (quadratic): (0.6108, 0.9526)
- Relaxed (nominal): (0.5116, 0.9342)
- Relaxed (quadratic): (0.6667, 0.9885)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        0        2        0
Teacher=1        0        0        0        0
Teacher=2        1        1        0        1
Teacher=3        0        1        0       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        0        2        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        1        0       13

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.