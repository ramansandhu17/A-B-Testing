# 🧪 A/B Test Summary: Checkout Page Redesign

## Objective

The goal of this analysis was to evaluate whether a new checkout page design had any effect on user conversion rates. We used a standard A/B testing approach and followed it up with causal inference using Propensity Score Matching to dig deeper.

---

## Dataset

- Source: Kaggle A/B Testing Dataset
- Files used: `ab_data.csv` and `countries.csv`
- Key variables: `user_id`, `group`, `landing_page`, `converted`, and `country`

---

## Initial A/B Test Results

After filtering out users who were assigned to the wrong page (e.g. treatment group seeing old page), we compared conversion rates between the two groups:

- Control group (old checkout page): 12.04%
- Treatment group (new checkout page): 11.88%
- Difference (ATE): -0.16 percentage points
- p-value from z-test: 0.2156

**Interpretation**:  
At this stage, the difference between the groups was very small and not statistically significant. It looked like the new design had no real impact.

---

## Going Deeper with Causal Inference (Propensity Score Matching)

We wanted to check whether user **country** was affecting the assignment to treatment/control and also possibly influencing conversion.

To control for that, we used **Propensity Score Matching**:
- We estimated the probability (propensity score) of being in the treatment group based on country.
- Then we matched each user in the treatment group with a user in the control group with a similar propensity score.
- This gave us more comparable groups — users with similar likelihoods
