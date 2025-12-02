## Project Title: AD 331 Prompt Engineering for Performance Improvement 
#### By: Amde Wubshet

### Task: 
Asking a LLM to generate a .CSV file using multiple prompt techniques along with raw text data as input.

### LLM Used: 
Google Gemini 3

| Prompt Techniques | Output Format Score (1 to 10) | Brief Observation |
|---|---|---|
| Baseline | 6 | It looks like it takes all the raw text data and sets it as CSV entries, but it also makes it look very bloated. For example "First Pokémon generation" Could just be "1st" |
| Role Prompt | 6.2 | Only notable difference would be the "Release date (Worldwide)" column compared to baseline |
| Chain-of-Thought | 7.2 | A huge jump in improvement, most notably at the "Generation" column. |
| Self Refine | 6.8 | Even when asking Gemini to critique itself, it looks like it was satisfied with the inital baseline prompt output and didn't change much. The column titles are much better. |
| Final (COT + Self Refine) | 7.5 | This two step final prompt approach produced an output I was pretty satisfied with. Although, it's missing elements that already exsited with the previous prompt techniques. |


### Key Lessons: 
I feel like these prompt techniques do make a huge difference for output generation from LLMs, but only using these techniques as a singular query leads to answers that are less than ideal (in my opinion). By using multiple techniques and multiple prompts for a task, you can get a pretty decent response from an LLM.     