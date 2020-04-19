Project 1: SAT & ACT Analysis

### Overview

This is a project done for the Data Science Immersive 14 course done with General Assembly Singapore.

We were tasked to examine possible correlations that may exist between the state average subject scores and participation rates of the SAT and ACT tests. The new format of the SAT was just released in March 2016 and we are interested in finding out where the College Board (which administers the SAT) should dedicate their funding.

Executive Summary:
The four datasets that we worked with were from 2017 and 2018; they contained the state averages of participation and test scores for the ACT and SAT tests. The full list of columns are given in the data dictionary below. The distribution for ACT and SAT participation rates were noticeably skewed to either ends, further research showed that 23 out of the 50 states administer either one of the tests and students rarely sat for both. It was also observed that test scores of ACT and SAT were unsuitable for statistical inference as the tests were designed differently resulting in different formats and scoring scales. Student performance on either tests would have to be compared against similar states who administer the same tests. It was also problematic accounting for other possible factors to a state's participation to the ACT or SAT test, whether the test was administered free of charge in that state or accounting for student population sizes in the different states.

---
|Feature|Type|Dataset|Description|
|---|---|---|---|
|state_index|*object*|ACT SAT|The 51 States of America
|act_2017_participation|*float*|ACT|ACT 2017 Participation rate for each State (given as a % of graduates from that state in that year)
|act_2017_english|*float*|ACT|ACT 2017 Average English scores per State
|act_2017_math|*float*|ACT|ACT 2017 Average Math scores per State
|act_2017_reading|*float*|ACT|ACT 2017 Average Reading scores per State
|act_2017_science|*float*|ACT|ACT 2017 Average Science scores per State
|act_2017_composite|*float*|ACT|ACT 2017 Average Composite scores per State (scale score taken from the raw scores of  ACT English, Math, Reading and Science tests)
|act_2018_participation|*float*|ACT|ACT 2018 Participation rate for each State (given as a % of graduates from that state in that year)
|act_2018_english|*float*|ACT|ACT 2018 Average English scores per State
|act_2018_math|*float*|ACT|ACT 2018 Average Math scores per State
|act_2018_reading|*float*|ACT|ACT 2018 Average Reading scores per State
|act_2018_science|*float*|ACT|ACT 2018 Average Science scores per State
|act_2018_composite|*float*|ACT|ACT 2018 Average Composite scores per State (scale score taken from the raw scores of  ACT English, Math, Reading and Science tests)
|sat_2017_participation|*float*|SAT|SAT 2017 Participation rate for each State
|sat_2017_reading_writing|*integer*|SAT|SAT 2017 Average Evidence-Based Reading and Writing scores per State
|sat_2017_math|*Integer*|SAT|SAT 2017 Average Math scores per State
|sat_2017_total|*Integer*|SAT|SAT 2017 Average Total scores per State
|sat_2018_participation|*float*|SAT|SAT 2018 Participation rate for each State
|sat_2018_reading_writing|*integer*|SAT|SAT 2018 Average Evidence-Based Reading and Writing scores per State
|sat_2018_math|*Integer*|SAT|SAT 2018 Average Math scores per State
|sat_2018_total|*Integer*|SAT|SAT 2018 Average Total scores per State
---

We recommend that we look further into California, by population size is the largest state population in the US, a percentage increase in this state would ensure the greatest coverage of students taking the SAT tests as compared to the other states that were considered. There were three states where the combined participation in ACT and SAT were in the 70 percent range (Iowa, Kansas and New Mexico) but taking into account the current population density of those states and the expected population growth of those countries, they are less attractive candidates. in California, 60% of the graduating class took the SAT as compared to 27% who took the ACT, combining for a total of 87% participation. That equates to about 850,000 students not covered by either the ACT or SAT test in California based on National Center for Education Statistics for Enrollment in public schools.

References:
Colorado made the switch from ACT to SAT in late 2017
https://www.denverpost.com/2017/03/06/colorado-juniors-sat-college-exam/
States the require their student to take either the SAT or ACT
https://www.ecs.org/wp-content/uploads/State-Information-Request_Use-of-ACT-SAT-and-PSAT-for-High-School-Testing-as-Required-by-ESSA.pdf
California's SAT annual report for 2017
https://reports.collegeboard.org/pdf/2017-california-sat-suite-assessments-annual-report.pdf
Kansas's SAT annual report for 2017
https://reports.collegeboard.org/pdf/2017-kansas-sat-suite-assessments-annual-report.pdf
Iowa's SAT annual report for 2017
https://reports.collegeboard.org/pdf/2017-iowa-sat-suite-assessments-annual-report.pdf
