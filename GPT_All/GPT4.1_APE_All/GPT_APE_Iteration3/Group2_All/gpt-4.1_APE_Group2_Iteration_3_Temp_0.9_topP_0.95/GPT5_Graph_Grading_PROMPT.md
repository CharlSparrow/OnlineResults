Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 52 / 47

Cohen's kappa:
- Strict (nominal): 0.7092
- Strict (quadratic-weighted): 0.8675
- Relaxed via acceptance sets (nominal): 0.8182
- Relaxed via acceptance sets (quadratic-weighted): 0.8966

Strict accuracy: 0.8077
Relaxed accuracy: 0.8846
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.7102, 0.9600)

temperature: 0.9
top_p: 0.95
seed: 42424242

Bias (model - expected): 0.1923  (95% CI: -0.0385, 0.4615)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4957, 0.9290)
- Strict (quadratic): (0.6929, 0.9783)
- Relaxed (nominal): (0.6224, 1.0000)
- Relaxed (quadratic): (0.7329, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        5        2        2        0
Teacher=1        0        0        0        0
Teacher=2        0        0        4        0
Teacher=3        0        0        1       12

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        6        1        2        0
Teacher=1        0        0        0        0
Teacher=2        0        0        4        0
Teacher=3        0        0        0       13

Tolerated off-diagonal hits (count): 2
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
TASK
Grade 26 hand-drawn graphs of the inverse logarithmic function (base 2) against the attached memorandum drawing. Grade each student independently.

SCORING (three binary checks → total is 0–3)
Check A — Asymptote at the y-axis (x=0)
  • AWARD if the curve does NOT clearly cross into x<0.
  • Touching/overlapping the axis because of line thickness is OK (still award).
  • Ignore axis arrowheads/ticks/labels and faint guidelines/erasures; those are not the curve.
  • A single plotted point left of the axis (e.g., (½;−1)) does NOT cause a deduction.
  • DEDUCT only when a continuous part of the drawn curve lies left of the y-axis.

Check B — x-intercept exactly at (1;0)  [EVIDENCE REQUIRED]
  • AWARD only if at least ONE of the following appears:
    – the coordinate text “(1;0)” or “(1,0)” anywhere on the page, or
    – the text “x=1” anywhere on the page, or
    – a dot/crossing on the x-axis at x≈1 WITH a nearby “1” label.
  • DO NOT award for: unlabeled dot on the axis, a “1” written near the axis without a dot,
    a bare crossing of the curve through the x-axis, “(0;1)”, “(½;−1)”, “2”, ticks, or generic marks.
  • Tolerance for the labeled dot/crossing: accept 0.9–1.1 of the tick spacing as “at 1”.

Check C — Log shape (base >1)
  • AWARD if the main curve is overall increasing and concave down (steep near x→0⁺, flatter to the right).
  • Hand sketches may be rough; if the ends bend and it is monotone increasing, AWARD (S17/S1-type).
  • DEDUCT for clear exponential (concave up), a straight line with no visible curvature, or a decreasing curve.

PREREQUISITES (axes handling)
  • If EITHER axis is missing or not drawn (no visible coordinate axes), set A=0 and B=0.
    Shape (C) may still be awarded if the curve alone clearly looks like a log; otherwise C=0.
    (Max possible without axes is 1/3.)

MULTIPLE CURVES
  • Only grade the intended inverse log curve. If several curves appear, use the one labeled “h⁻¹”;
    otherwise choose the curve that approaches the y-axis from the RIGHT and lies in the first quadrant neighborhood.
  • Do not use markings/labels from other curves (“h”, exponential distractors) to award any check.

TIE-BREAKERS / CALIBRATION
  • Never infer B from shape/crossing alone. Missing the explicit tokens above → B=0.
  • 1/3 should be rare: use it when exactly one of C,B,A clearly holds (common case: axes absent → only C may hold).

WHAT TO IGNORE
  • Page ruling, smudges, erasures, stray pencil marks, arrowheads, axis ticks, and faint guidelines.

OUTPUT CONTRACT (strict, parseable)
For EACH student 1..26, output exactly this block — no extra prose, no blank lines between fields, and do not restate other students’ marks. The token “/3” must appear exactly once in each student’s block.

Student <number>
Mark: `<X>/3`     <-- appears exactly once for this student
ErrorTags: [shape,x_intercept,asymptote] as [0/1,0/1,0/1]  <-- maps to C,B,A respectively
Reasons:
• Shape: <one sentence stating why awarded/deducted for C>
• x-intercept: <one sentence for B; cite explicit evidence or the lack thereof>
• Asymptote: <one sentence for A>

CALIBRATION SNIPPETS (for your decision process; DO NOT OUTPUT)
• S11-type: “(1;0)” text present (even without a dot) → B=1.
• S19-type: curve crosses near x≈1 but NO label/coordinate → B=0.
• S17/S1-type: mostly straight midsection but bends at ends and is increasing → C=1.
• S23/S24-type: axes missing → A=0, B=0; C may be 0 or 1 depending on shape (thus only 0/3 or 1/3 possible).
