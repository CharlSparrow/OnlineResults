Correct matches: 16 out of 26 students
Total marks Assigned / Total marks Expected: 55 / 48

Cohen's kappa:
- Strict (nominal): 0.3939
- Strict (quadratic-weighted): 0.6783
- Relaxed via acceptance sets (nominal): 0.5094
- Relaxed via acceptance sets (quadratic-weighted): 0.7312

Strict accuracy: 0.6154
Relaxed accuracy: 0.6923
Strict accuracy 95% CI: (0.4253, 0.7757)
Relaxed accuracy 95% CI: (0.5001, 0.8350)

temperature: 0.6
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.2692  (95% CI: -0.1154, 0.6538)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.1651, 0.6210)
- Strict (quadratic): (0.3961, 0.8722)
- Relaxed (nominal): (0.2811, 0.7333)
- Relaxed (quadratic): (0.4639, 0.9205)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        3        2        1
Teacher=1        0        0        0        0
Teacher=2        1        0        1        1
Teacher=3        0        0        2       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        3        2        1
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        0        1       13

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.