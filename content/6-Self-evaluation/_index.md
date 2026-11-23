---
title: "Self-Assessment"
date: 2026-10-28
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

During the **First Cloud AI Journey (FCAJ)** program, I worked on **CPAWS, an AWS-based commodity forecasting system**, primarily in **Modeling & Evaluation**. My responsibilities extended beyond checking final model results: I contributed to problem formulation, forecasting experiments, evaluation design, and the verification of research evidence.

At an early stage, I **proposed using log returns as the forecasting target instead of predicting absolute price levels directly**. I also helped review the specification of forecasts over 1–7 trading sessions, the predictive quantiles, and the probability of a price increase, so that the outputs could be interpreted and evaluated consistently. These were contributions within my technical area, not a claim that I led the entire project or implemented every component.

As development progressed, I focused on analyzing forecasting experiments, implementing and testing evaluation metrics, contributing to **Rolling Accuracy**, reviewing technical documentation, and carrying out the **official test2020** evaluation. I shared ideas within my area of expertise while making an effort to complete the tasks assigned by the team leader.

### Self-Assessment

| No. | Criteria | Description | Good | Fair | Average |
|---|---|---|:---:|:---:|:---:|
| 1 | **Professional knowledge & skills** | Field knowledge, practical application, tools and work quality | ✅ | ☐ | ☐ |
| 2 | **Ability to learn** | Learning new concepts and conducting independent research | ✅ | ☐ | ☐ |
| 3 | **Proactiveness** | Exploring ideas and taking initiative within assigned responsibilities | ✅ | ☐ | ☐ |
| 4 | **Sense of responsibility** | Completing assigned work with attention to quality | ✅ | ☐ | ☐ |
| 5 | **Discipline** | Following schedules, rules and work processes | ☐ | ✅ | ☐ |
| 6 | **Progressive mindset** | Accepting feedback and improving continuously | ☐ | ✅ | ☐ |
| 7 | **Communication** | Exchanging ideas and explaining technical matters clearly | ☐ | ✅ | ☐ |
| 8 | **Teamwork** | Collaborating and supporting other team members | ✅ | ☐ | ☐ |
| 9 | **Professional conduct** | Respecting colleagues and maintaining professional behavior | ☐ | ✅ | ☐ |
| 10 | **Problem-solving skills** | Identifying issues, analyzing options and proposing solutions | ☐ | ✅ | ☐ |
| 11 | **Contribution to project/team** | Technical contributions and effectiveness of delivered work | ✅ | ☐ | ☐ |
| 12 | **Overall** | Overall assessment of the internship | ☐ | ✅ | ☐ |

### Strengths

**1. Problem Analysis and Forecast Output Definition**

I consider it important to define the forecasting target and evaluation criteria before selecting a model. In CPAWS, in addition to proposing log returns, I reviewed trading-session horizons, predictive quantiles, `prob_up`, and the validity requirements for price observations at the endpoints. I also contributed feedback on the API contract to help ensure consistency between model calculations, stored records, and displayed forecasts.

This experience showed me how the definition of a forecasting output influences model design, data validation, and the way users interpret the results.

**2. Forecasting Research, Experiments, and Model Comparisons**

I contributed to experiments, analysis, and technical reviews using the **2019 validation period**. My work involved **DLinear**, **CEEMDAN–DLinear (K3)**, and volatility-based approaches such as **K3b/S1a**. I focused on comparing these methods against `baseline-q252`, examining their performance across assets and forecast horizons rather than assuming that a more complex model must perform better.

One important lesson was that an alternative model should not replace the baseline without sufficient evidence. The team therefore retained `baseline-q252` as champion while **S1a** remained a **shadow** challenger for further evaluation.

**3. Evaluation Methodology and Metric Testing**

I spent a significant part of my time on evaluation. I contributed to implementing and testing evaluation metrics, with **pinball skill** against the 252-session quantile baseline as the primary metric. Secondary measures helped assess return errors, prediction-interval coverage and width, and the quality of upward-movement probabilities.

I also worked on time-based evaluation rules, `valid mask` checks, consistent samples for model comparisons, and avoiding future-information leakage. Reviewing the schema for **validation, test, and rolling_8w** helped me understand how to make results traceable and suitable for their intended use.

**4. Rolling Accuracy Design and Review**

For **Rolling Accuracy**, I contributed to the evaluation specification and its core logic: a 56-day window, matching published forecasts with realized prices by `base_date` and `target_date`, **eligibility** requirements, data **provenance**, and handling missing forecasts or upstream failures.

I also reviewed the data contract supporting `/accuracy/{asset}`, checking consistency across job states, stored results, and API responses. This taught me that a successfully completed job does not necessarily mean that enough valid observations are available to publish an accuracy metric.

**5. Reproducible Evaluation and Result Verification**

I reviewed the **test2020** plan and runner, including valid-sample selection, statistical testing, bootstrap confidence intervals, and multiple-testing adjustments. On **November 16, 2026**, I personally executed the **single official test2020 run** using a frozen configuration and dataset, then audited its artifacts and verified **all seven SHA-256 checksums**.

In reporting the findings, I distinguished statistically supported results from cases where the evidence was insufficient, and documented the limitations of the data and methodology. The official test was intended for evaluation and reporting, not for retuning the models or automatically promoting a new champion.

**6. Responsibility, Independent Learning, and Teamwork**

I am relatively outgoing and comfortable contributing ideas during discussions related to Modeling & Evaluation. Beyond research, I reviewed pull requests, provided feedback on the **Proposal, ADRs, and API contract**, and helped align technical documentation with the evaluation results.

I made an effort to complete the tasks assigned by the team leader and independently study unfamiliar technical topics. Working with teammates responsible for data, APIs, and infrastructure improved my understanding of how decisions in one component affect the rest of a system.

### Areas for Improvement

**1. Explaining Complex Technical Issues**

Although I communicate proactively, I sometimes include too many conditions and technical details in a single explanation, making the main point harder to follow. I would like to communicate more clearly by structuring discussions around the **problem, evidence, proposed solution, and conclusion**.

**2. Managing Time Across Multiple Responsibilities**

At certain stages, I had to balance forecasting research, technical reviews, AWS labs, university coursework, and reporting. I would like to improve my prioritization, divide large assignments into smaller milestones, and allow more time for unexpected issues.

### Overall Reflection

I rate my **overall performance as Fair**. I am satisfied that I contributed across several stages of CPAWS, from defining forecasting outputs and comparing models to evaluation design, Rolling Accuracy, and the official test2020 verification. At the same time, I learned that trustworthy results require valid data, reproducible procedures, and conclusions that do not go beyond the evidence.

FCAJ also reinforced the importance of personal responsibility and teamwork in a multi-component AI system. I hope to improve my technical communication and time management as I pursue further research in **AI and Robotic AI**.
