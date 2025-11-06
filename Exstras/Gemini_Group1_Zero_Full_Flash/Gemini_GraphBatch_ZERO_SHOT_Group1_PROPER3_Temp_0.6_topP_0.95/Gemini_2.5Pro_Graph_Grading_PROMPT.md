Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 51 / 48

Cohen's kappa:
- Strict (nominal): 0.6725
- Strict (quadratic-weighted): 0.8838
- Relaxed via acceptance sets (nominal): 0.7320
- Relaxed via acceptance sets (quadratic-weighted): 0.8973

Strict accuracy: 0.8077
Relaxed accuracy: 0.8462
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.6647, 0.9385)

temperature: 0.6
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.1154  (95% CI: -0.1538, 0.3462)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4222, 0.8716)
- Strict (quadratic): (0.7153, 0.9800)
- Relaxed (nominal): (0.4800, 0.9299)
- Relaxed (quadratic): (0.7347, 0.9902)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        1        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        1        2
Teacher=3        0        1        0       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        1        2
Teacher=3        0        1        0       13

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.