# IowaDemCaucus2020

Scraped copies of the results of the 2020 Iowa Democratic Caucus from <https://results.thecaucuses.org/>.


## Contents

- `Iowa_caucus_harvest.Rmd`: The script that scrapes <https://results.thecaucuses.org/> and produces a tidy dataframe of the results.
    - `Iowa_caucus_harvest [timestamp].Rmd`: Finished runs of the above.
- `_compiled/`: Output folder of timestamped caucus results, in 'long' format.
    - **county**: County name
    - **precinct**: Precinct name
        - Can also be _Total_, which is the published Total for each county x candidate x measure.
        - Can also be _Total_recalc_, which is a total for each county x candidate x measure that is calculated by my script.
    - **candidate**: Candidate name
    - **measure**: 
        - _expression_1_ ("First Expression" on the website)
        - _expression_2_ ("Final Expression" on the website)
        - _sde_ ("SDE" on the website)
    - **value**: The published value of **measure**.
