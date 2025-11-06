Correct matches: 18 out of 26 students
Total marks Assigned / Total marks Expected: 51 / 48

Cohen's kappa:
- Strict (nominal): 0.5367
- Strict (quadratic-weighted): 0.7993
- Relaxed via acceptance sets (nominal): 0.7025
- Relaxed via acceptance sets (quadratic-weighted): 0.8731

Strict accuracy: 0.6923
Relaxed accuracy: 0.8077
Strict accuracy 95% CI: (0.5001, 0.8350)
Relaxed accuracy 95% CI: (0.6212, 0.9149)

temperature: 0.5
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.1154  (95% CI: -0.1923, 0.4231)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3333, 0.7508)
- Strict (quadratic): (0.6013, 0.9258)
- Relaxed (nominal): (0.4902, 0.9196)
- Relaxed (quadratic): (0.7039, 0.9782)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        5        1        0
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        0        1        0       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        3        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        1        0       13

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.