Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 45 / 48

Cohen's kappa:
- Strict (nominal): 0.5749
- Strict (quadratic-weighted): 0.6911
- Relaxed via acceptance sets (nominal): 0.6515
- Relaxed via acceptance sets (quadratic-weighted): 0.7197

Strict accuracy: 0.7692
Relaxed accuracy: 0.8077
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.6212, 0.9149)

temperature: 1.4
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.1154  (95% CI: -0.5769, 0.3077)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.2909, 0.8475)
- Strict (quadratic): (0.3784, 0.9222)
- Relaxed (nominal): (0.3659, 0.9185)
- Relaxed (quadratic): (0.4000, 0.9719)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        0        1
Teacher=1        0        0        0        0
Teacher=2        1        0        0        2
Teacher=3        2        0        0       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        0        1
Teacher=1        0        0        0        0
Teacher=2        0        0        1        2
Teacher=3        2        0        0       12

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.