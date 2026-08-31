# Dungeness Crab Biomass Modeling

This was my final project for **MATH 440: Mathematical Modeling** at Christopher Newport University. I used a data set with 55 yearly observations of Dungeness crab cohort biomass and compared five discrete population models.

My goal was to see which model fit the data best.

![Comparison of the five models](figures/model_comparison.png)

## Models

I fit the following models:

1. Discrete logistic
2. Smith-Slatkin
3. Beverton-Holt
4. Ricker
5. Theta-Ricker

The parameters were estimated with `scipy.optimize.curve_fit`. I compared the fitted models using residuals, RSS, and corrected Akaike Information Criterion (AICc).

## Results

The Beverton-Holt model had the lowest AICc when the models were fit to the full data set. I then used it for a 12-step forecast with a bootstrap confidence interval.

I also included an 80/20 holdout comparison to see how the models behaved on the last part of the time series after fitting on the first part.

![Holdout comparison](figures/holdout_validation.png)

![Forecast](figures/forecast.png)

## Files

- `dungeness_crab_biomass_modeling.ipynb`: the full analysis
- `data/DS14.csv`: the biomass data
- `figures/`: plots used in the analysis
- `requirements.txt`: Python packages needed to run the notebook

## Tools

Python, NumPy, Pandas, SciPy, and Matplotlib

## Run the notebook

```bash
pip install -r requirements.txt
jupyter notebook dungeness_crab_biomass_modeling.ipynb
```

The notebook reads the data from `data/DS14.csv`.
