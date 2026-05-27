Tyler Hann: First ai prompt

1. 
# Asked AI to teach me how to remove rows not needed.

Prompt:
    Hey Can you teach me how to remove empty rows/Give me the code in order for me to be able to remove full empty rows that makes the data Not applicable for further/later research. Do not write it for me i would just like to know the structure behind and what to do in order for this.

Response:
Example Structure using "df = df.dropna(how='all')" which is after first loading the excel file and then using dropna(how='all') will delete rows ONLY when the row is actually missing.

2. 