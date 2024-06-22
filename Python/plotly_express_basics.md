# Plotly Express Basics Cheatsheet

## Introduction

Plotly Express is a high-level data visualization library built on top of Plotly. It provides a simple and intuitive interface for creating interactive plots and charts.

[Plotly Express Website](https://plotly.com/python/plotly-express/)

[Github Repo](https://github.com/plotly/plotly_express)

## Installation

To install Plotly Express, you can use pip:

```
pip install plotly_express
```

## Importing Plotly Express

To use Plotly Express in your Python code, you need to import it:

```python
import plotly_express as px
```

## Creating a Scatter Plot

To create a scatter plot using Plotly Express, you can use the `scatter` function:

```python
fig = px.scatter(data_frame, x='x_column', y='y_column')
fig.show()
```

## Creating a Bar Chart

To create a bar chart using Plotly Express, you can use the `bar` function:

```python
fig = px.bar(data_frame, x='x_column', y='y_column')
fig.show()
```

## Creating a Line Chart

To create a line chart using Plotly Express, you can use the `line` function:

```python
fig = px.line(data_frame, x='x_column', y='y_column')
fig.show()
```

## Conclusion

This cheatsheet provides a basic overview of Plotly Express and how to create different types of plots. For more advanced features and customization options, refer to the Plotly Express documentation.
