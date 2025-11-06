Correct matches: 21 out of 26 students
Total marks Assigned / Total marks Expected: 43 / 45

Cohen's kappa:
- Strict (nominal): 0.7118
- Strict (quadratic-weighted): 0.9141
- Relaxed via acceptance sets (nominal): 0.9402
- Relaxed via acceptance sets (quadratic-weighted): 0.9571

Strict accuracy: 0.8077
Relaxed accuracy: 0.9615
Strict accuracy 95% CI: (0.6212, 0.9149)
Relaxed accuracy 95% CI: (0.8111, 0.9932)

temperature: 0.9
top_p: 0.95
seed: 42424242

Bias (model - expected): -0.0769  (95% CI: -0.3077, 0.1154)

Kappa 95% CIs (bootstrap):
- Strict (nominal): (0.5000, 0.8860)
- Strict (quadratic): (0.7840, 0.9812)
- Relaxed (nominal): (0.8138, 1.0000)
- Relaxed (quadratic): (0.8477, 1.0000)

=== Strict confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        8        1        0        0
Teacher=1        0        0        0        0
Teacher=2        1        2        2        1
Teacher=3        0        0        0       11

=== Relaxed confusion matrix ===
           Model=0  Model=1  Model=2  Model=3
Teacher=0        9        0        0        0
Teacher=1        0        0        0        0
Teacher=2        1        0        5        0
Teacher=3        0        0        0       11

Tolerated off-diagonal hits (count): 4
See confusion_matrix_tolerated_hits.csv for distribution by class.

 Prompt used: 
TASK

Grade 26 hand-drawn graphs of the inverse logarithmic function (base 2) against the attached memorandum. Grade each student independently.

RULE 0 — AXES REQUIRED (hard stop)

If either Cartesian axis is missing, unusable (faint/erased), or the curve is drawn off the axes:

Final Mark = 0/3

Error Tags = [0,0,0]

Reasons must state that Shape/X-intercept/Asymptote cannot be verified without axes.
Do not evaluate any other rules.

MULTIPLE CURVES ON ONE SET OF AXES (near-hard zero)

If more than one substantive curve is drawn on the same axes, default to 0/3 unless all conditions hold:

The inverse curve is unambiguously identified as “h⁻¹” along its own stroke;

The other curve(s) can be ignored without ambiguity; and

Every piece of evidence used for Shape / X-intercept / Asymptote is clearly attached to the h⁻¹ stroke (no borrowed labels).
If any doubt remains (curve identity, shared labels, shared intercepts, etc.) → 0/3.

WHAT TO GRADE (when not zeroed by the rule above)

Grade only the h⁻¹ curve. If no label exists, use the curve that approaches the y-axis from the right and lies near the first quadrant. If two candidates still fit → ambiguous → 0/3.

SCORING (three binary checks → sum is the mark 0–3)
1) SHAPE (vorm) — 1 mark

Award (Shape=1) only if all base conditions hold:

The chosen curve is strictly increasing on its visible branch, and

It is clearly concave down on a majority of the branch (not mostly straight).

…and at least one behavior cue is evident:

Left end near 𝑥→0+ is markedly steeper than the right tail; or

Left end trends towards negative y while the right tail visibly flattens.

Deduct (Shape=0) for any of:

Hyperbolic look (track along an axis),

Concave up / exponential-like,

Predominantly straight or ruler-like (even if slightly wavy or piecewise),

Decreasing anywhere on the drawn branch,

Visible extension into 𝑥≤0.

Borderline allowance: Only if both ends clearly bend and a steep-to-flat pattern is visible (S17/S1-type). Otherwise Shape=0.

2) X-INTERCEPT at (1;0) — 1 mark (strict evidence, attached to h⁻¹)

Award (X=1) only if at least one acceptable token is present and clearly belongs to h⁻¹:

The text “(1;0)” or “(1,0)” (order 1 then 0) written anywhere, and visually associated with the h⁻¹ intercept; or

The text “x=1” written anywhere, and clearly intended for the h⁻¹ intercept; or

A dot on the x-axis at x≈1 with a nearby explicit “1” label that the h⁻¹ curve passes through.

Do NOT award for:
unlabeled dot; “1” without a dot; a bare crossing of the axis; “(0;1)”; “(½;−1)”; “2”; generic ticks; or labels belonging to another curve (e.g., “h”).

Tolerance for the labeled dot/crossing: accept positions within 0.9–1.1 tick spacing of x=1.

3) ASYMPTOTE at the y-axis (x=0) — 1 mark

Award (Asymptote=1) when the entire h⁻¹ stroke remains in x>0.
Axis thickness, tiny nibs, or smudges do not count as crossing.

Deduct (Asymptote=0) if any of the following is true:

A continuous drawn segment of h⁻¹ lies on or left of the y-axis,

The stroke runs along the y-axis for a visible length,

The stroke touches at a clear point (e.g., a vertex at the origin) rather than merely grazing due to thickness,

The curve clearly passes from right to left at any point.

Ignore arrowheads, ticks, labels, faint guidelines/erasures. A single plotted point left of the axis (like 
(12;−1)(21;−1)) does not cause a deduction by itself.

EVIDENCE TRANSCRIPTION (mandatory pre-step)

Before deciding marks, write what you see for each student (keeps the grader honest):

Axes: present/absent.

Curves on the axes: <count>; “h⁻¹” label present? yes/no.

Left-of-y evidence: none / tiny nib / continuous segment ~<…>.

X-intercept tokens (verbatim): e.g., “(0;1)”, “(1;0)”, “x=1”, “unlabeled dot”.

Accepted for X (if any) and why they belong to h⁻¹.

Curvature summary: “increasing + concave down / straightish / concave up / hyperbolic along axis”.

If you cannot quote an acceptable X token attached to h⁻¹, set X=0.
If left-of-axis contact is uncertain and looks like thickness only, award Asymptote=1.

TIE-BREAKERS

Never infer X-intercept from a crossing alone. No acceptable token ⇒ X=0.

“1/3” should be rare (exactly one of Shape/X/Asymptote holds).

WHAT TO IGNORE

Page ruling, smudges, erasures, arrowheads, ticks, faint guidelines, and labels not attached to h⁻¹.

OUTPUT CONTRACT (strict, parseable)

For each student 1..26 output exactly the block below — no extra prose, no blank lines.
The token “/3” must appear exactly once per student.

Student <number>
Mark: `<X>/3`
ErrorTags: [shape,x_intercept,asymptote] as [0/1,0/1,0/1]
Findings:
• Axes: <present/absent>; Curves on axes: <n>; h⁻¹ label: <yes/no>.
• Left-of-y evidence: <none/tiny nib/continuous segment ~…>.
• X-intercept tokens (verbatim): <list>; Accepted for X: <list/none>.
• Curvature summary: <one clause>.
Reasons:
• Shape: <why 1 or 0 per curvature cues>.
• x-intercept: <why 1 or 0 based on accepted tokens attached to h⁻¹>.
• Asymptote: <why 1 or 0; mention continuous left-of-axis or its absence>.

CALIBRATION SNIPPETS (DO NOT OUTPUT; for decision consistency)

S6-type (two full curves on the same axes; h⁻¹ hugs/runs along y-axis): evidence belongs to other curve(s); h⁻¹ shows hyperbolic behavior and y-axis contact → Shape=0, X=0, Asymptote=0 ⇒ Final 0/3.

S8-type (mostly straight, then kicks up; contact at origin or left-of-y): Shape=0 (straight/piecewise & concave-up end); X=0 (no valid token); Asymptote=0 (clear point contact at y-axis/left segment) ⇒ 0/3.

S11-type (good memo-like): clear concave-down increase; “(1;0)” marked for h⁻¹; no continuous left-of-axis stroke → 3/3.

S19-type (multi-curve; no X token for h⁻¹): even if Shape and Asymptote look okay, X=0 (no acceptable token attached to h⁻¹) ⇒ at most 2/3.

No axes (S23/S24-type): Rule 0 triggers → 0/3.

“(0;1)” is not “(1;0)”; do not repurpose; only accept “(1;0)”/“x=1” (or labeled dot at x≈1) attached to h⁻¹.