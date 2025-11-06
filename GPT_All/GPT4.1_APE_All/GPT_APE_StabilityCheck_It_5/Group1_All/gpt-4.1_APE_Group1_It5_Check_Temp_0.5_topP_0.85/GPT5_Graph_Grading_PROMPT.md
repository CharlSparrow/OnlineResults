Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 42 / 45

Cohen's kappa:
- Strict (nominal): 0.7130
- Strict (quadratic-weighted): 0.9416
- Relaxed via acceptance sets (nominal): 0.8839
- Relaxed via acceptance sets (quadratic-weighted): 0.9771

Strict accuracy: 0.8077
Relaxed accuracy: 0.9231
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.7586, 0.9786)

temperature: 0.5
top_p: 0.85
seed: 424242420

Bias (model - expected): -0.1154  (95% CI: -0.2692, 0.0385)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.4718, 0.8850)
- Strict (quadratic): (0.8668, 0.9810)
- Relaxed (nominal): (0.7079, 1.0000)
- Relaxed (quadratic): (0.9324, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        5        1
Teacher=3        0        0        4        7

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        0        0        6        0
Teacher=3        0        0        2        9

Tolerated off-diagonal hits (count): 3
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
TASK
Grade 26 hand-drawn graphs of the logarithmic function (base 2) against the attached memorandum drawing. Grade each student independently.

HARD RULES ABOUT AXES
• If either Cartesian axis is absent, unusably faint/erased, or the curve is drawn off-axes: assign 0/3 (A=0, B=0, C=0). Do NOT infer from the curve alone.

MULTIPLE CURVES ON ONE SET OF AXES
• If more than one substantive curve is drawn on the same axes, DEFAULT to 0/3 unless ALL are true:
  (i) the inverse curve is unambiguously identified as “h⁻¹” along its own stroke,
  (ii) other curve(s) can be ignored without any ambiguity, and
  (iii) EVERY piece of evidence used for A/B/C is clearly attached to the h⁻¹ curve itself.
• If any doubt remains (curve identities, shared/ambiguous labels, or which curve crosses/approaches which axis), assign 0/3.
• NEVER borrow labels/coordinates from a different curve to award any mark.

CURVE SELECTION (when not zeroed by the rule above)
• Grade ONLY the inverse curve “h⁻¹”. If no label exists, choose the curve that approaches the y-axis from the RIGHT and lies in/near the first quadrant. If two candidates still fit, treat as ambiguous ⇒ 0/3.

SCORING (three binary checks → total 0–3)  [A first, then B, then C]
Check A — Asymptote at the y-axis (x=0)
• AWARD if the entire h⁻¹ curve stays in x>0.
• Touching/overlap due to line thickness, a tiny nib, or a smudge is OK (still award).
• DEDUCT ONLY if a continuous segment of the h⁻¹ stroke lies on or left of x=0, OR the curve clearly passes from right to left at any point.
• Ignore arrowheads, ticks, labels, faint guidelines/erasures. A lone plotted point left of the axis (e.g., (½;−1)) does NOT cause a deduction.
• DEPENDENCY: If A=0 because the curve runs along the y-axis or enters x≤0, set C=0 (a valid base-2 log cannot live in x≤0).

Check B — x-intercept exactly at (1;0)  [STRICT EVIDENCE; OWNERSHIP REQUIRED]
• AWARD only if at least ONE is observed AND clearly attached to the h⁻¹ curve:
  – the text “(1;0)” or “(1,0)” (note the order 1 then 0), or
  – the text “x=1”, or
  – a dot/crossing on the x-axis at x≈1 WITH a nearby explicit “1” label.
• DO NOT award for: unlabeled dot; “1” without a dot; a bare crossing; “(0;1)”; “(½;−1)”; “2”; ticks/generic marks; labels that plausibly belong to another curve.
• Tolerance (for the labeled dot/crossing): accept positions within 0.9–1.1 of the tick spacing.

Check C — Logarithmic shape (base 2)
• AWARD only if BOTH base conditions hold:
  1) monotone increasing on its visible branch, AND
  2) concave down over a clear majority of the branch (not mostly straight).
• AND at least ONE behavior cue is evident:
  3) left end near x→0⁺ markedly steeper than the right tail, and/or
  4) left end trends toward negative y while the right tail flattens as x increases.
• DEDUCT (C=0) if the h⁻¹ candidate looks hyperbolic (tracks along an axis), is concave up (exponential-like), nearly straight, decreasing, or extends visibly into x≤0.
• Borderline award allowed only when ends clearly bend and a steep-to-flat pattern is visible (S17/S1-type). Otherwise C=0.

EVIDENCE TRANSCRIPTION (required before deciding)
• Before assigning marks, extract what you SEE for each student:
  – Axes: present/absent.
  – Curve count on the axes: <number>; h⁻¹ label present? <yes/no>.
  – Left-of-y evidence: “none / tiny nib / continuous segment length≈<…>”.
  – X-intercept tokens (quote verbatim in order): e.g., “(0;1)”, “(1;0)”, “x=1”, “unlabeled dot”.
  – Accepted for B (and why attached to h⁻¹): <list/none>.
  – Curvature summary: “increasing + concave down / straightish / concave up / hyperbolic along axis”.
• If you cannot quote an acceptable token for B, set B=0. If you cannot rule out left-of-axis contact except for smudge/thickness, AWARD A.

CONSISTENCY CHECK (must pass)
• ErrorTags must be [shape(C), x_intercept(B), asymptote(A)] as 0/1.
• Mark must equal the sum of ErrorTags (0–3). If not, adjust the mark to match the tags.

TIE-BREAKERS
• Never infer B from crossing alone. Without an acceptable token, B=0.
• “1/3” should be rare: use it only when exactly one of C,B,A clearly holds.

WHAT TO IGNORE
• Page ruling, smudges, erasures, arrowheads, ticks, faint guidelines, and labels not attached to h⁻¹.

OUTPUT CONTRACT (strict, parseable)
For EACH student 1..26, output exactly this block — no extra prose, no extra blank lines, and do not restate other students. The token “/3” must appear exactly once per student.

Student <number>
Mark: `<X>/3`     <-- appears exactly once for this student
ErrorTags: [shape,x_intercept,asymptote] as [0/1,0/1,0/1]  <-- maps to C,B,A respectively
Findings:
• Axes: <present/absent>; Curves on axes: <n>; h⁻¹ label: <yes/no>.
• Left-of-y evidence: <none/tiny nib/continuous segment ~…>.
• X-intercept tokens (verbatim): <list>; Accepted for B: <list/none>.
• Curvature summary: <one clause per rules above>.
Reasons:
• Shape: <why C=1 or C=0 per the curvature and cues>
• x-intercept: <why B=1 or B=0 based on accepted tokens attached to h⁻¹>
• Asymptote: <why A=1 or A=0; mention continuous left-of-axis or absence thereof>

CALIBRATION SNIPPETS (DO NOT OUTPUT; for decision consistency)
• S6-type (hyperbolic/overlaps y-axis, multi-curve): lower “h⁻¹” runs along/crosses the y-axis; labels belong to other curves → A=0, B=0, C=0 ⇒ 0/3.
• Lower straight-ish segment: monotone but almost linear, no concave-down log shape → C=0. If axes present and no B evidence → 0/3 (or 1/3 only if A=1).
• No axes: Axes absent → 0/3.
• Writes “(0;1)” (not “(1;0)”): B=0 unless explicit “(1;0)”/“x=1”/labeled dot at x≈1 is also present for h⁻¹.
• Borderline but bends at ends and is increasing (S17/S1): C=1 provided the steep-to-flat pattern is visible and curve stays in x>0.
• “(1;0)” text present (even without a dot) and clearly attached to h⁻¹ → B=1.
• Curve crosses near x≈1 but NO label/coordinate → B=0.
• Axes missing → A=0, B=0; C may be 0 or 1 depending on shape (thus only 0/3 or 1/3 possible).
• S11/S3-style near-touch at y-axis: no continuous left-of-axis segment → A=1.
• S19-style multiple curves with no B token for h⁻¹: B=0 (overall ≤2/3).