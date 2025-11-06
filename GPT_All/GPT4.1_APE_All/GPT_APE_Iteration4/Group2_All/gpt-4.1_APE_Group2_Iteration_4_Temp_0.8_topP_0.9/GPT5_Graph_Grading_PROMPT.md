Correct matches: 20 out of 26 students
Total marks Assigned / Total marks Expected: 48 / 47

Cohen's kappa:
- Strict (nominal): 0.6389
- Strict (quadratic-weighted): 0.8141
- Relaxed via acceptance sets (nominal): 0.8098
- Relaxed via acceptance sets (quadratic-weighted): 0.8524

Strict accuracy: 0.7692
Relaxed accuracy: 0.8846
Strict accuracy 95% CI: (0.5795, 0.8897)
Relaxed accuracy 95% CI: (0.7102, 0.9600)

temperature: 0.8
top_p: 0.9
seed: 42424242

Bias (model - expected): 0.0385  (95% CI: -0.2692, 0.3471)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.3915, 0.8653)
- Strict (quadratic): (0.5445, 0.9690)
- Relaxed (nominal): (0.5854, 1.0000)
- Relaxed (quadratic): (0.5905, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        7        1        0        1
Teacher=1        0        0        0        0
Teacher=2        0        1        2        1
Teacher=3        0        1        1       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        0        0        1
Teacher=1        0        0        0        0
Teacher=2        0        0        3        1
Teacher=3        0        1        0       12

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
TASK
Grade 26 hand-drawn graphs of the inverse logarithmic function (base 2) against the attached memorandum drawing. Grade each student independently.

HARD RULE ABOUT AXES
• If either Cartesian axis is absent or the curve is drawn without axes, assign 0/3 (A=0, B=0, C=0). Do not infer anything from the curve alone.
• If axes exist but are clearly unrelated to the graded curve (e.g., drawn elsewhere), treat as “axes absent”.

CURVE SELECTION
• Grade ONLY the inverse log curve. If multiple curves appear, prefer the one labeled “h⁻¹”. If none is labeled, choose the curve that approaches the y-axis from the RIGHT and lies near the first quadrant. Do NOT use marks/labels from a different curve (e.g., “h”) to award any criterion.

SCORING (three binary checks → total 0–3)
Check A — Asymptote at the y-axis (x=0)
• AWARD if the entire h⁻¹ curve stays strictly in x>0.
• Small nibs from pen thickness that just touch are OK. 
• DEDUCT if a continuous piece of the drawn curve lies on or left of the y-axis, OR the curve runs along the y-axis for a visible segment, OR it clearly passes from right to left at any point.
• Ignore arrowheads, ticks, labels, faint guidelines/erasures. A single plotted point left of the axis (e.g., (½;−1)) does NOT cause a deduction.

Check B — x-intercept exactly at (1;0)  [EVIDENCE REQUIRED]
• AWARD if at least ONE of the following appears:
  – the text “(1;0)” or “(1,0)” anywhere on the page, OR
  – the text “x=1” anywhere on the page, OR
  – a dot/crossing on the x-axis at x≈1 WITH a nearby explicit “1” label.
• DO NOT award for: unlabeled dot on the axis; a “1” written near the axis without a dot; a bare crossing of the curve through the x-axis; “(0;1)”; “(½;−1)”; “2”; ticks or generic marks.
• Tolerance for the labeled dot/crossing: accept positions within 0.9–1.1 of the tick spacing.

Check C — Logarithmic shape (base 2)
• AWARD only if ALL of the following base conditions hold:
  1) The chosen curve is **monotone increasing** on its drawn branch, and
  2) It is **concave down** over most of the visible branch.
• AND at least **one** of the two behavior cues holds (→ require 3 of 4 cues total):
  3) The **left end** approaches the y-axis (x close to 0⁺) more steeply than the right end (i.e., left is “more vertical”, right is “flatter”), and/or
  4) The **left end** heads downward (toward negative y) as it nears the y-axis, while the right tail flattens as x increases.
• DEDUCT (C=0) for any of: obvious exponential (concave up), nearly straight line with no visible curvature, decreasing behavior, hyperbolic-looking branch that tracks along the y-axis, or a branch that extends visibly into x≤0.
• Borderline award is allowed only when the ends clearly bend and the steep-to-flat pattern is evident (e.g., S17-type). Otherwise C=0.

TIE-BREAKERS
• Never infer B from curve crossing alone. If the explicit evidence list is missing, set B=0.
• “1/3” should be rare: use it only when exactly one of C, B, A clearly holds.

WHAT TO IGNORE
• Page ruling, smudges, erasures, arrowheads, ticks, faint guidelines, labels like “h⁻¹” that overlap the curve. These are not the curve.

OUTPUT CONTRACT (strict, parseable)
For EACH student 1..26, output exactly this block — no extra prose, no extra blank lines, and do not restate other students. The token “/3” must appear exactly once per student.

Student <number>
Mark: `<X>/3`     <-- appears exactly once for this student
ErrorTags: [shape,x_intercept,asymptote] as [0/1,0/1,0/1]  <-- maps to C,B,A respectively
Reasons:
• Shape: <one sentence stating why awarded/deducted for C using the cues above>
• x-intercept: <one sentence for B; cite explicit evidence or the lack thereof>
• Asymptote: <one sentence for A; mention crossing/overlap or staying in x>0>

CALIBRATION SNIPPETS (DO NOT OUTPUT; for decision consistency)
(hyperbolic/overlaps y-axis): lower “h⁻¹” runs along/crosses the y-axis and is not concave down → A=0, C=0, B=0 ⇒ 0/3.
(lower straight-ish segment): monotone but almost linear, no concave-down log shape → C=0. If axes present and no B evidence → 0/3 (or 1/3 only if A=1 and C=0 fails).
(no axes): Axes absent → 0/3.
(writes “(0;1)”, not “(1;0)”): B=0 unless explicit “(1;0)”/“x=1”/labeled dot at x≈1 is also present.
(borderline but bends at ends and is increasing): C=1 provided the steep-to-flat pattern is visible.
“(1;0)” text present (even without a dot) → B=1.
curve crosses near x≈1 but NO label/coordinate → B=0.
• axes missing → A=0, B=0; C may be 0 or 1 depending on shape (thus only 0/3 or 1/3 possible).
