# Thompson Sampling

This repository contains code for implementing Thompson Sampling, a technique used in multi-armed bandit problems, to optimize the click-through rate (CTR) for online advertisements. The code is written in Python & R and uses the pandas and matplotlib libraries.

## Code Explanation

The code performs the following steps:

1. Imports the required libraries: numpy, matplotlib, and pandas.
2. Reads the dataset from a CSV file named `Ads_CTR_Optimisation.csv`.
3. Initializes the parameters for the Thompson Sampling algorithm, including the number of rounds (`N`) and the number of advertisements (`d`).
4. Implements the Thompson Sampling algorithm by iterating over the specified number of rounds (`N`).
  - For each round, it selects an advertisement based on the maximum random value drawn from the beta distributions of each advertisement's rewards and failures.
  - The selected advertisement's reward (1 for click, 0 for no click) is observed from the dataset.
  - The reward counts for the selected advertisement are updated accordingly.
5. Visualizes the results using a histogram that shows the number of times each advertisement was selected.

## Dataset

The dataset used in this code is included in the repository and named `Ads_CTR_Optimisation.csv`. A portion of the dataset is shown below:

| Ad 1 | Ad 2 | Ad 3 | Ad 4 | Ad 5 | Ad 6 | Ad 7 | Ad 8 | Ad 9 | Ad 10 |
|------|------|------|------|------|------|------|------|------|-------|
| 1    | 0    | 0    | 1    | 0    | 0    | 0    | 1    | 0    | 0     |
| 0    | 0    | 0    | 0    | 0    | 0    | 0    | 1    | 0    | 0     |
| 0    | 0    | 0    | 0    | 0    | 0    | 0    | 0    | 0    | 0     |
| 0    | 1    | 0    | 0    | 0    | 0    | 1    | 0    | 0    | 0     |
| 0    | 0    | 0    | 0    | 0    | 0    | 0    | 0    | 0    | 0     |

Each column represents an advertisement, and each row represents a user visit. A value of 1 indicates that the user clicked on the corresponding advertisement, while a value of 0 indicates that the user did not click.

## Usage

To run the code, you need to have Python and the required libraries installed. You can install the necessary libraries using pip:
After installing the required libraries, you can run the code by executing the Python script.

## Contributing

Contributions to this repository are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
