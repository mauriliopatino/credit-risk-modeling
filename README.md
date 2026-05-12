# Credit Risk Modeling — A Practitioner's Series

**Maurilio Patiño García**

A series of technical notes and Python notebooks on credit portfolio risk, starting from the mathematical foundations of the Basel II IRB formula and building toward empirical calibration and extensions.

## Contents

|#|Topic|Format|Link|
|-|-|-|-|
|1|Why does the Basel II IRB formula work?|PDF|[ASRF\_Proof.pdf](ASRF_Proof.pdf)|
|2|Simulating credit portfolios: from VBA to vectorized Python|Notebook + PDF|[Notebook](Loss_Dist_MC_Convergence.ipynb) · [PDF](Loss_Dist_MC_Convergence.pdf)|
|3|VaR vs Expected Shortfall: the technical case|Notebook + PDF|[Notebook](VaR_vs_Expected_Shortfall.ipynb) · [PDF](VaR_vs_Expected_Shortfall.pdf)|
|4|The copula inside the Basel formula|Notebook + PDF|[Notebook](The_Copula_Inside_the_Basel_Formula.ipynb) · [PDF](The_Copula_Inside_the_Basel_Formula.pdf)|

## References

### Books

* C. Bluhm, L. Overbeck, Ch. Wagner. "An Introduction to Credit Risk Modelling". Chapman & Hall/CRC, 2003.
* G. Löffler, P. Posch. "Credit Risk Modeling using Excel and VBA". Wiley, 2nd ed.
* P. Glasserman. "Monte Carlo Methods in Financial Engineering". Springer, 2003.
* D. Rösch, H. Scheule. "Deep Credit Risk: Machine Learning with Python". 2020.
* A. J. McNeil, R. Frey, P. Embrechts. "Quantitative Risk Management: Concepts, Techniques and Tools". Princeton University Press, revised ed., 2015.

### Papers

* P. Artzner, F. Delbaen, J.-M. Eber, D. Heath. "Coherent Measures of Risk". Mathematical Finance, 9(3):203–228, 1999.
* C. Acerbi, D. Tasche. "On the Coherence of Expected Shortfall". Journal of Banking & Finance, 26(7):1487–1503, 2002.
* C. Acerbi. "Spectral Measures of Risk: A Coherent Representation of Subjective Risk Aversion". Journal of Banking & Finance, 26(7):1505–1518, 2002.
* M. B. Gordy. "A Risk-Factor Model Foundation for Ratings-Based Bank Capital Rules". Journal of Financial Intermediation, 12(3):199–232, 2003.
* O. Vasicek. "The Distribution of Loan Portfolio Value". Risk, 15(12):160–162, 2002.
* T. Gneiting. "Making and Evaluating Point Forecasts". Journal of the American Statistical Association, 106(494):746–762, 2011.
* S. Emmer, M. Kratz, D. Tasche. "What Is the Best Risk Measure in Practice? A Comparison of Standard Measures". Journal of Risk, 18(2):31–60, 2015.
* A. Hamerle, D. Rösch. "Misspecified Copulas in Credit Risk Models: How Good is Gaussian?". Journal of Risk, 8(1):41–58, 2005.
* D. Brigo, A. Pallavicini, R. Torresetti. "Credit Models and the Crisis: A Journey into CDOs, Copulas, Correlations and Dynamic Models". Wiley, 2010.

### Regulatory Documents

* Basel Committee on Banking Supervision. "An Explanatory Note on the Basel II IRB Risk Weight Functions". BIS, 2005.
* Basel Committee on Banking Supervision. "Minimum Capital Requirements for Market Risk". BIS, 2019.
* EIOPA. "The Underlying Assumptions in the Standard Formula for the Solvency Capital Requirement Calculation". 2014.
* Swiss Federal Office of Private Insurance. "Technical Document on the Swiss Solvency Test". FOPI, 2006.
* OSFI Canada. "Mortgage Insurer Capital Adequacy Test (MICAT) Guideline". 2025.

## License

This material is shared for educational purposes. The code is provided as-is with no warranty.
