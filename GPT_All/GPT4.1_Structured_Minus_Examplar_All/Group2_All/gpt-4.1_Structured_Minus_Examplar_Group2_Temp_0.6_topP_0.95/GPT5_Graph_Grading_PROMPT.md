Correct matches: 17 out of 26 students
Total marks Assigned / Total marks Expected: 61 / 47

Cohen's kappa:
- Strict (nominal): 0.4455
- Strict (quadratic-weighted): 0.5973
- Relaxed via acceptance sets (nominal): 0.4964
- Relaxed via acceptance sets (quadratic-weighted): 0.6166

Strict accuracy: 0.6538
Relaxed accuracy: 0.6923
Strict accuracy 95% CI: (0.4622, 0.8059)
Relaxed accuracy 95% CI: (0.5001, 0.8350)

temperature: 0.6
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.5385  (95% CI: 0.1923, 0.9231)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.1875, 0.6887)
- Strict (quadratic): (0.3279, 0.8201)
- Relaxed (nominal): (0.2604, 0.7347)
- Relaxed (quadratic): (0.3558, 0.8395)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        0        5        1
Teacher=1        0        0        0        0
Teacher=2        0        0        2        2
Teacher=3        0        0        1       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        3        0        5        1
Teacher=1        0        0        0        0
Teacher=2        0        0        2        2
Teacher=3        0        0        0       13

Tolerated off-diagonal hits (count): 1
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
Using the memorandum grade the 26 students graphs X/3.

The memorandum defines three marks that can be obtained, making the maximum mark three:
A mark for the shape (vorm) of the graph being similar to that of a logarithmic graph with base two. The shape of the logarithmic graph is generally considered correct should the part of the graph above the x-axis is roughly pointing to the right.
A mark for correctly writing out the co-ordinate of the intersection between the logarithmic graph and the x-axis (x-afsnit). The correct co-ordinate is (1;0), it is also correct if the student draws a dot where the logarithmic graph intersects the x-axis and then writes a "1" nearby.
A mark for the students graph correctly respecting the asymptote (assimptoot), thus meaning that the students graph does not cross y-axis. Should there be ambiguity the student should be awarded the mark, meaning if it comes very close but does not actually cross the y-axis they still get the mark, a mark here should only be deducted if it appears that the student truely intentionally crossed the y-axis since this is a graph drawn by hand pencil artifacts etc likely make it look more wrong than it is.
