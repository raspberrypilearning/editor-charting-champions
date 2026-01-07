<h2 class="c-project-heading--task">Population data</h2>
--- task ---
Compare with population data in another CSV file
--- /task ---

### Population sizes
Why might they have the most medals?

Look at the population of nations to see if there is any sort of pattern.

In the file tab open `pop.csv`. Because the data in `pop.csv` is also made up of a text string and a number, you can re-use your code with only small changes.

Change the chart title, the `width` of the chart, the file you are opening, and the category name to draw a chart based on the population data in `pop.csv`.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 3 
line_highlights: 4, 6, 12, 13
---
# Create a chart
chart = Bar(title='Population', width='600')

# Add data to the chart
with open('pop.csv') as f:
    for line in f:
        #print(line)
        pieces = line.split(',')
        #print(pieces)
        team = pieces[0]
        population = pieces[1]
        chart.add(team, int(population))  # Make population a number
--- /code ---

**Test:** run your program and look at the chart it draws. 

Hover the mouse over the biggest bars and notice which countries they belong to. Click the names of the really big ones to remove them from the chart; that will let you get a closer look at the others. Do any of the countries with lots of people have a large number of medals?

<div class="c-project-output">
![A bar chart showing the populations of many nations. Information appears when the mouse hovers over a bar. Bars disappear as the names of nations are clicked.](images/pop.gif){:width="500px"}
</div>

