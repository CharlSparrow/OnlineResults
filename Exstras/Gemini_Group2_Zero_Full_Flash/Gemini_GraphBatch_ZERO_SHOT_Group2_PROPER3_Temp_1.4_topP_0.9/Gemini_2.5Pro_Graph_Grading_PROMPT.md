Correct matches: 12 out of 26 students
Total marks Assigned / Total marks Expected: 47 / 48

Cohen's kappa:
- Strict (nominal): 0.1670
- Strict (quadratic-weighted): 0.2237
- Relaxed via acceptance sets (nominal): 0.2212
- Relaxed via acceptance sets (quadratic-weighted): 0.2288

Strict accuracy: 0.4615
Relaxed accuracy: 0.5000
Strict accuracy 95% CI: (0.2876, 0.6454)
Relaxed accuracy 95% CI: (0.3206, 0.6794)

temperature: 1.4
top_p: 0.9
seed: 42424242

Bias (model - expected): -0.0385  (95% CI: -0.6538, 0.6154)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (-0.0734, 0.3929)
- Strict (quadratic): (-0.1953, 0.5762)
- Relaxed (nominal): (-0.0493, 0.4846)
- Relaxed (quadratic): (-0.1936, 0.5845)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        1        0        4
Teacher=1        0        0        0        0
Teacher=2        0        2        0        1
Teacher=3        2        3        1        8

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        1        0        4
Teacher=1        0        0        0        0
Teacher=2        0        1        1        1
Teacher=3        2        3        1        8

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.