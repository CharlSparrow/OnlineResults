Correct matches: 18 out of 26 students
Total marks Assigned / Total marks Expected: 42 / 48

Cohen's kappa:
- Strict (nominal): 0.5185
- Strict (quadratic-weighted): 0.8349
- Relaxed via acceptance sets (nominal): 0.8646
- Relaxed via acceptance sets (quadratic-weighted): 0.9021

Strict accuracy: 0.6923
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.5001, 0.8350)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 1.4
top_p: 0.85
seed: 42424242

Bias (model - expected): -0.2308  (95% CI: -0.5385, 0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.2731, 0.7387)
- Strict (quadratic): (0.6086, 0.9605)
- Relaxed (nominal): (0.6524, 1.0000)
- Relaxed (quadratic): (0.6775, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        2        0        1
Teacher=3        1        0        3       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        1        0        0       13

Tolerated off-diagonal hits (count): 6
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.