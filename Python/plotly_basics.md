# Plotly Basics Cheatsheet

Plotly is a powerful data visualization library for Python. It creates interacitve data visualizations.  Users should also reference the [plotly express cheatsheet](https://github.com/RaphCodec/MD_Cheatsheets/blob/main/Python/plotly_express_basics.md) as plotly express is now a port of this library.

[Plotly Website](https://plotly.com/python/)

[Plotly Github Repo](https://github.com/plotly/plotly.py)

## Installation

To install Plotly, you can use pip:

```bash
pip install plotly
```

## Importing Plotly

To use Plotly in your Python script, you need to import the `plotly.graph_objects` module:

```python
import plotly.graph_objects as go
```

## Creating a Basic Plot

To create a basic plot with Plotly, you need to define the data and layout. Here's an example:

```python
import plotly.graph_objects as go

# Define the data
x = [1, 2, 3, 4, 5]
y = [10, 8, 6, 4, 2]

# Create a trace
trace = go.Scatter(x=x, y=y)

# Create the layout
layout = go.Layout(title='My Plot')

# Create the figure
fig = go.Figure(data=[trace], layout=layout)

# Show the plot
fig.show()
```

This will create a simple line plot with the given data.

## Customizing the Plot

Plotly provides a wide range of customization options to make your plots more informative and visually appealing. Here are a few examples:

- Changing the plot type: You can create different types of plots, such as scatter plots, bar charts, and pie charts, by using the appropriate trace type.

- Adding titles and labels: You can add titles to the plot and axis labels to provide context to your data.

- Changing colors and markers: You can customize the colors and markers used in your plot to highlight different data points.

- Adding annotations: You can add annotations to specific data points or regions in your plot to provide additional information.

For more details on customizing your plots with Plotly, refer to the official documentation.

## Saving the Plot

To save your Plotly plot as an image or HTML file, you can use the `write_image` or `write_html` methods, respectively. Here's an example:

```python
fig.write_image("plot.png")  # Save as PNG image
fig.write_html("plot.html")  # Save as HTML file
```
