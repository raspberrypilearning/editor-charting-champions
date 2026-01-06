<h2 class="c-project-heading--task">More lists, more data</h2>
--- task ---
Practice adding more data in lists
--- /task ---

<h2 class="c-project-heading--explainer">Add new lists</h2>
Load two more nations by adding new data lists and using `chart.add()` for each one.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 6 
line_highlights: 10-11, 16-17
---
# Add data to the chart
us = ['United States', 2399]
gb = ['Great Britain', 1304]
fr = ['France', 751]
ge = ['Germany', 655]
ch = ['China', 636]

chart.add(us[0], us[1])
chart.add(gb[0], gb[1])
chart.add(fr[0], fr[1])
chart.add(ge[0], ge[1])
chart.add(ch[0], ch[1])

--- /code ---
</div>

**Run** your code to see the new bars of data in the chart. 

<div class="c-project-output">
![A bar chart showing the medals won by the United States, Great Britain, France, Germany, and China. When the United States' name is clicked, the tallest bar vanishes from the chart, which resizes.](images/short_list_2.gif){:width="300px"}
</div>

<div class="c-project-callout c-project-callout--tip">

### Tip

Try clicking on the United States' name. Then watch the scale of the chart change.

</div>



