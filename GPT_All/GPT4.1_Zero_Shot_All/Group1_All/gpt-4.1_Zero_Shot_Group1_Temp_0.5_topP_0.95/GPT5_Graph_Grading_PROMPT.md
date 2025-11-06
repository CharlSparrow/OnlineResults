Correct matches: 23 out of 26 students
Total marks Assigned / Total marks Expected: 47 / 48

Cohen's kappa:
- Strict (nominal): 0.8055
- Strict (quadratic-weighted): 0.9077
- Relaxed via acceptance sets (nominal): 0.9343
- Relaxed via acceptance sets (quadratic-weighted): 0.9581

Strict accuracy: 0.8846
Relaxed accuracy: 0.9615
Strict accuracy 95% CI: (0.7102, 0.9600)
Relaxed accuracy 95% CI: (0.8111, 0.9932)

temperature: 0.5
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.0385  (95% CI: -0.2692, 0.1923)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.5895, 1.0000)
- Strict (quadratic): (0.7644, 1.0000)
- Relaxed (nominal): (0.7931, 1.0000)
- Relaxed (quadratic): (0.8527, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        1        0
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        0        0        1       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        0       14

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.