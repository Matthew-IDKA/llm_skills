# Medical Statistics for Laypeople

The single most important skill in reading medical research is translating statistics into plain language. Most alarming (and exciting) health headlines are statistical illusions at the bottom of this page.

---

## Relative Risk vs. Absolute Risk

This is the most important distinction in all of medical statistics.

**Scenario:** A drug reduces your risk of a heart attack by 50%.

- Sounds dramatic.
- If your baseline risk is **2%**, the drug reduces it to **1%** — absolute benefit of 1 percentage point.
- If your baseline risk is **0.2%**, the drug reduces it to **0.1%** — absolute benefit of 0.1 percentage points.

**Formula:**
- Relative Risk Reduction (RRR) = (Control rate − Treatment rate) / Control rate
- Absolute Risk Reduction (ARR) = Control rate − Treatment rate

**Rule of thumb:** Headlines almost always report relative risk. Always ask for the baseline rate to compute the absolute benefit before deciding if something matters.

---

## Number Needed to Treat (NNT)

How many patients must receive a treatment for one patient to benefit?

**Formula:** NNT = 1 / ARR

**Example:** ARR = 1% → NNT = 100
- 100 people take the drug; 1 avoids a heart attack; 99 got side effects with no personal benefit.

**Rough benchmarks:**
| NNT | Interpretation |
|---|---|
| 2–5 | Excellent — strong individual benefit |
| 10–20 | Good for serious conditions |
| 50–100 | Modest — meaningful at population scale, worth scrutiny for the individual |
| 200+ | Low — carefully weigh against side effect profile |

**Number Needed to Harm (NNH):** The same concept for adverse effects. If NNT = 50 and NNH = 30, the drug harms more people than it helps. Compare both before forming an opinion.

A useful pre-computed NNT/NNH resource: **thennt.com**

---

## P-Values

**What it means:** If there were truly no effect, the p-value is the probability of seeing results at least this extreme by chance alone.

**What it does NOT mean:**
- The probability that the treatment works
- The size or importance of the effect

**The threshold trap:** p < 0.05 is an arbitrary convention, not a law of nature.
- A result can be statistically significant (p = 0.03) and clinically meaningless (ARR = 0.01%)
- A result can be non-significant (p = 0.08) and clinically important — with a small sample that was underpowered to detect the real effect

**What to weigh instead:** Effect size + confidence intervals, interpreted in clinical context.

---

## Confidence Intervals (CI)

A 95% CI is the range within which the true effect most plausibly falls.

**Example:** "Hazard ratio 0.80 (95% CI: 0.65–0.98)"
- Best estimate: 20% relative reduction in the outcome
- Plausible range: 2% to 35% relative reduction
- The CI excludes 1.0 → statistically significant, but barely

**Red flags:**
- Wide CI (e.g., 0.3–2.1): huge uncertainty; the true effect could be benefit, harm, or nothing
- CI that barely excludes 1.0: technically significant but fragile — a slightly different study might not replicate

**Rule:** A narrow CI near a meaningful effect size is more compelling than a wide CI that happens to exclude the null.

---

## Surrogate Endpoints vs. Clinical Endpoints

**Surrogate:** A measurable marker assumed to predict outcomes (tumor shrinkage, LDL level, HbA1c, blood pressure)

**Clinical:** What actually matters to patients (survived 5 years, didn't have a stroke, quality of life improved, avoided hospitalization)

**The trap:** A drug can improve a surrogate without improving clinical outcomes — and some drugs have been approved on surrogates and later found harmful.

**Ask every time:** "Does this study measure what patients actually experience, or a lab marker assumed to represent that?"

---

## Correlation vs. Causation

Observational studies track people with different exposures. They cannot randomly assign treatments. Confounding is always possible.

**Confounders:** Variables that correlate with both the exposure and the outcome, creating the illusion of a causal relationship.

**Classic example:** Coffee drinkers showed lower rates of Parkinson's disease in early observational studies. But coffee drinkers also tended to be non-smokers — and nicotine in tobacco actually reduces Parkinson's risk. Smoking was the confounder.

**Rule:** "Associated with" ≠ "causes." Only RCTs can establish causation. When you see observational data, ask: what could explain this association besides the proposed mechanism?

---

## Publication Bias

Positive results are published more frequently than null or negative results. This means:

- The published literature systematically overstates treatment benefits
- Meta-analyses inherit this bias unless they actively seek unpublished data
- "No published evidence of harm" can mean "no one published the null result"

**How to check:** Does the systematic review describe efforts to find unpublished or grey literature? Does it assess funnel plot asymmetry? Does it note a GRADE rating for the evidence quality?

---

## Absolute vs. Relative Risk: The Headline Test

When you see a health headline, run it through this quick filter:

1. **Is the reported number relative or absolute?** ("reduces risk by 40%" → relative until proven otherwise)
2. **What is the baseline rate?** (Find it in the study's control arm)
3. **Compute the ARR** (Control rate × relative reduction = absolute reduction)
4. **Compute the NNT** (1 / ARR)
5. **Is the effect clinically meaningful for this patient's baseline risk?**

Most dramatic headlines collapse at step 3.
