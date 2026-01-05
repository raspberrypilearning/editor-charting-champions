
<h2 class="c-project-heading--task">Add data</h2>
--- task ---
Add some data to your chart.
--- /task ---

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



<h2 class="c-project-heading--explainer">Make lists</h2>

Use the indexes of your lists and `chart.add()` to display your data. The nation's name at item 0 will be used as a category label for the chart and the amount of medals at item 1 will determine the height of the bar.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 12 
line_highlights: 12-14
---
chart.add(us[0], us[1])
chart.add(gb[0], gb[1])
chart.add(fr[0], fr[1])
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

