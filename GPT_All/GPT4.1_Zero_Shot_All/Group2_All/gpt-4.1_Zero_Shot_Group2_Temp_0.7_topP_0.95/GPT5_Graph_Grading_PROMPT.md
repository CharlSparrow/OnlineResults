Correct matches: 16 out of 26 students
Total marks Assigned / Total marks Expected: 50 / 48

Cohen's kappa:
- Strict (nominal): 0.4444
- Strict (quadratic-weighted): 0.8034
- Relaxed via acceptance sets (nominal): 0.7005
- Relaxed via acceptance sets (quadratic-weighted): 0.9070

Strict accuracy: 0.6154
Relaxed accuracy: 0.8077
Strict accuracy 95% CI: (0.4253, 0.7757)
Relaxed accuracy 95% CI: (0.6212, 0.9149)

temperature: 0.7
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0769  (95% CI: -0.2308, 0.3846)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.2301, 0.6549)
- Strict (quadratic): (0.6273, 0.9145)
- Relaxed (nominal): (0.4857, 0.9196)
- Relaxed (quadratic): (0.7819, 0.9800)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        5        1        0
Teacher=1        0        0        0        0
Teacher=2        1        0        2        0
Teacher=3        0        0        3       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        3        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        0        0        1       13

Tolerated off-diagonal hits (count): 5
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs X/3.