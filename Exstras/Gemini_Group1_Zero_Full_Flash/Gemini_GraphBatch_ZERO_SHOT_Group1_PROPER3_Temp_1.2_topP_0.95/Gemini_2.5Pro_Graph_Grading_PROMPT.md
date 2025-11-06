Correct matches: 19 out of 26 students
Total marks Assigned / Total marks Expected: 45 / 48

Cohen's kappa:
- Strict (nominal): 0.5816
- Strict (quadratic-weighted): 0.9246
- Relaxed via acceptance sets (nominal): 0.8045
- Relaxed via acceptance sets (quadratic-weighted): 0.9688

Strict accuracy: 0.7308
Relaxed accuracy: 0.8846
Strict accuracy 95% CI: (0.5392, 0.8630)
Relaxed accuracy 95% CI: (0.7102, 0.9600)

temperature: 1.2
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.1154  (95% CI: -0.3077, 0.0769)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3333, 0.8074)
- Strict (quadratic): (0.8440, 0.9719)
- Relaxed (nominal): (0.5738, 1.0000)
- Relaxed (quadratic): (0.9173, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        1        1        1
Teacher=3        0        0        4       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        1
Teacher=3        0        0        1       13

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memo grade the 26 students graphs.