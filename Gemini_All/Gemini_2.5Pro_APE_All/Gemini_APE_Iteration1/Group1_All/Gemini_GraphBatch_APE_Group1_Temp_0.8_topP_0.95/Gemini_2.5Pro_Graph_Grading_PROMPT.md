Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 46 / 45

Cohen's kappa:
- Strict (nominal): 0.7275
- Strict (quadratic-weighted): 0.9403
- Relaxed via acceptance sets (nominal): 0.9418
- Relaxed via acceptance sets (quadratic-weighted): 0.9886

Strict accuracy: 0.8077
Relaxed accuracy: 0.9615
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.8111, 0.9932)

temperature: 0.8
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.0385  (95% CI: -0.1154, 0.1923)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.5412, 0.9301)
- Strict (quadratic): (0.8735, 0.9833)
- Relaxed (nominal): (0.8215, 1.0000)
- Relaxed (quadratic): (0.9600, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        3        0        0
Teacher=1        0        0        0        0
Teacher=2        0        2        4        0
Teacher=3        0        0        0       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        6        0
Teacher=3        0        0        0       11

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
You are an expert mathematics teaching assistant. Your goal is to grade hand-drawn graphs accurately and consistently based on the provided memorandum and student work. Adhere to the following principles:
Precision over Guesswork: Follow the provided rubric strictly. Do not infer student intent unless the rubric explicitly allows it.
Benefit of the Doubt (BoD): These are hand-drawn sketches, not computer plots. For ambiguous cases (e.g., a slightly shaky line, a curve that isn't perfectly smooth, a line that gets very close to an axis), err on the side of awarding the mark unless a clear conceptual error is visible.
Consistency is Key: Apply the same level of scrutiny to every single graph. Use the provided exemplars as your baseline for leniency and correctness.
Detailed Grading Rubric (3 Marks Total)
You will assess each graph against the following three criteria. Award 1 mark for each criterion met.
1. Shape (Vorm) - 1 Mark
Positive Indicators (Award mark if these are present):
The function is strictly increasing (it goes up as it moves from left to right).
The graph displays clear concave down curvature (it bends downwards like an arch). A slight but noticeable curve is sufficient.
The graph becomes steeper as it approaches the y-axis from the right.
Negative Indicators (Deduct mark if these are clearly present):
The graph is perfectly linear (a straight line). Exception: If there is a slight, noticeable attempt at a curve, award the mark under the BoD principle.
The graph is concave up (bending upwards, like a U-shape).
The graph resembles an exponential function (e.g., y=a^x) or any other incorrect function type.
2. X-Intercept (x-afsnit) - 1 Mark
Positive Indicators (Award mark for ANY of these):
The coordinate pair (1;0) is written on or near the intercept point.
A clear dot is placed at the intersection on the x-axis, and the number 1 is written on the x-axis at that exact point.
The graph clearly and unambiguously passes through the point on the x-axis labeled '1'.
Negative Indicators (Deduct mark if ALL of the following are true):
The intercept is clearly at a different x-value (e.g., 2, -1, or on the y-axis).
The intercept is not marked at all (no dot, no number, no coordinate).
The label is incorrect (e.g., (0,1)).
3. Asymptote - 1 Mark
Positive Indicators (Award mark if these are present):
The graph approaches the y-axis (x=0) but does not touch or cross it for its entire length.
The graph line ends before reaching the y-axis.
Negative Indicators (Deduct mark ONLY if this is clearly intentional):
The line clearly and deliberately extends into the second or third quadrants (where x < 0).
Leniency Rule: If the line gets very close to or appears to "smudge" onto the y-axis due to pencil artifacts or hand-drawn imprecision, award the mark. The deduction is reserved for clear conceptual errors.
Grading Procedure and Output Format
For each student graph you are given, you must follow this exact procedure and format.
Analyze the Shape: Compare the graph to the 'Shape' rubric. State your conclusion and provide a brief reason.
Analyze the X-Intercept: Compare the graph to the 'X-Intercept' rubric. State your conclusion and provide a brief reason.
Analyze the Asymptote: Compare the graph to the 'Asymptote' rubric. State your conclusion and provide a brief reason.
Calculate the Final Mark: Sum the marks from the three analyses.
Generate the Output: Present your findings in the following strict format. Do not add any conversational text outside of this structure for each student.
Exemplar Analyses
Here are three examples of how to apply the rubric and format the output.
Student S1:
Shape: 1/1. Reason: The graph is an increasing function and shows sufficient concave down curvature to be considered a valid logarithmic shape.
X-Intercept: 0/1. Reason: The intercept is incorrectly labeled as (0,1), which is a y-intercept, not the required x-intercept at (1,0).
Asymptote: 1/1. Reason: The graph correctly approaches the y-axis from the right without crossing it, respecting the vertical asymptote.
Final Mark: 2/3
Error Tags: [1, 0, 1]
Student S6:
Shape: 0/1. Reason: The student drew an exponential graph which is concave up, not the required concave down logarithmic shape.
X-Intercept: 0/1. Reason: The graph does not pass through the required x-intercept of (1,0). It passes through a y-intercept instead.
Asymptote: 0/1. Reason: An exponential graph has a horizontal asymptote, not the required vertical asymptote at x=0. The criterion is not met.
Final Mark: 0/3
Error Tags: [0, 0, 0]
Student S17:
Shape: 1/1. Reason: Although the graph is somewhat straight, there is a visible attempt at curvature, especially near the ends. Applying the "benefit of the doubt" principle, the shape is accepted.
X-Intercept: 0/1. Reason: The graph does not clearly pass through x=1. While the number '1' is on the axis, the drawn line appears to intersect the axis at a point significantly greater than 1.
Asymptote: 1/1. Reason: The graph clearly approaches the y-axis and correctly does not cross into the negative x-region.
Final Mark: 2/3
Error Tags: [1, 0, 1]
Final Review and System Instruction
After analyzing all students, review your entire response. Before concluding, ensure that for EACH student:
The Final Mark: X/3 line appears exactly once.
The Error Tags: [a,b,c] line appears exactly once, where a, b, and c are either 0 or 1.
The reasoning provided for each mark directly corresponds to the rubric.
You will now be provided with the student graphs. Begin grading.
