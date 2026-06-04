Tyler Hann: First ai prompt

1. 
# Asked AI to teach me how to remove rows not needed.

Prompt:
    Hey Can you teach me how to remove empty rows/Give me the code in order for me to be able to remove full empty rows that makes the data Not applicable for further/later research. Do not write it for me i would just like to know the structure behind and what to do in order for this.

Response:
Example Structure using "df = df.dropna(how='all')" which is after first loading the excel file and then using dropna(how='all') will delete rows ONLY when the row is actually missing.

2. 
# Asked AI how to check data trends by making a graph using the raw cases of malaria and population per incidence

Prompt:
    Hey Can you teach me how to check if my data trends upwards exponentially when comparing total population against malaria cases? Give me the conceptual structure behind how to back-calculate absolute population sizes from percentage columns (like rural and urban population percentages) using raw case numbers and incidence rates, and how to structure a scatter plot with a connected trendline to visualize this growth over the years. Do not write the code for me, I would just like to know the logic and structure behind doing this in a VS Code Jupyter Notebook using pandas, seaborn, and matplotlib.
Response:
    Graph created using examples/given ideas of how to do it.

3. 
# Designing the Scatter Plot's Colors and Visual Style

Prompt:
    I want to know the logic behind styling this scatter plot. Can you teach me how to choose the right color palette, dot sizes, and layering order so that the visual design actually helps explain whether the trend is exponential or linear? Focus only on the styling mechanics and design choices.

Responses: 
The Color Scheme (palette='viridis'):  Instead of a mix of random colors, a single fading color path called viridis was chosen. It smoothly changes from a dark purple for the oldest years to a bright yellow for the newest years. Because your population grows over time, your eyes ca follow the colors like a timeline to see the direction the data is moving.

The Dot Size (s=150): Default chart dots are tiny and hard to see. Setting the size to a large, fixed number makes every year's data point stand out clearly in your VS Code notebook so they don't get lost on the page.

The Layering Order (zorder): Usually, Python draws lines right through the middle of dots, making them look messy. By setting the line to a lower layer and the dots to a higher layer, the trendline stays neatly in the background while the colorful year dots sit cleanly on top.