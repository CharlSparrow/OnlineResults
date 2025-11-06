Correct matches: 19 out of 26 students
Total marks Assigned / Total marks Expected: 41 / 48

Cohen's kappa:
- Strict (nominal): 0.5892
- Strict (quadratic-weighted): 0.7804
- Relaxed via acceptance sets (nominal): 0.9342
- Relaxed via acceptance sets (quadratic-weighted): 0.9108

Strict accuracy: 0.7308
Relaxed accuracy: 0.9615
Strict accuracy 95% CI: (0.5392, 0.8630)
Relaxed accuracy 95% CI: (0.8111, 0.9932)

temperature: 1.4
top_p: 0.9
seed: 42424242

Bias (model - expected): -0.2692  (95% CI: -0.6538, 0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3516, 0.8107)
- Strict (quadratic): (0.5353, 0.9504)
- Relaxed (nominal): (0.7689, 1.0000)
- Relaxed (quadratic): (0.6857, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        2        0        0
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        1        1        2       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        1        0        0       13

Tolerated off-diagonal hits (count): 6
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.