Correct matches: 23 out of 26 students
Total marks Assigned / Total marks Expected: 46 / 48

Cohen's kappa:
- Strict (nominal): 0.8030
- Strict (quadratic-weighted): 0.9401
- Relaxed via acceptance sets (nominal): 0.8677
- Relaxed via acceptance sets (quadratic-weighted): 0.9497

Strict accuracy: 0.8846
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.7102, 0.9600)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 1
top_p: 0.9
seed: 42424242

Bias (model - expected): -0.0769  (95% CI: -0.2692, 0.0769)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.5919, 1.0000)
- Strict (quadratic): (0.8199, 1.0000)
- Relaxed (nominal): (0.6667, 1.0000)
- Relaxed (quadratic): (0.8326, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        1        1        1
Teacher=3        0        1        0       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        1        0       13

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.