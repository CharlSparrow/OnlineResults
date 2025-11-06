Correct matches: 10 out of 26 students
Total marks Assigned / Total marks Expected: 41 / 48

Cohen's kappa:
- Strict (nominal): 0.0437
- Strict (quadratic-weighted): 0.0063
- Relaxed via acceptance sets (nominal): 0.0972
- Relaxed via acceptance sets (quadratic-weighted): 0.0095

Strict accuracy: 0.3846
Relaxed accuracy: 0.4231
Strict accuracy 95% CI: (0.2243, 0.5747)
Relaxed accuracy 95% CI: (0.2554, 0.6105)

temperature: 0.8
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.2692  (95% CI: -1.0000, 0.4615)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.2122, 0.2886)
- Strict (quadratic): (-0.3809, 0.3791)
- Relaxed (nominal): (-0.1904, 0.3769)
- Relaxed (quadratic): (-0.3879, 0.3858)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        0        1        4
Teacher=1        0        0        0        0
Teacher=2        0        2        0        1
Teacher=3        5        2        1        6

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        0        1        4
Teacher=1        0        0        0        0
Teacher=2        0        1        1        1
Teacher=3        5        2        1        6

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.