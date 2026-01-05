<h2 class="c-project-heading--task">Add data</h2>
--- task ---
Add some data to your chart.
--- /task ---

<h2 class="c-project-heading--explainer">Add some data</h2>

Python can store related data as a **list**. You can create lists by using square brackets `[]`. Items in a list are separated with commas.

--- task ---

Create three lists of data to show on your chart.

Each list will store a nation's name and the number of medals won by that nation. 

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

When you store something in a list, it gets an **index**. An index is a number that tells you an item's position in a list. List indexes start from `0`, instead of `1`.

<h2 class="c-project-heading--explainer">Make lists</h2>

You can get an item from a list by its index. For example, `my_list[3]` will get the **fourth** item in `my_list`, because indexes start at `0`.

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


**Test:** Run your code to see the chart.

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


**Debug**: If you see a message about an `IndexError`, your code is trying to get a value from a list index that doesn't exist (e.g. `us[2]`). To fix this:
 - Check each of your `chart.add` lines to be sure you are only using `0` and `1` as indexes.
 - Check the lines where you created your lists. Make sure each list has two items, separated by a comma.