<h2 class="c-project-heading--task">Load CSV into chart</h2>
--- task ---
Use `int()` to **cast** a string to a number and load into a chart
--- /task ---

Load your data into the chart as part of your `for` loop. `team` is a string so can be used as a label on the chart. `medal` is currently a string, but needs to be converted to a number. You can use the `int()` function to **cast** a string to a number.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 9 
line_highlights: 14-16
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



--- task ---

**Test:** Run your code and look at the chart it creates. Try hovering over some of the bars, or clicking on the names of teams to add and remove them from the chart.

![A bar chart showing the medal counts of many nations. Information appears when the mouse hovers over a bar. Bars disappear as the names of nations are clicked.](images/adjust_chart.gif){:width="400px"}

**Debug:** If your chart is empty, check that you have `int(medals)` in your `chart.add()`.

**Debug:** If you see a message about an `IndexError`, your code is trying to get a value from a list index that doesn't exist (e.g. `pieces[2]`). To fix this:
 - Check each of your `team` and `medals` variables to be sure you are only using `0` and `1` as indexes.
 - Check the printed `pieces` lists to be sure they have two items: `['Tonga', '1\n']`, not `['Tonga,1\n']`. If they don't, then check that you have `','` in the `()` of `line.split()`.
 - Check you do not have a blank line at the bottom of your .csv file.

--- /task ---