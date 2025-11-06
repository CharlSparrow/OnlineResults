Correct matches: 22 out of 26 students
Total marks Assigned / Total marks Expected: 46 / 48

Cohen's kappa:
- Strict (nominal): 0.7374
- Strict (quadratic-weighted): 0.8802
- Relaxed via acceptance sets (nominal): 0.8646
- Relaxed via acceptance sets (quadratic-weighted): 0.9021

Strict accuracy: 0.8462
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.6647, 0.9385)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 1.4
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.0769  (95% CI: -0.3846, 0.1538)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.5115, 0.9290)
- Strict (quadratic): (0.6566, 0.9905)
- Relaxed (nominal): (0.6524, 1.0000)
- Relaxed (quadratic): (0.6775, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        1        1        1
Teacher=3        1        0        0       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        1        0        0       13

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.