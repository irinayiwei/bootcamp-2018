# MSIA Boot Camp - Final R exercise

You've learned quite a lot about R in a short time. Congratulations! This exercise is designed to give you some additional practice on the material we have discussed this week while the lectures are still fresh in your mind, and to integrate different tools and skills that you have learned.

## Instructions

#### Task 1: Import your data 

Read the data files `nys_schools.csv` and `nys_acs.csv` into R. These data come from two different sources: one is data on *schools* in New York state from the [New York State Department of Education](http://data.nysed.gov/downloads.php), and the other is data on *counties* from the American Communities Sruvey from the US Census Bureau. Review the codebook file so that you know what each variable name means in each dataset. 

#### Task 2: Recoding and variable manipulation

1. Deal with missing values, which are currently coded as `-99`.
2. Create a categorical variable that groups counties into "high", "medium", and "low" poverty groups. Decide how you want to split up the groups and briefly explain your decision. 
3. The tests that the NYS Department of Education administers changes from time to time, so scale scores are not directly comparable year-to-year. Create a new variable that is the standardized z-score for math and English Language Arts (ELA) for each year (hint: group by year and use the `scale()` function)

#### Task 3: Merge datasets

Create a county-level dataset that merges variables from the schools dataset and the ACS dataset. Remember that you have learned multiple approaches on how to do this, and that you will have to decide how to summarize data when moving from the school to the county level.

#### Task 4: Create summary tables

Generate tables showing the following:

1. For each county: total enrollment, percent of students qualifying for free or reduced price lunch, and percent of population in poverty.
2. For the counties with the top 5 and bottom 5 poverty rate: percent of population in poverty, percent of students qualifying for free or reduced price lunch, mean reading score, and mean math score.

#### Task 5: Data visualization

Using `ggplot2`, visualize the following:

1. The relationship between access to free/reduced price lunch and test performance, at the *school* level.
2. Average test performance across *counties* with high, low, and medium poverty.

#### Task 6: Answering questions

Using the skills you have learned in the past three days, tackle the following question: 

> What can the data tell us about the relationship between poverty and test performance in New York public schools? Has this relationship changed over time? Is this relationship at all moderated by access to free/reduced price lunch?

You may use summary tables, statistical models, and/or data visualization in pursuing an answer to this question. Feel free to build on the tables and plots you generated above in Tasks 4 and 5.

Given the short time period, any answer will of course prove incomplete. The goal of this task is to give you some room to play around with the skills you've just learned. Don't hesitate to try something even if you don't feel comfortable with it yet. Do as much as you can in the time allotted.

## Github submission

When you have completed the exercise, commit your RMarkdown file to our shared Github repo [NEED TO ADD DETAILS]. Make sure your file has the following filename structure: `FinalRExercise_LastnameFirstname.Rmd`.

## Reminders

- Remember to **load necessary packages**.
- Remember to **comment extensively** in your code. Since you will be working in an RMarkdown file, you can describe your workflow in the text section. But you should also comment within all of your code chunks.
- Attempt to knit your Markdown file into HTML format before committing it to Github. Troubleshoot any errors with the knit process by checking the lines referred to in the error messages.