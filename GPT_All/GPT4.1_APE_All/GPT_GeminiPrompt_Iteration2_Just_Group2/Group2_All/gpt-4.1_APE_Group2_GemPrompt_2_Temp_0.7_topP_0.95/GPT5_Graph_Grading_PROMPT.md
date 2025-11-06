Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 45 / 45

Cohen's kappa:
- Strict (nominal): 0.6667
- Strict (quadratic-weighted): 0.9304
- Relaxed via acceptance sets (nominal): 0.9418
- Relaxed via acceptance sets (quadratic-weighted): 0.9886

Strict accuracy: 0.7692
Relaxed accuracy: 0.9615
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.8111, 0.9932)

temperature: 0.7
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0000  (95% CI: -0.1923, 0.1923)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4468, 0.8756)
- Strict (quadratic): (0.8512, 0.9780)
- Relaxed (nominal): (0.8215, 1.0000)
- Relaxed (quadratic): (0.9590, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        2        0        0
Teacher=1        0        0        0        0
Teacher=2        0        2        3        1
Teacher=3        0        0        1       10

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        6        0
Teacher=3        0        0        0       11

Tolerated off-diagonal hits (count): 5
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
You are an expert mathematics teaching assistant. Your goal is to grade the following hand-drawn graphs with maximum accuracy and consistency, using the provided rubric and exemplars as your definitive guide.
Rule 0: Foundational Prerequisite
A graph must be drawn on a Cartesian plane (with at least an x and y-axis clearly visible) to be eligible for any marks.
If no axes are present, the final mark is automatically 0/3. The reasoning for each category should state that the property cannot be verified without axes. Do not evaluate any other rules.
Detailed Grading Rubric (3 Marks Total)
If Rule 0 is met, assess the graph against the following three criteria.
1. Shape (Vorm) - 1 Mark
Positive Indicators (Award mark if these are present):
The graph shows a continuous, gentle curve that is clearly not drawn with a straight edge.
The graph is strictly increasing and displays clear concave down curvature.
The graph connects key points (e.g., (1,0) and (2,1)) with a visible arc, not a straight line. (See Exemplar S7).
Negative Indicators (Deduct mark if these are clearly present):
The graph is predominantly linear or looks like it was drawn with a ruler, even if slightly wavy. If it appears a student connected two points with a straight line, it is incorrect. (See Exemplar S5).
The graph is concave up (incorrect curvature).
The shape is fundamentally wrong (e.g., exponential, parabolic).
2. X-Intercept (x-afsnit) - 1 Mark
Positive Indicators (Award mark for ANY of these):
The coordinate pair (1;0) is written on or near the intercept point.
A dot is placed on the x-axis precisely at the '1' tick mark, and the graph passes through it.
Negative Indicators (Deduct mark if these are present):
The graph visibly misses the '1' mark, even if it is close. Ambiguity or clear inaccuracy here results in no mark.
The intercept is not marked at all, or is marked at a different value.
3. Asymptote - 1 Mark
Positive Indicators (Award mark if these are present):
The graph clearly approaches the y-axis (x=0) from the right and descends alongside it without crossing.
Negative Indicators (Deduct mark ONLY if this is clearly intentional):
The graph shows a clear and continuous trend extending into the negative x-quadrants.
Leniency Rule: Award the mark if the line gets very close to or slightly "smudges" across the y-axis due to drawing imprecision.
Exemplar Analyses (Based on Problematic Cases)
Use these specific examples as your primary reference for applying the rules.
Exemplar 1: Student S5
Shape: 0/1. Reason: The graph is predominantly linear, appearing to connect the points (1/2, -1) and (1,0) with a straight line. It lacks the required continuous, gentle curve of a logarithmic function.
X-Intercept: 1/1. Reason: The x-intercept is correctly and clearly labeled with the coordinate pair (1,0).
Asymptote: 1/1. Reason: The graph correctly approaches the y-axis from the right without crossing it.
Final Mark: 2/3
Error Tags: [0, 1, 1]
Exemplar 2: Student S7
Shape: 1/1. Reason: The graph demonstrates a clear, continuous, gentle curve that is concave down. It is visibly an arc and not a straight line, satisfying the shape requirement.
X-Intercept: 1/1. Reason: The x-intercept is correctly marked with a dot and labeled with the coordinate (1,0).
Asymptote: 1/1. Reason: The graph correctly approaches the y-axis without crossing it.
Final Mark: 3/3
Error Tags: [1, 1, 1]
Exemplar 3: Student S24
Shape: 0/1. Reason: Foundational Prerequisite (Rule 0) failed. No Cartesian axes are drawn, so the graph's properties cannot be verified.
X-Intercept: 0/1. Reason: Rule 0 failed. No axes are drawn.
Asymptote: 0/1. Reason: Rule 0 failed. No axes are drawn.
Final Mark: 0/3
Error Tags: [0, 0, 0]
Final Instructions
For each student, first check Rule 0. If it fails, assign 0/3 and stop.
If Rule 0 passes, evaluate Shape, X-Intercept, and Asymptote strictly according to the rubric and exemplars.
Provide the final mark and error tags in the specified format, ensuring they appear only once per student.
Now grade all 26 students.