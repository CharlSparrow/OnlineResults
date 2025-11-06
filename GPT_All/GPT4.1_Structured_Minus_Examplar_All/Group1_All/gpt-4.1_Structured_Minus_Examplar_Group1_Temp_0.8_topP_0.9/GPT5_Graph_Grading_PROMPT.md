Correct matches: 19 out of 26 students
Total marks Assigned / Total marks Expected: 53 / 45

Cohen's kappa:
- Strict (nominal): 0.5835
- Strict (quadratic-weighted): 0.7398
- Relaxed via acceptance sets (nominal): 0.6455
- Relaxed via acceptance sets (quadratic-weighted): 0.7795

Strict accuracy: 0.7308
Relaxed accuracy: 0.7692
Strict accuracy 95% CI: (0.5392, 0.8630)
Relaxed accuracy 95% CI: (0.5795, 0.8897)

temperature: 0.8
top_p: 0.9
seed: 42424242

Bias (model - expected): 0.3077  (95% CI: 0.0000, 0.6163)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3217, 0.8121)
- Strict (quadratic): (0.5124, 0.9024)
- Relaxed (nominal): (0.3915, 0.8673)
- Relaxed (quadratic): (0.5726, 0.9320)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        0        4        0
Teacher=1        0        0        0        0
Teacher=2        1        0        3        2
Teacher=3        0        0        0       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        0        4        0
Teacher=1        0        0        0        0
Teacher=2        0        0        4        2
Teacher=3        0        0        0       11

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memorandum grade the 26 students graphs X/3.

The memorandum defines three marks that can be obtained, making the maximum mark three:
A mark for the shape (vorm) of the graph being similar to that of a logarithmic graph with base two. The shape of the logarithmic graph is generally considered correct should the part of the graph above the x-axis is roughly pointing to the right.
A mark for correctly writing out the co-ordinate of the intersection between the logarithmic graph and the x-axis (x-afsnit). The correct co-ordinate is (1;0), it is also correct if the student draws a dot where the logarithmic graph intersects the x-axis and then writes a "1" nearby.
A mark for the students graph correctly respecting the asymptote (assimptoot), thus meaning that the students graph does not cross y-axis. Should there be ambiguity the student should be awarded the mark, meaning if it comes very close but does not actually cross the y-axis they still get the mark, a mark here should only be deducted if it appears that the student truely intentionally crossed the y-axis since this is a graph drawn by hand pencil artifacts etc likely make it look more wrong than it is.
