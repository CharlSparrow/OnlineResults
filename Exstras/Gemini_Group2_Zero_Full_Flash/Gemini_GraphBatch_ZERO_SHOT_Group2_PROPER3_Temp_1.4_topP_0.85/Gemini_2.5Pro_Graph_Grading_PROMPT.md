Correct matches: 11 out of 26 students
Total marks Assigned / Total marks Expected: 42 / 48

Cohen's kappa:
- Strict (nominal): 0.0972
- Strict (quadratic-weighted): 0.0095
- Relaxed via acceptance sets (nominal): 0.2334
- Relaxed via acceptance sets (quadratic-weighted): 0.0591

Strict accuracy: 0.4231
Relaxed accuracy: 0.5385
Strict accuracy 95% CI: (0.2554, 0.6105)
Relaxed accuracy 95% CI: (0.3546, 0.7124)

temperature: 1.4
top_p: 0.85
seed: 42424242

Bias (model - expected): -0.2308  (95% CI: -0.9615, 0.5000)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.1879, 0.3705)
- Strict (quadratic): (-0.3905, 0.3800)
- Relaxed (nominal): (-0.1049, 0.5315)
- Relaxed (quadratic): (-0.3369, 0.4308)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        0        0        5
Teacher=1        0        0        0        0
Teacher=2        1        1        1        0
Teacher=3        4        2        2        6

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        0        0        5
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        4        2        0        8

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.