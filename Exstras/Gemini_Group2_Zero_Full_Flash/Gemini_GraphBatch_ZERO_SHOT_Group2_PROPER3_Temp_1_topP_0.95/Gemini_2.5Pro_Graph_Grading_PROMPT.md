Correct matches: 16 out of 25 students
Total marks Assigned / Total marks Expected: 53 / 48

Cohen's kappa:
- Strict (nominal): 0.4032
- Strict (quadratic-weighted): 0.5214
- Relaxed via acceptance sets (nominal): 0.5219
- Relaxed via acceptance sets (quadratic-weighted): 0.5568

Strict accuracy: 0.6400
Relaxed accuracy: 0.7200
Strict accuracy 95% CI: (0.4452, 0.7975)
Relaxed accuracy 95% CI: (0.5242, 0.8572)

temperature: 1
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.2000  (95% CI: -0.2800, 0.6800)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.1216, 0.6719)
- Strict (quadratic): (0.0932, 0.8286)
- Relaxed (nominal): (0.1987, 0.7962)
- Relaxed (quadratic): (0.1170, 0.8608)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        1        0        3
Teacher=1        0        0        0        0
Teacher=2        0        1        1        1
Teacher=3        0        2        1       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        0        0        3
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        2        1       11

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the students graphs.