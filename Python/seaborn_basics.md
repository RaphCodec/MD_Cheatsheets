# Seaborn Basics heatsheet

## Introduction
Seaborn is a python library, based on MatPlotLib and  used for creating data visualizations.

[Seaborn Offical Website](https://seaborn.pydata.org/)

[Seaborn Github Repo](https://github.com/mwaskom/seaborn)

## Installation
To install Seaborn, you can use pip:

```bash
pip install seaborn
```

## Importing Seaborn
Standard convention for importing seaborn:

```python
import seaborn as sns
```

## Loading Datasets
Seaborn comes with built-in datasets that you can load and use for visualization. Here's an example of loading the "tips" dataset:

```python
tips = sns.load_dataset("tips")
```

To see a list of available datasets use:
```python
sns.get_dataset_names()
```

## Plotting with Seaborn
Seaborn can be used to make all types of standard data visualizations. The aforementioned visuals can be created by doing the following.

### Scatter Plot
To create a scatter plot using Seaborn, you can use the `scatterplot()` function:

```python
sns.scatterplot(x="total_bill", y="tip", data=tips)
```

### Line Plot
To create a line plot using Seaborn, you can use the `lineplot()` function:

```python
sns.lineplot(x="day", y="total_bill", data=tips)
```

### Bar Plot
To create a bar plot using Seaborn, you can use the `barplot()` function:

```python
sns.barplot(x="day", y="total_bill", data=tips)
```

### Histogram
To create a histogram using Seaborn, you can use the `histplot()` function:

```python
sns.histplot(data=tips, x="total_bill")
```

### Box Plot
To create a box plot using Seaborn, you can use the `boxplot()` function:

```python
sns.boxplot(x="day", y="total_bill", data=tips)
```

## Customizing Plots
Seaborn provides various options to customize your plots. Here are some examples:

### Changing Color Palette
You can change the color palette of your plot using the `set_palette()` function:

```python
sns.set_palette("husl")
```

### Adding Titles and Labels
You can add titles and labels to your plot using the `title()`, `xlabel()`, and `ylabel()` functions:

```python
sns.lineplot(x="day", y="total_bill", data=tips)
sns.title("Total Bill by Day")
sns.xlabel("Day")
sns.ylabel("Total Bill")
```

### Changing Figure Size
You can change the figure size of your plot using the `figure()` function:

```python
sns.figure(figsize=(8, 6))
```

