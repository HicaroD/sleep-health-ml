# Sleep Health

How much caffeine do you need to take to affect your sleep?

## Overview

This project aims to identify the amount of caffeine (in mg) necessary to
affect sleep quality. By analyzing a dataset containing information about
sleep, we can understand the relationship between caffeine intake and sleep
quality.

The dataset used in this project includes variables, such as Sleep quality
scores, Heart rate variability, Sleep movements, Caffeine intake in mg and
more. For more information about the dataset, you can find on Kaggle
[here](https://www.kaggle.com/datasets/uom190346a/sleep-and-health-metrics).

## Methodology

To analyze the data, I employed a correlation matrix to determine the
relationships between the variables. The analysis revealed a strong correlation
of 72% between caffeine intake (in mg) and sleep quality.

Based on these findings, I trained a machine learning model using
`scikit-learn`, more specifically I used the Gradient Boosting Regressor
algorithm, which demonstrated the best accuracy among the models evaluated. The
accuracy was assessed using the `LazyPredict` package.

## Steps

1. Data Preprocessing: Clean and prepare the dataset for analysis.
2. Correlation Analysis: Utilize a correlation matrix to identify relationships
   between variables.
3. Model Training: Train the Gradient Boosting Regressor model.
4. Predictions: Use the trained model to predict sleep quality scores based on
   caffeine intake.
5. Threshold Definition: Define a minimum sleep quality score necessary for
   ideal sleep and identify the appropriate caffeine intake to maintain sleep
   quality.

## Results

| Caffeine Intake (mg) | Sleep Quality Score (0 to 10) |
| -------------------- | ----------------------------- |
| 50                   | 6.11                          |
| 100                  | 1.17                          |
| 200                  | 1.00                          |
| 300                  | 1.00                          |

And, lastly, to maintain a sleep quality score of 7 or higher, limit caffeine
intake to 35 mg or less.

## License

This project is licensed under the MIT License. See [LICENSE](./LICENSE).
