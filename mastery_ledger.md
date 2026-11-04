# Statistics Mastery Lab — assessment ledger

Updated: 2026-10-27 (America/Toronto)

## Training target

Develop independent statistical fluency, rigorous reasoning, and professional judgment for industry and research roles. Teach measure-theoretic probability to the depth needed to understand assumptions, conditioning, convergence, and statistical inference; do not make specialist probability theory a prerequisite for continuing the broader diagnostic.

## Rating convention

Each topic has separate fluency (F), rigour (R), and judgment (J) ratings on a 0–4 scale. U means insufficient independent evidence, not a score of zero. A 1 means fragmentary independent performance with a material gap. Work completed after instruction or hints is recorded as supported work and does not raise independent mastery.

## Current assessment status

Diagnostic Session 1 (probability foundations) began with one unassisted recall question on conditional expectation, then paused for Learning Mode on measure-theoretic probability. A fresh diagnostic question on the exact normal-mean confidence interval has now been completed with substantial prompting. An applied-design question on randomized assignment with outcome observation only among app openers was completed with support; the independent answer did not identify the estimand or selection issue, and the learner reported uncertainty after a challenge. The linear-model foundations screen was completed with prompts; asymptotic reasoning is next. No coding assessments have been administered. Existing notebooks are excluded as evidence.

| Topic | F | R | J | Confidence | Basis |
| --- | ---: | ---: | ---: | --- | --- |
| Measure-theoretic probability, overall | U | U | U | — | Learner reports unfamiliarity; broad domain not yet assessed. Foundational instruction needed. |
| Conditional expectation: definition and identities | 1 | U | 1 | Low | Independent answer gave an informal density-based definition, omitted existence/uniqueness, and asserted a false product identity from unconditional independence. Correctly recalled linearity and scaling, subject to missing integrability assumptions. |
| Conditional probability calculation | 1 | U | U | Low | In the Bernoulli counterexample, twice omitted part of the conditioning calculation; corrected after targeted prompts. |
| Normal-mean inference and confidence coverage | 1 | 1 | 1 | Low | Independently recalled the t-interval form and sample variance, but could not derive the pivot or exact coverage without substantial prompts; made errors in variance scaling, choice of critical value, and coverage probability. |
| Randomized experiment with selective outcome observation | U | U | 1 | Low | Correctly computed observed group sizes, but focused on a test of observed means and did not independently identify the all-user estimand or selection induced by observing only app openers. |
| Linear-model OLS foundations | 1 | 1 | 1 | Low | Independently began with simple-regression formulas and later stated unbiasedness; recalled the general OLS formula and derived positive definiteness and the general covariance only after prompts. Initially conflated convexity with uniqueness and imposed normal, spherical errors unnecessarily. |
| Other statistical topics | U | U | U | — | Not yet assessed. |

## Observed performance and learning evidence

- Independently recalled linearity and constant scaling of conditional expectation, but did not state the needed integrability conditions or almost-sure nature of the identities.
- Could not state the measure-theoretic definition of conditional expectation or independently construct a counterexample to the proposed conditional-product identity.
- After a Bernoulli/sum prompt, identified the event where the identity fails. Needed further prompts to normalize the conditional probability correctly.
- In Learning Mode, derived finite-partition conditional-expectation coefficients and parts of the verification with scaffolding; recognized that a zero-probability cell makes its coefficient undetermined and explains almost-sure uniqueness.
- Identified the Radon–Nikodym derivative of A ↦ E[X 1_A] relative to P on the full sigma-algebra after a direct prompt.
- Self-reported unfamiliarity with measure-theoretic probability and the Radon–Nikodym theorem. This is a training need, not an inference about ability in other statistical domains.

- In the normal-mean diagnostic, independently recalled the t-interval form, sample-variance formula, and an algebraic decomposition of total and residual sums of squares.
- Initially invoked the central limit theorem for an exact normal-sample result, misstated the standardized mean distribution, and miscomputed the variance of a sum. Corrected the mean and variance after prompts.
- Could not establish independence of sample mean and sample variance; the orthogonal-normal proof was taught. Initially inferred a chi-square difference from marginal laws alone.
- Initially used a normal critical value for an exact finite-sample t interval and misstated coverage as 0.05. After prompts, correctly derived the central t probability as 0.95.

- In the app-reminder case, correctly computed observed counts (3,000 reminder; 2,000 control), but proposed a one-sided pooled test before defining the target estimand. The proposed standard error omitted a square root, and the pooled standard deviation was described as t-distributed. After a challenge, the learner reported not knowing how to distinguish the all-user effect from the observed-user contrast.
- After the estimand and missing-outcome formula were explained, correctly computed illustrative all-user means of $7.20 and $10.00 and a difference of -$2.80. This was supported learning, not independent mastery.

- In the linear-model screen, began with scalar simple-regression formulas rather than the requested general matrix model. After a prompt, gave the OLS matrix formula; after another, identified positive definiteness of X^T X from full column rank. The first-order equation was supplied.
- Correctly stated unbiasedness. Initially gave the spherical-error covariance formula and imposed normality, although the stated model allowed general covariance Omega. After a prompt, gave the correct sandwich covariance expression. The need for normality was clarified by instruction, not established independently.

## Error log and follow-up

| Issue | Type | Evidence | Next independent check |
| --- | --- | --- | --- |
| Treated a conditional density as necessary for conditional expectation and argued existence from weights summing to one. | Conceptual; missing assumptions | Initial unassisted answer | Define conditional expectation on a new probability space and justify existence/uniqueness. |
| Assumed independence of X and Y implies E[XY|G] = E[X|G]E[Y|G] for arbitrary G. | Conceptual | Initial unassisted answer | Analyze a new conditioning structure and state sufficient conditions for the identity. |
| Confused a joint probability with a conditional probability; later dropped part of an intersection. | Conditional-probability calculation | Bernoulli/sum example | Solve a fresh conditional-probability problem without prompts. |
| Indexed a finite-partition conditional expectation by all sigma-algebra events rather than its disjoint atoms. | Conceptual; proof structure | Supported learning exercise | Derive a fresh partition conditional expectation independently. |
| Used asymptotic normal reasoning for an exact normal-sample result and initially applied variance scaling incorrectly. | Conceptual; algebraic | Normal-mean diagnostic | Derive sampling distributions and variances in a new model without prompts. |
| Inferred the law of a difference of chi-square variables from their marginal laws without establishing joint structure. | Incomplete proof; missing independence | Normal-mean diagnostic | Justify a new pivot from its joint distribution or state a precise theorem with assumptions. |
| Used a normal cutoff for an exact finite-sample t interval and confused 95% coverage with 5% noncoverage. | Conceptual; probability calculation | Normal-mean diagnostic | Analyze a fresh interval, define quantiles precisely, and compute coverage. |
| Tested observed means without first defining the all-user causal estimand or addressing outcome observation determined after randomization. | Applied judgment; missing-data assumption | App-reminder diagnostic | In a fresh scenario, distinguish the target population effect from the observed-data contrast and assess identification. |
| Proposed an incompletely specified pooled test with an incorrect standard error and distributional statement. | Algebraic; missing assumptions | App-reminder diagnostic | If a test is warranted, state its estimand, assumptions, statistic, and reference distribution precisely. |
| Used ordinary convexity as a uniqueness argument without showing strict convexity or positive definiteness. | Incomplete proof | Linear-model diagnostic | Derive uniqueness in a new optimization problem and distinguish convexity from strict convexity. |
| Replaced general Omega by sigma^2 I and added normality when computing OLS covariance. | Missing assumptions; model interpretation | Linear-model diagnostic | Derive estimator moments under a new nonspherical covariance structure and identify exactly when normality is needed. |

## Training implication

After the diagnostic, include a focused measure-theoretic probability sequence: sigma-algebras and measurable random variables; Lebesgue expectation and L1; conditional expectation and the meaning of Radon–Nikodym; convergence theorems; and the assumptions behind statistical asymptotics. Assess these through statistical examples. Deeper specialist topics should be added only when they serve the learner's research or demonstrated needs. Also prioritize variance calculations, exact versus asymptotic sampling distributions, t pivots, and confidence-interval coverage in statistical examples. Include applied training on estimands, post-randomization selection, missing outcomes, and whether an observed-data analysis identifies a decision-relevant effect. Include linear-model geometry, assumptions behind unbiasedness and covariance, and exact versus moment-based inference. Revisit the listed gaps with new, unassisted problems; taught examples do not count as mastery evidence.
