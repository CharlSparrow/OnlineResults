Correct matches: 15 out of 26 students
Total marks Assigned / Total marks Expected: 48 / 48

Cohen's kappa:
- Strict (nominal): 0.4066
- Strict (quadratic-weighted): 0.7524
- Relaxed via acceptance sets (nominal): 0.6018
- Relaxed via acceptance sets (quadratic-weighted): 0.8428

Strict accuracy: 0.5769
Relaxed accuracy: 0.7308
Strict accuracy 95% CI: (0.3895, 0.7446)
Relaxed accuracy 95% CI: (0.5392, 0.8630)

temperature: 0.5
top_p: 0.9
seed: 42424242

Bias (model - expected): 0.0000  (95% CI: -0.3462, 0.3077)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.1993, 0.6103)
- Strict (quadratic): (0.5452, 0.8889)
- Relaxed (nominal): (0.3853, 0.8178)
- Relaxed (quadratic): (0.6623, 0.9549)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        5        1        0
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        0        1        3       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        4        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        1        1       12

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.