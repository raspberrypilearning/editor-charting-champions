## Make a chart

Use Python to create and display a chart.

The starter project already has some code to import the `pygal` library, which you will use to draw your chart.

```python filename="main.py" line_numbers="true" line_number_start="1" line_highlights="1"

from pygal import Bar

```

## Step 1

Add a title for your chart below the `# Create a chart` comment.

```python filename="main.py" line_numbers="true" line_number_start="3" line_highlights="4"
# Create a chart
chart = Bar(title='Olympic medals')
```

## Step 2

Call `chart.render()` to display the chart.

```python filename="main.py" line_numbers="true" line_number_start="10" line_highlights="11"
# Display the chart
chart.render()
```

## Now run your code

Run your code to see the chart. It will be empty because it doesn't have data yet.

![The words 'Olympic medals' on a black background.](images/empty_chart.png){:width="300px"}

> [!DEBUG]
>
> If you see an error about `Bar()` or `chart.render()` being `not defined`:
>
>  - If the error is for `Bar()`, make sure it has an uppercase B at the start, and brackets at the end
>  - If the error is for `chart.render()`, check that it has the `.` between `chart` and `render`, as well as the brackets at the end
>
> If you are not using the Raspberry Pi code editor, and the graph hasn't appeared when you run your code, replace `chart.render()` with `chart.render_in_browser()`.
