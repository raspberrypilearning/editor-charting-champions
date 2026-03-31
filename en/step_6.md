<h2 class="c-project-heading--task">Load CSV into chart</h2>
### Step 1

Use `int()` to convert a string to a number and load it into a chart

Load your data into the chart as part of your `for` loop. `team` is a string, so it can be used as a label on the chart. `medals` is currently a string, but it needs to be converted to a number. You can use `int()` to do this.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 7
line_highlights: 12-14
---
with open('medals.csv') as f:
    for line in f:
        #print(line)
        pieces = line.split(',')
        #print(pieces)
        team = pieces[0]
        medals = pieces[1]
        chart.add(team, int(medals))  # Make medals a number
--- /code ---

**Tip:** You can now use `#` to turn `print(pieces)` into a comment too.

### Step 2

**Test:** Run your code and look at the chart it creates. Try hovering over some of the bars, or clicking on the names of teams to add and remove them from the chart.

<div class="c-project-output">
![A bar chart showing the medal counts of many nations. Information appears when the mouse hovers over a bar. Bars disappear as the names of nations are clicked.](images/adjust_chart.gif){:width="400px"}
</div>

<div class="c-project-callout c-project-callout--debug">

### Debugging

If your chart is empty, check that you have `int(medals)` in your `chart.add()`.

If you see a message about an `IndexError`, your code is trying to get a value from a list index that doesn't exist (e.g. `pieces[2]`). To fix this:
 - Check each of your `team` and `medals` variables to be sure you are only using `0` and `1` as indexes.
 - Check the printed `pieces` lists to be sure they have two items: `['Tonga', '1\n']`, not `['Tonga,1\n']`. If they don't, then check that you have `','` in the `()` of `line.split()`.
 - Check you do not have a blank line at the bottom of your .csv file.

</div>
