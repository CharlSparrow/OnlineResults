Correct matches: 19 out of 26 students
Total marks Assigned / Total marks Expected: 54 / 48

Cohen's kappa:
- Strict (nominal): 0.5787
- Strict (quadratic-weighted): 0.8818
- Relaxed via acceptance sets (nominal): 0.7419
- Relaxed via acceptance sets (quadratic-weighted): 0.9233

Strict accuracy: 0.7308
Relaxed accuracy: 0.8462
Strict accuracy 95% CI: (0.5392, 0.8630)
Relaxed accuracy 95% CI: (0.6647, 0.9385)

temperature: 0.7
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.2308  (95% CI: 0.0375, 0.4615)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3587, 0.7979)
- Strict (quadratic): (0.7468, 0.9598)
- Relaxed (nominal): (0.5210, 0.9305)
- Relaxed (quadratic): (0.8020, 0.9895)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        4        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        0        1       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        2        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        0        0       14

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.