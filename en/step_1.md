
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
chart.render_in_browser()
--- /code ---
</div>

<h2 class="c-project-heading--explainer">Add some data</h2>

You can now add data to the chart.

Add the code below under the `# Add data to the chart` comment.
Then click the *Run* button.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 7 
line_highlights: 8-10
---
# Add data to the chart
us = ['United States', 2399]
gb = ['Great Britain', 1304]
fr = ['France', 751]
--- /code ---
</div>


<div class="c-project-output">
![A bar chart showing the medals won by the United States, Russia, and Great Britain.](images/short_list.png){:width="300px"}
</div>

<div class="c-project-callout c-project-callout--tip">

### Tip

BULLET POINT TIPS HERE (OPTIONAL)

</div>

<div class="c-project-callout c-project-callout--debug">

### Debugging

BULLET POINT DEBUG POINTS HERE (OPTIONAL)

</div>

