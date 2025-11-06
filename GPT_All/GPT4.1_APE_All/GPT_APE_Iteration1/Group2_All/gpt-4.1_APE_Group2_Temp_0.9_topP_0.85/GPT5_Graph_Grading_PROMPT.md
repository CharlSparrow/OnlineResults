Correct matches: 18 out of 26 students
Total marks Assigned / Total marks Expected: 53 / 47

Cohen's kappa:
- Strict (nominal): 0.5140
- Strict (quadratic-weighted): 0.8416
- Relaxed via acceptance sets (nominal): 0.6321
- Relaxed via acceptance sets (quadratic-weighted): 0.8975

Strict accuracy: 0.6923
Relaxed accuracy: 0.7692
Strict accuracy 95% CI: (0.5001, 0.8350)
Relaxed accuracy 95% CI: (0.5795, 0.8897)

temperature: 0.9
top_p: 0.85
seed: 42424242

Bias (model - expected): 0.2308  (95% CI: -0.0385, 0.5000)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3088, 0.7306)
- Strict (quadratic): (0.6922, 0.9432)
- Relaxed (nominal): (0.4072, 0.8564)
- Relaxed (quadratic): (0.7784, 0.9702)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        4        4        1        0
Teacher=1        0        0        0        0
Teacher=2        1        0        1        2
Teacher=3        0        0        0       13

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        3        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        2
Teacher=3        0        0        0       13

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
TASK
You are grading hand-drawn graphs of the inverse logarithmic function (base 2). Use the attached memorandum drawing as ground truth. Grade each student independently. Follow the rubric exactly. Output must follow the schema below with no extra prose or headers.

RUBRIC (apply in this order; each awarded = 1 mark; total out of 3)
A. ASYMPTOTE (y-axis at x=0)
   • Award if the drawn curve does NOT clearly cross the y-axis.
   • Touching or brushing the axis counts as NOT crossing.
   • Axis ticks, labels, or arrowheads are NOT the curve.
   • Deduct only when a visible part of the curve lies to the left of the y-axis.

B. X-INTERCEPT at (1;0)
   • Award if any of the following are present near x≈1 on the x-axis:
     (i) a dot with a nearby “1” label,
     (ii) the coordinate (1;0) or (1,0),
     (iii) “x=1”.
   • x-intercept tolerance: treat markings from x=0.8 to x=1.2 as at x=1.
   • Do NOT infer the intercept from curve shape alone if there is no dot/label/crossing.

C. SHAPE of a log curve with base >1
   • Award if the main curve is increasing and concave down, with a steep left tail as x→0⁺ and a slowly rising right tail.
   • The curve may be rough; if it shows some curvature at the ends and is overall increasing, award (borderline S17-type drawings qualify).
   • Deduct if the drawing is obviously an exponential (concave up), a straight line with no curvature, or decreasing.

AMBIGUITY POLICY
• For A and B: if ambiguous, AWARD.
• For C: award when there is some curvature and monotone increase; otherwise deduct.

WHAT TO IGNORE
• Page ruling, shading, smudges, erasures, arrowheads, labels such as “h⁻¹”, and stray pencil marks.
• If multiple curves appear, choose the one nearest the first quadrant that approaches the y-axis from the right.

STRICT vs RELAXED
• STRICT mark (“Mark”) is the sum of A/B/C decisions above (0–3). ErrorTags must match these decisions exactly.
• RELAXED potential marks (“PotentialMarks”) list all marks that could reasonably be awarded under generous interpretation:
  – award A and/or B if borderline,
  – award C if there is some curvature and monotone increase.
• PotentialMarks must be a sorted list of unique integers from {0,1,2,3} and MUST include the strict mark.

OUTPUT CONTRACT (MANDATORY — do not deviate)
For EACH student, output exactly the following block. Use plain text, no markdown. Do not add blank lines between fields other than those shown. Do not echo examples. Do not write “3/3” anywhere except the single Mark line. Do not restate earlier students’ marks.

Student <number>
Mark: `<X>/3`     <-- appears exactly once for this student
ErrorTags: [shape,x_intercept,asymptote] as [0/1,0/1,0/1]
Reasons:
• Shape: <one concise sentence stating why awarded/deducted>
• x-intercept: <one concise sentence>
• Asymptote: <one concise sentence>
PotentialMarks: [<comma-separated integers from {0,1,2,3}>]

NOTES FOR REASONS
• Keep each reason to one sentence, factual and tied to the rubric.
• Use only numerals and standard coordinate forms (e.g., (1;0) or (1,0)) inside the Reasons.
• Never include any additional “/3” strings anywhere in Reasons or PotentialMarks.

IN-CONTEXT EXAMPLES (for understanding only — DO NOT OUTPUT THESE; they use “of” to avoid the “/3” token)
Example A (perfect memo-like)
Student EX-A
Mark: `3 of 3`
ErrorTags: [1,1,1]
Reasons:
• Shape: Increasing, concave-down log curve matching the memo.
• x-intercept: Dot and label at x=1 on the x-axis.
• Asymptote: Curve approaches but does not cross the y-axis.
PotentialMarks: [3]

Example B (borderline S17-like)
Student EX-B
Mark: `2 of 3`
ErrorTags: [1,1,0]  (or [1,1,1] if it only touches)
Reasons:
• Shape: Mostly straight but bends at ends and is overall increasing, so award shape.
• x-intercept: “1” marked on the x-axis near the crossing at x≈1.
• Asymptote: [state “crosses” if any part lies left of the y-axis; otherwise “does not cross”].
PotentialMarks: [1,2,3]

Example C (exponential S6-like)
Student EX-C
Mark: `0 of 3`
ErrorTags: [0,0,0]
Reasons:
• Shape: Exponential (concave up) rather than logarithmic.
• x-intercept: No valid (1;0) indication on the x-axis.
• Asymptote: Drawing not consistent with a log graph’s y-axis asymptote.
PotentialMarks: [0,1]

NOW GRADE
Using the rules above and the attached memorandum image plus the 26 student images, produce one block per student numbered 1 to 26 using the exact Output Contract. Do not include any summary or extra text before, between, or after the student blocks.
