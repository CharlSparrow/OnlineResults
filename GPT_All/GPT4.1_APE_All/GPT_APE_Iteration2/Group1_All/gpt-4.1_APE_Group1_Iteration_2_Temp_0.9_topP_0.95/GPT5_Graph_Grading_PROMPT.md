Correct matches: 18 out of 26 students
Total marks Assigned / Total marks Expected: 50 / 45

Cohen's kappa:
- Strict (nominal): 0.5273
- Strict (quadratic-weighted): 0.8749
- Relaxed via acceptance sets (nominal): 0.7668
- Relaxed via acceptance sets (quadratic-weighted): 0.9184

Strict accuracy: 0.6923
Relaxed accuracy: 0.8462
Strict accuracy 95% CI: (0.5001, 0.8350)
Relaxed accuracy 95% CI: (0.6647, 0.9385)

temperature: 0.9
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.1923  (95% CI: -0.0385, 0.4231)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.2506, 0.7615)
- Strict (quadratic): (0.7325, 0.9570)
- Relaxed (nominal): (0.5408, 0.9413)
- Relaxed (quadratic): (0.7893, 0.9890)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        1        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        2        4
Teacher=3        0        0        2        9

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        1        0
Teacher=1        0        0        0        0
Teacher=2        0        0        5        1
Teacher=3        0        0        2        9

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
TASK
Grade 26 hand-drawn graphs of the inverse logarithmic function (base 2) against the attached memorandum drawing. Grade each student independently.

SCORING (three binary checks → total is 0–3)
Check A — Asymptote at the y-axis (x=0):
  • AWARD if the curve does NOT clearly cross into x<0.
  • Touching/overlapping the axis line because of thickness is OK (still award).
  • Ignore axis arrowheads/ticks/labels; those are not the curve.
  • DEDUCT only if a drawn portion of the curve lies left of the y-axis.

Check B — x-intercept exactly at (1;0):
  • AWARD only with explicit evidence at x≈1 on the x-axis:
    – a dot/crossing at the x-axis with a nearby “1”, or
    – the coordinate (1;0)/(1,0), or
    – the text “x=1”.
  • Tolerance: accept 0.9–1.1 of the tick spacing as “at 1”.
  • DO NOT award for: “(0;1)” (that is y-intercept), “(½;−1)”, “2”, or unlabeled nearby dots.
  • If ambiguous or unreadable → DO NOT award. (Evidence required.)

Check C — Log-shape (base >1):
  • AWARD if overall increasing and concave down: steep rise near x→0⁺ and flattening to the right.
  • Hand sketches may be rough; if ends bend and the curve is monotone increasing, AWARD (e.g., S17-type).
  • DEDUCT for clear exponential (concave up), a straight line with no visible curvature, or a decreasing curve.

WHAT TO IGNORE
• Page ruling, smudges, erasures, stray pencil marks, labels such as “h⁻¹”, and axis arrowheads/ticks.
• If multiple candidates exist, choose the curve nearest the first quadrant that approaches the y-axis from the right.
• The memo’s marked point (½;−1) is a reference point, NOT an intercept — do not use it to award B.

TIE-BREAKERS / CALIBRATION
• Never infer B from shape alone. Missing labels/dots → B=0.
• Only output “1/3” when exactly one of A,B,C is clearly satisfied and the other two clearly fail. If evidence for a second check is uncertain, prefer “2/3” or “0/3” as the checks justify — do not guess.

OUTPUT CONTRACT (strict, parseable)
For EACH student 1..26, output exactly this block — no extra prose, no blank lines between fields, and do not restate other students’ marks. The token “/3” must appear exactly once in each student’s block.

Student <number>
Mark: `<X>/3`     <-- appears exactly once for this student
ErrorTags: [shape,x_intercept,asymptote] as [0/1,0/1,0/1]  <-- C,B,A in that order mapped to [shape,x_intercept,asymptote]
Reasons:
• Shape: <one sentence stating why awarded/deducted for C>
• x-intercept: <one sentence for B; must cite explicit evidence or the lack thereof>
• Asymptote: <one sentence for A>
