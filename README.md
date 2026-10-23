# A/B Testing — Designing the Data-Generating Process

## Objective
I used randomized experiments and observational comparisons to measure treatment effects, identify selection bias, test statistical significance, and determine sample sizes for A/B tests.

## Methodology
- Loaded the LaLonde NSW job training experiment with 445 participants (185 trainees and 260 controls) and calculated the experimental average treatment effect (ATE) on earnings.
- Simulated an observational comparison group to demonstrate selection bias and decomposed the result using: Observational ATE = True ATE + Selection Bias.
- Ran a permutation test with 9,999 shuffles to test statistical significance and calculated a bootstrap BCa 95% confidence interval for the ATE.
- Conducted a power analysis to estimate the study's statistical power and the sample sizes needed to detect three different dollar effects.
- Applied the same testing methods to the Cookie Cats mobile game A/B test, comparing Day-1 retention for 90,189 players assigned to gates at levels 30 and 40.
- Wrote an `n_needed()` function, checked its results against the power analysis, and used it to calculate the sample size required for a Cookie Cats rerun.

## Key Findings
- **Job training effect:** Trainees earned $[YOUR VALUE] more than controls on average (permutation p-value = [YOUR VALUE]; 95% BCa confidence interval: $[YOUR VALUE] to $[YOUR VALUE]).
- **Selection bias:** The simulated observational comparison produced an ATE of $[YOUR VALUE], showing how differences in group composition can change the estimated treatment effect.
- **Cookie Cats A/B test:** The difference in Day-1 retention between the two gate placements was [YOUR VALUE] percentage points (p-value = [YOUR VALUE]).
- **Sample-size planning:** I estimated that a rerun of Cookie Cats would require [YOUR VALUE] players per group.

These results helped me understand why random assignment matters, how to distinguish treatment effects from selection bias, and how statistical power and sample size affect experimental design.
