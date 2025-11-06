Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 42 / 48

Cohen's kappa:
- Strict (nominal): 0.6934
- Strict (quadratic-weighted): 0.8383
- Relaxed via acceptance sets (nominal): 0.8729
- Relaxed via acceptance sets (quadratic-weighted): 0.8703

Strict accuracy: 0.8077
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 1
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.2308  (95% CI: -0.5769, 0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4846, 0.8774)
- Strict (quadratic): (0.6043, 0.9806)
- Relaxed (nominal): (0.6750, 1.0000)
- Relaxed (quadratic): (0.6371, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        2        1        0
Teacher=3        1        1        0       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        3        0
Teacher=3        1        1        0       12

Tolerated off-diagonal hits (count): 3
Model     0 1 2 3
Teacher=0 0,1,0,0
Teacher=1 0,0,0,0
Teacher=2 0,2,0,0
Teacher=3 0,0,0,0


 Prompt used: 
Using the memo grade the 26 students graphs X/3.