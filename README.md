| Prompt Techniques | Output Format Score | Brief Observation |
|---|---|---|
| Baseline | 6 | It looks like it takes all the raw text data and sets it as CSV entries, but it also makes it look very bloated. For example "First Pokémon generation" Could just be "1st" |
| Role Prompt | 6.2 | Only notable difference would be the "Release date (Worldwide)" column compared to baseline |
| Chain-of-Thought | 7.2 | A huge jump in improvement, most notably at the "Generation" column. |
| Self Refine | 6.8 | Even when asking Gemini to critique itself, it looks like it was satisfied with the inital baseline prompt output and didn't change much. The column titles are much better. |
| Final (COT + Self Refine) | 7.5 | This two step final prompt approach produced an output I was pretty satisfied with. Although, it's missing elements that already exsited with the previous prompt techniques. |