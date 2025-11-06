Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 51 / 45

Cohen's kappa:
- Strict (nominal): 0.7105
- Strict (quadratic-weighted): 0.9064
- Relaxed via acceptance sets (nominal): 0.7636
- Relaxed via acceptance sets (quadratic-weighted): 0.9204

Strict accuracy: 0.8077
Relaxed accuracy: 0.8462
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.6647, 0.9385)

temperature: 0.9
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.2308  (95% CI: 0.0769, 0.4231)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4879, 0.8850)
- Strict (quadratic): (0.7816, 0.9794)
- Relaxed (nominal): (0.5498, 0.9402)
- Relaxed (quadratic): (0.7985, 0.9891)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        2        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        4        2
Teacher=3        0        0        0       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        1        1        0
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
