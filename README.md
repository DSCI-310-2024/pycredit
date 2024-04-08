[![codecov](https://codecov.io/github/DSCI-310-2024/pycredit/graph/badge.svg?token=L68Uui9hpr)](https://codecov.io/github/DSCI-310-2024/pycredit)

# pycredit

DSCI310 Group 12's package for running data analyses around credit risk.

## Installation

```bash
$ pip install pycredit
```

## Usage

`pycredit` provides several useful functions for data preprocessing and analysis in understanding credit risk, such as, preprocess data, create histograms, transform labels, and create parameter grids for grid search.

```python
from pycredit import preprocess_data, column_histogram, map_labels_to_binary, param_grid_for_grid_search
import matplotlib.pyplot as plt

# Preprocess data
X_transformed, y, preprocessor = preprocess_data(df, numeric_features, categorical_features)

# Create histogram for a column
column_plot = column_histogram(fig_width, fig_height, data_frame, column_name)
plt.show()

# Transform label values
y_transformed = map_labels_to_binary(y)

# Create parameter grid for grid search
param_grid = param_grid_for_grid_search(n_estimators_range, max_depth_range)
```

## Contributing

Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.

## License

`pycredit` was created by Jade Bouchard, Shahrukh Islam Prithibi, Sophie Yang, Yovindu Don. It is licensed under the terms of the MIT license.

## Credits

`pycredit` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).
