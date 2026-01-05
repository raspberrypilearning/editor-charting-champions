
<h2 class="c-project-heading--task">Make a chart</h2>
--- task ---
Use Python to create and display a chart.
--- /task ---

<h2 class="c-project-heading--explainer">Give the chart a name</h2>

Add a title for your chart below the `# Create a chart` comment.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 4 
line_highlights: 5
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



<div class="c-project-output">
![The words 'Olympic medals' on a black background.](images/empty_chart.png){:width="300px"}
</div>

<div class="c-project-callout c-project-callout--tip">

### Tip

BULLET POINT TIPS HERE (OPTIONAL)

</div>

<div class="c-project-callout c-project-callout--debug">

### Debugging

BULLET POINT DEBUG POINTS HERE (OPTIONAL)

</div>

