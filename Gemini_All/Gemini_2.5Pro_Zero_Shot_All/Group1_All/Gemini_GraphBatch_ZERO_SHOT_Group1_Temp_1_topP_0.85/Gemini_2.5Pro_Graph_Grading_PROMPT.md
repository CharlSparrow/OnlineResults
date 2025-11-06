Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 43 / 48

Cohen's kappa:
- Strict (nominal): 0.7052
- Strict (quadratic-weighted): 0.8833
- Relaxed via acceptance sets (nominal): 0.9356
- Relaxed via acceptance sets (quadratic-weighted): 0.9592

Strict accuracy: 0.8077
Relaxed accuracy: 0.9615
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.8111, 0.9932)

temperature: 1
top_p: 0.85
seed: 42424242

Bias (model - expected): -0.1923  (95% CI: -0.4615, 0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4770, 0.9259)
- Strict (quadratic): (0.7187, 0.9806)
- Relaxed (nominal): (0.7833, 1.0000)
- Relaxed (quadratic): (0.8440, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        1        2        0
Teacher=3        0        2        1       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        1        0       13

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.