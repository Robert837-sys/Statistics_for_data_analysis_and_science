# Statistics for Data Analysis and Science

A hands-on Jupyter notebook that walks through the core statistics used in data analysis, with every concept paired with Python code. It goes from descriptive statistics all the way to confidence intervals and hypothesis testing.

## What's Covered

| # | Topic | What you'll learn |
|---|-------|-------------------|
| 1 | **Introduction** | Population vs sample, representative samples, descriptive vs inferential statistics |
| 2 | **Measures of center** | Mean, median and mode |
| 3 | **Variation** | Range, quartiles, percentiles, interquartile range, standard deviation (population and sample) |
| 4 | **Statistical inference** | Using a sample to draw conclusions about a population |
| 5 | **Normal distribution** | Properties of the bell curve, generating and plotting normal data |
| 6 | **Standard normal (Z) distribution** | Z-values, `cdf()` and `ppf()`, p-values |
| 7 | **Student's t-distribution** | Small-sample uncertainty, degrees of freedom |
| 8 | **Estimation** | Point estimates, confidence intervals, confidence levels, margin of error |
| 9 | **Confidence interval for a proportion** | Worked example: 6 occurrences in a sample of 30 gives [0.057, 0.343] at 95% |
| 10 | **Confidence interval for a mean** | Worked example: sample of 30 with mean 62.1 gives [57.07, 67.13] at 95% |
| 11 | **Hypothesis testing** | Null vs alternative hypothesis, significance level, critical value and p-value approaches |
| 12 | **Testing a proportion** | Worked example: more than 20% of Nobel winners US-born (p-value 0.2145, claim not supported) |
| 13 | **Testing a mean** | Worked example: average age of Nobel winners above 55 (t = 2.889, p-value 0.0036, claim supported at 1%) |
| 14 | **Revision** | Plot comparing the t-distribution at different degrees of freedom with the standard normal curve |

## Key Python Snippets

```python
from scipy import stats

stats.norm.cdf(3)        # value -> probability (Z = 3 gives 0.9987)
stats.norm.ppf(0.9)      # probability -> value (90th percentile gives Z = 1.28)
stats.t.ppf(0.75, 29)    # t-value with 29 degrees of freedom
stats.norm.ppf(1 - 0.025)  # critical z-value for a 95% confidence interval (1.96)
```

`cdf()` turns a value into a probability, and `ppf()` turns a probability back into a value.

## The Five Steps of a Hypothesis Test

1. Check the conditions
2. Define the claims (null and alternative hypotheses)
3. Decide the significance level
4. Calculate the test statistic
5. Conclude, using either the critical value approach or the p-value approach

## Tools and Libraries

- Python 3
- [NumPy](https://numpy.org/)
- [pandas](https://pandas.pydata.org/)
- [SciPy](https://scipy.org/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)
- Jupyter Notebook / JupyterLab

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/Robert837-sys/Statistics_for_data_analysis_and_science.git
   cd Statistics_for_data_analysis_and_science
   ```

2. Install the dependencies:

   ```bash
   pip install numpy pandas scipy matplotlib seaborn jupyter
   ```

3. Launch the notebook:

   ```bash
   jupyter notebook stats.ipynb
   ```

## Repository Structure

```
.
├── stats.ipynb   # The full tutorial notebook
├── images/       # Diagrams and illustrations used in the notebook
└── README.md
```

## Who This Is For

Anyone starting out in data analytics or data science who wants to understand the statistics behind the tools, not just run the code.

## Author

**Robert Owuor Agie**
Final-year Computer Science student (Data Analytics), University of Eldoret, Kenya

GitHub: [Robert837-sys](https://github.com/Robert837-sys)
