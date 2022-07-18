# School District Analysis
## Overview of the School District Analysis 
### Purpose and Background
Chief Data Scientist, Maria, has asked me to help analyze information on schools, funding, standardized test scores, and performance trends. The school board has noticed evidence of academic dishonesty and requests we modify the results for the ninth grade class at Thomas High School, while keeping all other data intact. After doing so, we will compare the results and describe how the changes affect the overall analysis. The following are the new steps and adjustments made from the original code:
1. Install NumPy.
2. Utilize Pandas loc method to retrieve scores for Thomas High School's ninth grade class.
3. Replace ninth grade reading and math scores from Thomas High School with NaN using "np.nan".
4. Create a new district summary.
5. Create a new school summary.
6. Calculate new passing average percentages for math, reading, and overall.
7. Compare results. 
## Results
- How is the district summary affected?

At a glance, the tables show there is hardly any difference even after we adjust Thomas High School's ninth grade class data to NaN. There is less than a one percent difference. If we were rounding to whole numbers, the data would remain identical.

Original district summary: 
<img width="1009" alt="Screen Shot 2022-07-17 at 4 35 27 PM" src="https://user-images.githubusercontent.com/107595127/179429328-b264a7de-0ea0-4b32-bfb1-16d0cb56b297.png">

Adjusted district summary:
<img width="1012" alt="Adjusted District Summary" src="https://user-images.githubusercontent.com/107595127/179429280-c09f84bb-5ab1-4631-b4b1-6b2d36c1d822.png">

- How is the school summary affected?

When looking at the school summary, we notice a more drastic change. The overall percentage drops about 25% when we compare Thomas High School results with and without ninth grade data. 

Original School Summary:
<img width="862" alt="Original School Summary" src="https://user-images.githubusercontent.com/107595127/179432462-bbca6320-5ba5-4026-813b-033c7a837445.png">

Adjusted School Summary:
<img width="865" alt="Adjusted School Summary" src="https://user-images.githubusercontent.com/107595127/179432486-9f79998c-8688-4478-b142-fa75738503a8.png">

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Replacing the ninth graders' math and reading scores has no affect on Thomas High School's performance. As you can see from the images below, Thomas High School is still in the top five performing schools and ranked #2. After replacing the ninth graders' scores, the data practically remains the same.

Original School Performance:
<img width="858" alt="Original Performance" src="https://user-images.githubusercontent.com/107595127/179432950-479f7960-664d-4cb9-8010-f33a50578588.png">

Adjusted School Performance:
<img width="865" alt="Adjusted Performance" src="https://user-images.githubusercontent.com/107595127/179432971-69da3cb3-6082-47c2-bf41-f11110e03a28.png">

### How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade:
    
When replacing the Math and reading scores, the DataFrame has no value for Thomas High School's ninth  grade class. Instead, NaN is displayed. 
 
Original Math Scores:

<img width="328" alt="Original Math" src="https://user-images.githubusercontent.com/107595127/179435918-36f8ac8b-82aa-49b9-a37c-0369863263fe.png">

  
Adjusted Math Scores:

<img width="330" alt="Adjusted Math" src="https://user-images.githubusercontent.com/107595127/179437437-26667c29-fff2-4cdc-84a4-71b5d3830298.png">

  
Original Reading Scores:

<img width="324" alt="original reading score" src="https://user-images.githubusercontent.com/107595127/179434209-d51aef75-a097-47eb-b46f-1786378bf0de.png">

Adjusted Reading Scores:

<img width="321" alt="Adjusted Reading" src="https://user-images.githubusercontent.com/107595127/179434077-aa5f7006-b2a9-4fba-8c32-6ab9a1af26c8.png">

- Scores by school spending:

There is no change in scores by school spending. 

Original School Spending:

<img width="866" alt="Original Spending" src="https://user-images.githubusercontent.com/107595127/179435318-932f2323-6197-4bdb-853f-16cd5a6dd967.png">


Adjusted Spending:

<img width="862" alt="Adjust School Spending" src="https://user-images.githubusercontent.com/107595127/179435690-137d937a-fa4a-4730-874e-f5eb8b08cbc6.png">


- Scores by school size:

There is no change in scores by school size.

Original School Size:

<img width="872" alt="Original size" src="https://user-images.githubusercontent.com/107595127/179435341-aac06cb9-90c2-4f1f-a326-4f6cd1ad4cfb.png">


Adjusted School Size:

<img width="872" alt="Adjust School Size" src="https://user-images.githubusercontent.com/107595127/179435712-e2c16a94-b916-46a2-9d88-5482fe6adbf6.png">

- Scores by School Type:

There is no change in scores by school types. 

Original School Type:

<img width="772" alt="Original School Type" src="https://user-images.githubusercontent.com/107595127/179435370-9f556af8-6dd3-4445-be53-bf7a84ee7ba6.png">

Adjusted School Type: 

<img width="774" alt="Adjust School type" src="https://user-images.githubusercontent.com/107595127/179435739-4fb19509-e26b-4582-a331-61ac41d5cf4d.png">

# Summary
When replacing the data for Thomas High School's ninth grade class with NaN, there are no differences to school spending, school size, or school type. We only removed the ninth grade class' scores. We did not remove the students from the overall DataFrame. In other words, the students are still accounted for, except their scores. 
