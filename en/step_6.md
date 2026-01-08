<h2 class="c-project-heading--task">Split into lists</h2>
--- task ---
Use `split(',')` to make a new list item every time there is a comma
--- /task ---

Put a `#` in front of `print(line)`. This will turn that code into a comment, so Python will ignore it. 

Use `split()` to break up the CSV when there is a `,`. 

then store the first and second pieces in a new list. Then print those lists out.

--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 7 
line_highlights: 10-11
---
with open('medals.csv') as f:
    for line in f:
        #print(line)
        pieces = line.split(',') # Breaks the string into a list
        print(pieces) # Print each list
--- /code ---

**Run** your code and look at the text it prints out in the Text output tab. Each line should be a list with two items. 

<div class="c-project-output">
![Many lists, each with two items, printed out.](images/tally.png){:width="400px"}
</div>

<div class="c-project-callout c-project-callout--tip">

### Tip
You may notice that the second item has `\n` or `\r\n` at the end. This tells the computer it has reached the end of the line in a file.
</div>