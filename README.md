#Quantitative analysis of the pledged mortgage

## About the project

This project started from a personal question: if I already have money invested in the stock market and I want to buy an apartment, is it better to sell my investments to pay the down payment, or to use my portfolio as collateral and get a 100% pledged mortgage?

To answer that, I built a financial simulation model in Python that compares three different ways to finance a home purchase in Spain. All three models assume the same monthly budget so the comparison is fair:

- **Traditional model without investment:** The entire portfolio is sold to cover the down payment and purchase costs. Any leftover monthly savings go into a bank account at 0% interest.
- **Traditional model with DCA:** Same as above, but the monthly savings are invested in the stock market every month.
- **Pledged mortgage:** Nothing is sold. The savings remain invested as collateral for the loan. The mortgage covers 100% of the property price.

The analysis uses real historical data from the S&P 500 (1996-2020) downloaded from Yahoo Finance, interest rates from current Spanish banking offers (2026), and actual Spanish tax law (capital gains brackets). It also includes costs that many simplified models overlook: fund management fees (TER), mandatory mortgage life insurance, and home insurance.

The notebook includes a sensitivity analysis crossing different market returns with different interest rates, a Monte Carlo simulation with 1,000 random scenarios, and a comparison showing how the conclusion changes depending on the property price. This last point turned out to be the key finding: the pledged mortgage is only profitable when the initial savings are large enough relative to the price of the property.

The full report in PDF (compiled with LaTeX) covers every section of the analysis with detailed explanations, charts, and tables.
## Author

Carlos Fernandez Fernandez -- BSc in Data Science and Engineering.
