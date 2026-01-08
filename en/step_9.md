<h2 class="c-project-heading--task">Challenge</h2>
--- task ---
Upgrade your project by changing how your chart looks, or what data it uses.
--- /task ---

<h2 class="c-project-heading--explainer">Pie chart</h2>
To create a pie chart instead of a bar chart, change the import from `pygal` to `Pie` instead of `Bar` and change the code in line for to `Pie`.


<h2 class="c-project-heading--explainer">Different data</h2>
Try loading and charting other data with the program you've written.

There are two other `.csv` files available in this project:

 - `mcu.csv` is the runtime and gross income from the Marvel Cinematic Universe films
 - `carbon.csv` is the total (thousands of tons) and per-person (tons) carbon dioxide emissions of different countries and regions


Change `medals.csv` in your code to your new file name.  

- These files have more than one column of numbers. Use indexes on the `tally` list to choose which to add to your chart. 
- The carbon dioxide data uses numbers with decimals. To convert them from text, you'll need to use `float()` instead of `int()`.
