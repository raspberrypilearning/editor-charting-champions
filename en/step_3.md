<h2 class="c-project-heading--task">More data</h2>
--- task ---
Load more teams to your chart
--- /task ---

<h2 class="c-project-heading--explainer">Add new lists</h2>
Load two more teams by adding new lists and `chart.add()` calls.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 7 
line_highlights: 11-12, 17-18
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
</div class="c-project-code">

**Test:** Run your code to see the updated chart. Try clicking on the United States' name. Then watch the scale of the chart change.

<div class="c-project-output">
![A bar chart showing the medals won by the United States, Great Britain, France, Germany, and China. When the United States' name is clicked, the tallest bar vanishes from the chart, which resizes.](images/short_list_2.gif){:width="300px"}
</div>

<div class="c-project-callout c-project-callout--tip">

### Tip

BULLET POINT TIPS HERE (OPTIONAL)

</div>

<div class="c-project-callout c-project-callout--debug">

### Debugging

BULLET POINT DEBUG POINTS HERE (OPTIONAL)

</div>



**Debug**: If you see a message about an `IndexError`, your code is trying to get a value from a list index that doesn't exist (e.g. `fr[2]`). To fix this:
 - Check each of your `chart.add` lines to be sure you are only using `0` and `1` as indexes.
 - Check the lines where you created your lists. Make sure each list has two items, separated by a comma.


