Correct matches: 16 out of 25 students
Total marks Assigned / Total marks Expected: 51 / 48

Cohen's kappa:
- Strict (nominal): 0.4125
- Strict (quadratic-weighted): 0.7234
- Relaxed via acceptance sets (nominal): 0.5296
- Relaxed via acceptance sets (quadratic-weighted): 0.7534

Strict accuracy: 0.6400
Relaxed accuracy: 0.7200
Strict accuracy 95% CI: (0.4452, 0.7975)
Relaxed accuracy 95% CI: (0.5242, 0.8572)

temperature: 0.6
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.1200  (95% CI: -0.2400, 0.4800)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.1813, 0.6390)
- Strict (quadratic): (0.4066, 0.9168)
- Relaxed (nominal): (0.2611, 0.7826)
- Relaxed (quadratic): (0.4344, 0.9434)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        3        0        1
Teacher=1        0        0        0        0
Teacher=2        0        1        0        2
Teacher=3        0        2        0       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        2        0        1
Teacher=1        0        0        0        0
Teacher=2        0        0        1        2
Teacher=3        0        2        0       12

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the students graphs.