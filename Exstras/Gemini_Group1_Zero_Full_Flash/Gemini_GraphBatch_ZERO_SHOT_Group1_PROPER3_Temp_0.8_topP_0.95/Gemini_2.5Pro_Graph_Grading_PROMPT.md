Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 50 / 48

Cohen's kappa:
- Strict (nominal): 0.6750
- Strict (quadratic-weighted): 0.8323
- Relaxed via acceptance sets (nominal): 0.7990
- Relaxed via acceptance sets (quadratic-weighted): 0.8562

Strict accuracy: 0.8077
Relaxed accuracy: 0.8846
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.7102, 0.9600)

temperature: 0.8
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0769  (95% CI: -0.1923, 0.3846)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4268, 0.8719)
- Strict (quadratic): (0.5771, 0.9799)
- Relaxed (nominal): (0.5491, 1.0000)
- Relaxed (quadratic): (0.5986, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        1        0        1
Teacher=1        0        0        0        0
Teacher=2        0        1        1        1
Teacher=3        0        1        0       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        0        1
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        1        0       13

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.