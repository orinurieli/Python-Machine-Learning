# Python Machine Learning

The project focuses on computational learning with Python, analyzing large amounts of data and working with the Pandas and Numpy libraries. 
# Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pandas and numpy.

```bash
pip install pandas
```
```bash
pip install numpy
```

## Initiate

```python
import pandas as pd
import matplotlib.pyplot as plt
plt.rcParams.update({'font.size': 20, 'figure.figsize': (8, 4)})

%matplotlib inline
import matplotlib_inline
matplotlib_inline.backend_inline.set_matplotlib_formats('svg')

import seaborn as sns
sns.set()
```

## Code Example

```python

# plot a line chart of total sales ('Total') per hour in our dataset
# the x axis will be an hour (e.g., 9, 10, 11), and the y axis will be the total amout of sales during that hour

# Get Hour for each row
df["Time"] = pd.to_datetime(df["Time"]).dt.hour

result = df_filtered.groupby("Time")["Total"].sum()

# Plot the data as a line chart
result.plot()

# Add a title and axis labels
plt.title("Total sales per Hour")
plt.xlabel("Hour")
plt.ylabel("Total sales")

# Show the plot
plt.show()
```


## Main Goals

- Interfacing with Python Libararies
- Working with big Datasets
- Analyze and draw conclusions according to given data
## License

[MIT](https://choosealicense.com/licenses/mit/)
