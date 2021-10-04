# School Analysis Project

## Overview and Background
The purpose of this analysis is to take a set of fake data on schools in a certain school district and to do multiple things with it. The first thing that must be done is the purging of all scores that are considered to no longer be valid, in this case all 9th graders at Thomas High School have been determined to no longer have valid test scores and must therefore be purged from the dataset to hold up the integrity of the analysis. And due to the purging of the data we much adjust the data from Thomas High School to ignore the 9th graders so that the school does not show innacurate percentages for students passing the tests in their school analysis compared to the rest of the school district. 

## Analysis and Differences
Now we must actually double check how losing the scores of the 9th graders affected Thomas High School

![Original Data](https://i.imgur.com/VykMqNk.png)

This is the summary of the data not taking into account that all 9th graders must be ignored in the passing rates of Thomas High School

![Adjusted Data](https://imgur.com/cJPGbUD.png)

This is the adjusted data showing how Thomas High School passing percentages look without the 9th graders.

- From these images we can see that without adjusting for the 9th graders score being invalid the entirety of Thomas High School moves from one of the top schools in the district to one of the worst
- To be exact the overall passing rate in Thomas High School jumped up nearly 20% once you factored out the null values left by the purged 9th grade scores.
- This shows in the fact that it went from one of the bottom 5 schools in the districts to one of the top 5 with just this one adjustment in data.

Now we should look at how this change in data has effected the overall analysis of the data from the original one done prior to purging the 9th graders.

![Math Scores](https://imgur.com/h4zCrdV.png)

These are the Math Scores by Grade

![Reading Scores](https://i.imgur.com/jPpLkRr.png)

These are the Reading Scores by Grade

- As we can see here the 9th grade score is completely thrown out and replaced with NaN in these charts. 
- This means that the scores for the other grades are completely unaffected as only 9th graders at Thomas High School were the ones purged as a part of this analysis.
- We can also see how the scores of the other grades at Thomas High School match those of the top scoring schools in the district and not of the lower ones that the original data would have you belive Thomas High School was a part of.

## Summary 
From this data we can see that there is no large difference in the data of Thomas High Schools 10-12th grade scores from those of the other top scoring schools in the district. This means that it is best to indeed throw out the 9th grade null scores to better reflect the true nature of the school in the data compared to that of the picture that was painted by the data taking those null values into account still. While there weren't many major changes in the data this has actually pulled up Thomas High School as a higher performing school for the money spent per capita. It also puts it near the top of the pack with it's medium size. 
