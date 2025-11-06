Correct matches: 18 out of 26 students
Total marks Assigned / Total marks Expected: 43 / 48

Cohen's kappa:
- Strict (nominal): 0.5196
- Strict (quadratic-weighted): 0.8233
- Relaxed via acceptance sets (nominal): 0.6941
- Relaxed via acceptance sets (quadratic-weighted): 0.8823

Strict accuracy: 0.6923
Relaxed accuracy: 0.8077
Strict accuracy 95% CI: (0.5001, 0.8350)
Relaxed accuracy 95% CI: (0.6212, 0.9149)

temperature: 0.7
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.1923  (95% CI: -0.5000, 0.0769)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.2930, 0.7347)
- Strict (quadratic): (0.6371, 0.9352)
- Relaxed (nominal): (0.4693, 0.8874)
- Relaxed (quadratic): (0.7191, 0.9800)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        2        0        0
Teacher=1        0        0        0        0
Teacher=2        1        1        0        1
Teacher=3        0        2        1       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        2        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        2        0       12

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.