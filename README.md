# Credit Risk Modeling: A Practitioner's Series

**Maurilio Patiño García**

A series of technical notes and Python notebooks on credit risk, starting from the mathematical foundations of the Basel II IRB formula and building toward the full modeling toolkit: PD and LGD estimation, transition matrices, survival analysis, credit scoring, and empirical calibration with loan-level data.

## Contents

| # | Topic | Format | Link |
|---|-------|--------|------|
| 1 | Why does the Basel II IRB formula work? | PDF | [ASRF_Proof.pdf](ASRF_Proof.pdf) |
| 2 | Simulating credit portfolios: from VBA to vectorized Python | Notebook + PDF | [Notebook](Loss_Dist_MC_Convergence.ipynb) · [PDF](Loss_Dist_MC_Convergence.pdf) |
| 3 | VaR vs Expected Shortfall: the technical case | Notebook + PDF | [Notebook](VaR_vs_Expected_Shortfall.ipynb) · [PDF](VaR_vs_Expected_Shortfall.pdf) |
| 4 | The copula inside the Basel formula | Notebook + PDF | [Notebook](The_Copula_Inside_the_Basel_Formula.ipynb) · [PDF](The_Copula_Inside_the_Basel_Formula.pdf) |
| 5 | Why does Basel survive heavy tails? | Notebook + PDF | [Notebook](Misspecified_Copulas_in_Credit_Risk.ipynb) · [PDF](Why%20Basel%20Survives%20Heavy%20Tails.pdf) |
| 6 | If you need a PD, don't rebalance | Notebook + PDF | [Notebook](If_You_Need_a_PD_Dont_Rebalance.ipynb) · [PDF](If_You_Need_a_PD_Dont_Rebalance.pdf) |

Data for note 6: Kaggle, "Give Me Some Credit" (2011), https://www.kaggle.com/c/GiveMeSomeCredit. The notebook reads a local copy of `cs-training.csv` if there is one, otherwise downloads an identical public copy, and in both cases verifies its SHA-256 hash.

## In preparation

In the order planned:

1. Calibration by segment: right on average, wrong by segment.
2. Bayesian estimation of PD for segments with few defaults.
3. Weight of evidence: when it helps and when it gets in the way.
4. Non-linearity and interactions in credit scoring.
5. Scorecards without starting from a logistic regression.
6. Recalibration with few defaults.
7. PD over time: validation by vintage, survival analysis (Cox), lifetime PD with competing risks, and point-in-time versus through-the-cycle PD.
8. LGD estimation: workout approach, censoring, and downturn LGD.
9. Empirical PD-LGD co-movement with agency loan-level data.
10. Calibration of the Basel asset correlation with agency loan-level data.
11. Transition and generator matrices for credit portfolios: estimation, embeddability, and applications.

## References

### Books

- C. Bluhm, L. Overbeck, Ch. Wagner. "An Introduction to Credit Risk Modelling". Chapman & Hall/CRC, 2003.
- G. Löffler, P. Posch. "Credit Risk Modeling using Excel and VBA". Wiley, 2nd ed.
- P. Glasserman. "Monte Carlo Methods in Financial Engineering". Springer, 2003.
- R. B. Nelsen. "An Introduction to Copulas". Springer, 2nd ed., 2006.
- D. Rösch, H. Scheule. "Deep Credit Risk: Machine Learning with Python". 2020.
- A. J. McNeil, R. Frey, P. Embrechts. "Quantitative Risk Management: Concepts, Techniques and Tools". Princeton University Press, revised ed., 2015.

### Papers

- A. Sklar. "Fonctions de répartition à n dimensions et leurs marges". Publications de l'Institut de Statistique de l'Université de Paris, 8:229–231, 1959.
- M. Sibuya. "Bivariate Extreme Statistics". Annals of the Institute of Statistical Mathematics, 11(2):195–210, 1960.
- A. J. McNeil, R. Frey, M. A. Nyfeler. "Copulas and Credit Models". Risk, 14(10):111–114, 2001.
- P. Artzner, F. Delbaen, J.-M. Eber, D. Heath. "Coherent Measures of Risk". Mathematical Finance, 9(3):203–228, 1999.
- D. X. Li. "On Default Correlation: A Copula Function Approach". Journal of Fixed Income, 9(4):43–54, 2000.
- P. Embrechts, A. J. McNeil, D. Straumann. "Correlation and Dependence in Risk Management: Properties and Pitfalls". Risk Management: Value at Risk and Beyond, pages 176–223, 2002.
- C. Acerbi, D. Tasche. "On the Coherence of Expected Shortfall". Journal of Banking & Finance, 26(7):1487–1503, 2002.
- C. Acerbi. "Spectral Measures of Risk: A Coherent Representation of Subjective Risk Aversion". Journal of Banking & Finance, 26(7):1505–1518, 2002.
- O. Vasicek. "The Distribution of Loan Portfolio Value". Risk, 15(12):160–162, 2002.
- M. B. Gordy. "A Risk-Factor Model Foundation for Ratings-Based Bank Capital Rules". Journal of Financial Intermediation, 12(3):199–232, 2003.
- A. Hamerle, D. Rösch. "Misspecified Copulas in Credit Risk Models: How Good is Gaussian?". Journal of Risk, 8(1):41–58, 2005.
- D. Brigo, A. Pallavicini, R. Torresetti. "Credit Models and the Crisis: A Journey into CDOs, Copulas, Correlations and Dynamic Models". Wiley, 2010.
- T. Gneiting, A. E. Raftery. "Strictly Proper Scoring Rules, Prediction, and Estimation". Journal of the American Statistical Association, 102(477):359–378, 2007.
- T. Gneiting. "Making and Evaluating Point Forecasts". Journal of the American Statistical Association, 106(494):746–762, 2011.
- S. Emmer, M. Kratz, D. Tasche. "What Is the Best Risk Measure in Practice? A Comparison of Standard Measures". Journal of Risk, 18(2):31–60, 2015.

### Papers: credit scoring and classification

- G. W. Brier. "Verification of Forecasts Expressed in Terms of Probability". Monthly Weather Review, 78(1):1–3, 1950.
- J. A. Hanley, B. J. McNeil. "The Meaning and Use of the Area under a Receiver Operating Characteristic (ROC) Curve". Radiology, 143(1):29–36, 1982.
- R. Kerber. "ChiMerge: Discretization of Numeric Attributes". Proceedings of AAAI-92, 1992.
- J. C. Platt. "Probabilistic Outputs for Support Vector Machines and Comparisons to Regularized Likelihood Methods". Advances in Large Margin Classifiers, MIT Press, pages 61–74, 1999.
- C. Elkan. "The Foundations of Cost-Sensitive Learning". Proceedings of IJCAI-01, pages 973–978, 2001.
- G. King, L. Zeng. "Logistic Regression in Rare Events Data". Political Analysis, 9(2):137–163, 2001.
- N. V. Chawla, K. W. Bowyer, L. O. Hall, W. P. Kegelmeyer. "SMOTE: Synthetic Minority Over-sampling Technique". Journal of Artificial Intelligence Research, 16:321–357, 2002.
- B. Zadrozny, C. Elkan. "Transforming Classifier Scores into Accurate Multiclass Probability Estimates". Proceedings of KDD 2002, pages 694–699, 2002.
- Z. C. Lipton, C. Elkan, B. Narayanaswamy. "Optimal Thresholding of Classifiers to Maximize F1 Measure". ECML PKDD 2014, LNCS 8725, Springer, 2014.
- G. Ke et al. "LightGBM: A Highly Efficient Gradient Boosting Decision Tree". Advances in Neural Information Processing Systems 30, 2017.
- R. van den Goorbergh, M. van Smeden, D. Timmerman, B. Van Calster. "The Harm of Class Imbalance Corrections for Risk Prediction Models: Illustration and Simulation Using Logistic Regression". Journal of the American Medical Informatics Association, 29(9):1525–1534, 2022.
- A. Carriero, K. Luijken, A. de Hond, K. G. M. Moons, B. Van Calster, M. van Smeden. "The Harms of Class Imbalance Corrections for Machine Learning Based Prediction Models: A Simulation Study". Statistics in Medicine, 2025.

### Regulatory Documents

- Basel Committee on Banking Supervision. "An Explanatory Note on the Basel II IRB Risk Weight Functions". BIS, 2005.
- Basel Committee on Banking Supervision. "Minimum Capital Requirements for Market Risk". BIS, 2019.
- EIOPA. "The Underlying Assumptions in the Standard Formula for the Solvency Capital Requirement Calculation". 2014.
- Swiss Federal Office of Private Insurance. "Technical Document on the Swiss Solvency Test". FOPI, 2006.
- OSFI Canada. "Mortgage Insurer Capital Adequacy Test (MICAT) Guideline". 2025.

## License

Code is released under the [MIT License](LICENSE). Technical notes (PDFs) are shared under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/): feel free to use them with attribution. All material is provided as-is, for educational purposes, with no warranty.
