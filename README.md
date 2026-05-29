# 🎯 A/B Testing Framework

> *"Most teams stop at p-values. ."*

A production-grade experimentation framework applied to a 294K-user A/B test — 


---

##  What Makes This Different

Most A/B test notebooks on Kaggle run one z-test and call it done.  
This project runs **5 layers of analysis** — the same way a real DS team would 
before making a $1M+ shipping decision.

| Section | Method | Why It Matters |
|--------|---------|----------------|
| 0 | Data Quality Audit + SRM Check | Garbage in = garbage out |
| 1 | Frequentist Z-Test + Power Analysis | The baseline every team runs |
| 2 | Bayesian A/B Test | Probability treatment wins — more intuitive for stakeholders |
| 3 | Novelty Effect Detection | Did the new page only win early? False wins kill products |
| 4 | CUPED Variance Reduction | Netflix's secret weapon — 62.9% variance reduction achieved |
| 5 | Executive Business Memo | Should we ship? Dollar impact framing, not just p-values |

---

## Key Results

| Metric | Value |
|--------|-------|
| Dataset size | 294,478 users |
| Control conversion | 12.04% |
| Treatment conversion | 11.88% |
| Lift | -1.31% |
| P-value | 0.1899 (not significant) |
| P(Treatment wins) — Bayesian | **9.4%** |
| Novelty effect detected |  No — result is stable |
| CUPED variance reduction | **62.9%** |
| CI width reduction | **39.2%** |
| **Final decision** | ** Do not ship the new page** |

---

##  Business Impact

Assuming 1M MAU at current conversion rate:
- Shipping the new page = **~$945K annualized revenue risk**
- CUPED confirms we had sufficient power — null result is real, not noise

---

##  Methods Used

- Z-test for proportions
- Beta-Binomial Bayesian inference (Monte Carlo, 100K samples)
- Temporal novelty effect analysis via daily conversion trends
- CUPED (Controlled-experiment Using Pre-Experiment Covariates)
- Sample Ratio Mismatch (SRM) detection


---

---

