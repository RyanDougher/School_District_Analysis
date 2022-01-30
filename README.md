# School_District_Analysis

## School district analysis with Python

### Purpose

A school district asked for an analysis of key metrics for each school within the district. The analysis consisted of the overall performance of math and reading scores by school and grade level. After the initial review, it was apparent that the data from Thomas High School's 9th grade was innaccurate. The analysis was redone after removing the questionable data.

## Results

### How is the district summary affected?

Original Analysis:
![Original_district_summary_df](https://user-images.githubusercontent.com/96550846/151715035-c3dea6e2-d70b-4848-a59d-f5a1557e3a70.png)

The reading and math scores of the 491 students in the 9th grade at Thomas High School was turned into Null data. Without chainging the total student count, the percentages of passing math, passing reading, and overall passing were all adjusted.

Adjusted Analysis:
![Adjusted_district_summary_df](https://user-images.githubusercontent.com/96550846/151715123-df7e2b4b-7451-4e26-a116-55254d4f9e03.png)

We can see that this had a very small impact on the data set as a whole. The change was less than a 1% difference, and with rounding, almost imperceivable.

### How is the school summary affected?

The original school analysis showed Thomas High School with high passing percentages: 93% for math, 97% for reading, and about 91% overall. An observation was made that this data was innacurate, so new passing percentages were calculated for Thomas High School by excluding the 9th grade scores.

Original school summary:
![Original_school_Summary_df](https://user-images.githubusercontent.com/96550846/151715257-bb4b6b15-8e66-4e69-95bf-ad5287114502.png)

Adjusted school summary:
![Adjusted_school_summary_df](https://user-images.githubusercontent.com/96550846/151715263-666e9c96-d3d8-41c5-849f-7dcb20eff5e8.png)

The new adjusted school summary brought the overall passing percentage for Thomas High School down to 65%.

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

The original analysis had Thomas High School ranked 2nd in the district. After adjusting the data to remove the 9th grade data, Thomas High School dropped to the 7th ranked school in the district.

### How does replacing the ninth-grade scores affect the following:

#### Math and reading scores by grade

The original analysis showed an 83.6 math average and 83.7 reading average for the 9th grade at Thomas High School. After adjsuting the data, the 9th grade scores for Thomas High Schools math and reading are shown as NaN.

Adjusted math scores by grade:
![Adjusted_math_scores_by_grade](https://user-images.githubusercontent.com/96550846/151715570-9ede7f85-2a37-469a-8d8b-b72036ed8736.png)

#### Scores by school spending

The change to the scores by school spending analysis was nominal. Thomas High School falls in the $630-$644 range, but we see no difference because this is rounded to the nearest whole number. We would have to add two decimal places in order to see this small change.

Original analysis of scores by school spending:
![Original_spending_range](https://user-images.githubusercontent.com/96550846/151715733-54ba3221-11b0-4a27-a736-28b886824b05.png)

Adjsuted analysis of scores by school spending:
![Adjusted_spending_range](https://user-images.githubusercontent.com/96550846/151715743-480c006a-32ce-4e47-a980-3cb738af0bd4.png)

#### Scores by school size

Similar to the scores by school spending, the changes to scores by school size were small enough that it does not show in the images below. We would need to add two decimal places to see this small change.

Original analysis of scores by school size
![Original_scores_by_size](https://user-images.githubusercontent.com/96550846/151715885-be36b9a0-a760-4bf8-abb9-9a9133fb45d6.png)

Adjsuted analysis of scores by school size
![Adjusted_scores_by_size](https://user-images.githubusercontent.com/96550846/151715882-abbb566b-e2c9-40d3-9c57-6441962fa5b2.png)

#### Scores by school type

Similar to the above, no noticeable change was made to the scores by school type. Two decimal places would need to be added to see this small change.

Original analysis of scores by school type
![Original_scores_by_type](https://user-images.githubusercontent.com/96550846/151715995-f8f8b47b-0ad6-442a-bc9e-752ffafb0334.png)

Adjusted analysis of scores by school type
![Adjusted_scores_by_type](https://user-images.githubusercontent.com/96550846/151716008-2fa6cd3a-6d14-452e-a16d-10dbc12b352c.png)

## Summary

### Four changes made to the school district analysis after replacing Thomas High School's 9th grade data.

1. The math passing rate, reading passing rate, and overall passing rate for Thomas High School dropped dramatically after replacing the 9th grade data with NaNs.
2. After replacing the 9th grade data for Thomas High School, their ranking dropped from 2nd to 7th.
3. The 9th grade data for Thomas High School is how shown as NaN in the dataframe.
4. In any category that contained Thomas High School for the scores by school spending or scores by school size, the passing rates were decreased slightly.
