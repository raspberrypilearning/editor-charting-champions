
<h2 class="c-project-heading--task">Make a chart</h2>
--- task ---
Use Python to create and display a chart
--- /task ---

The starter project already has some code to import the `pygal` library, which you will use to draw your chart.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 1
---

from pygal import bar

--- /code ---

<h2 class="c-project-heading--explainer">Give the chart a name</h2>

Add a title for your chart below the `# Create a chart` comment.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 3
line_highlights: 4
---
# Create a chart
chart = Bar(title='Olympic medals')
--- /code ---
</div>

<h2 class="c-project-heading--explainer">Display the chart</h2>

Call `chart.render()` to display the chart.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 11 
line_highlights: 12
---
# Display the chart
chart.render()
--- /code ---
</div>

**Test:** Run your code to see the chart. It will be empty because it doesn't have data yet.

<div class="c-project-output">
![The words 'Olympic medals' on a black background.](images/empty_chart.png){:width="300px"}
</div>

<div class="c-project-callout c-project-callout--tip">

### Tip

BULLET POINT TIPS HERE (OPTIONAL)

</div>

<div class="c-project-callout c-project-callout--debug">

### Debugging

**Debug**: If you see an error about `Bar()` or `chart.render()` being `not defined`:

 - If the error is for `Bar()`, make sure it has an uppercase B at the start, and brackets at the end
 - If the error is for `chart.render()`, check that it has the `.` between `chart` and `render`, as well as the brackets at the end

**Debug**: If you are not using the Raspberry Pi code editor, and the graph hasn't appeared when you run your code, replace `chart.render()` with `chart.render_in_browser()`.

</div>


