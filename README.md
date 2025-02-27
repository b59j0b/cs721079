java c   Statistics Assignment #25 pointsMarketing Research
INSTRUCTIONS:
This assignment must be completed individually. This means that you may not ask any person other than the professor for help. You are permitted to use the internet to look up how to perform. certain operations in JASP or to look up certain statistical concepts. You can use generative AI (e.g., ChatGPT) to ask questions about what a certain term may mean or look up how to perform. a certain operation in JASP. You may not use AI to generate answers for any of these questions.   If you have any question, please ask the professor directly.
Instructions for this assignment assume that you are using JASP. You may use a different statistical software (e.g., SPSS, Stata, R) if you like, but it is your responsibility to make sure that the results, graphs, etc. from this software match the correct JASP output. Additionally, copy/pasting outputs directly from JASP into Word may cause some issues (e.g., table columns may not be properly aligned). As a result,   I recommend that you screenshot the JASP output   and then copy the screenshot into Word   rather than just using the copy/paste function in JASP. You may   not use Excel for this assignment.
For early assignments, I will give you relatively detailed instructions about how to perform. certain functions and tests in JASP and notes to go with them. Please note that these instructions apply to a relatively recent version of JASP (version 0.18.3) for macOS. Other versions of JASP or JASP running on Windows or Linux may differ slightly. Once we have covered a certain function, the instructions will be less detailed. You should go back and look at old assignments and questions to see the more detailed notes on a certain function.

Please use the “IBM Watson Customer Lifetime Value.csv” dataset posted on Canvas. 
This is a dataset that examines customer lifetime value for a car insurance company. Specifically, it contains detailed customer profile data, the service (policy) customers purchased, the vehicle information, the claim information, and whether customers responded to a recent promotion.   Here is a list of the variables in the data:
·   Customer
·   State
·   Customer Lifetime Value
·   Response
·   Coverage
·   Education
·   Effective To Date
·   Employment Status
·   Gender
·   Income
·   Location Code
·   Marital Status
·   Monthly Premium Auto
·   Months Since Last Claim
·   Months Since Policy Inception
·   Number of Open Complaints
·   Number of Policies
·   Policy Type
·   Policy
·   Renew Offer Type
·   Sales Channel
·   Total Claim Amount
·   Vehicle Class
·   Vehicle Size

For the first two questions in this assignment, imagine that the insurance company is evaluating whether the amount people claim differs based on gender and marital status. Specifically, the company wants to know:a.   Do people of different gender groups (on average) claim different amounts?b.   Do people of different marital status (on average) claim different amounts?
Question 1 (1.75 points total)
Load the data using the same method that you used in Assignment #1. 
For research question (a), the dataset divides gender into two groups (it is an old dataset). Because you are comparing claim amounts between two groups, the best way to do this is by using a t-test.   T-tests are quick tests that tell you if the averages of some variable (in this case, claim amounts) are different across two groups (in this case, genders).
To conduct a t-test in JASP, first click on the big “T-Tests” button at the top of the window. Click on “Independent Samples T-Test” under the “Classical” header. You choose “Independent Samples” because you are comparing different groups of people.   You would choose “Paired Samples T-Test” if you were comparing datapoints from the same person at two different times. You would choose “One Sample T-Test” if you were just comparing the average of one group to a specific value (for instance, if the average claim was greater than $1,000).
You should now see a new window that shows you the list of variables in the data on the left and a blank t-test “results table” on the right. On the left side, there is also two empty fields for “Dependent Variables” and “Grouping Variable.” Under the “Dependent Variables” field, you should put “Total Claim Amount.” You put this variable there because it is the variable you are comparing across the two groups. Under the “Grouping Variable” you should put “Gender.” You put this variable there because it contains the groups that you are comparing. A.   Paste the screenshot of the T-Test result below (0.5 points):B.   What is the p-value associated with the test? (0.25 points):C.   Assume that you have a null hypothesi代 写Statistics Assignment #2 Marketing ResearchJava
代做程序编程语言s that men and women both submit the same size claims, on average. Before you run the test, you set a p-value cutoff (i.e., alpha value) of 0.05. Given the p-value from part (B), do you reject or fail to reject your null hypothesis? (0.25 points)D.   Given your decision in part (C), do you believe men and women submit different average claim amounts? (0.25 points)E.   Using information only from the test you just ran   (i.e., using only what is in your answer from part A), can you conclude that men submit larger claims, on average, than women do? Why or why not? (0.5 points)
Question 2 (1.25 points)
For research question (b), the dataset divides marital status into 3 groups (Divorced, Married, and Single). Because T-Tests only allow you to compare averages across two groups, you need to use an ANOVA in this question to compare averages across more than two groups.   
To conduct an ANOVA in JASP, first click on the big “ANOVA” button at the top of the window. Click on “ANOVA” under the “Classical” header. The process for conducting an ANOVA test in JASP is nearly identical to conducting a T-Test. The main difference is that the “Grouping Variable” field from the T-Test is called “Fixed Factors” for ANOVA. So, put “Total Claim Amount” in the “Dependent Variable” field and “Marital Status” in the “Fixed Factor” field.A.   Paste the screenshot of the ANOVA result below. (0.5 points)B.   What is the p-value associated with this test? (0.25 points)C.   Unlike with t-tests, ANOVAs by themselves can only tell you if there are any differences between averages across the groups you are testing. That is, for example, it can only tell you if married people submit different claim amounts on average than single people OR if single people submit different amounts than divorced people OR if married people submit different claim amounts than divorced people. However, it cannot tell you which one of those it is.   So, in this case, your null hypothesis is that “there are no differences in average claim amounts across groups.”
Assuming a p-value cutoff (i.e., alpha value) of 0.05, do you reject or fail to reject this null hypothesis? (0.25 points)D.   What do you conclude from this test? That is, do people with different marital statuses submit different average claim amounts or not? (0.25 points)
Question 3 (1 point total) (EXAM)
Imagine that you want to know whether income is positively correlated with house size. That is, do people who make more money own bigger houses? To do this, you write a survey that asks people how much money they make per year and how big their house is. You then run a correlation test to see if the correlation between income and house size is significantly different from zero. The test shows you that the correlation is 0.51 and the p-value is .01.
a. Does this result suggest that there is likely to be a relationship between income and house size? (0.25 points)
YES                                                      NO
b. Does this result suggest that earning a higher income causes people to buy larger houses? (0.25 points)
YES                                                      NOc.   If the p-value of the test was .001 instead of .01, would this make you more   confident or less   confident that there is a reliable relationship between income and house size? (0.25 points)
MORE CONFIDENT                                LESS CONFIDENTd.   Suppose that you wanted to become more confident that this relationship exists. Holding all else equal, which of these could you   change to make the evidence of the relationship stronger? (0.25 points)
INCREASE SAMPLE SIZE                                INCREASE VARIANCE         
INCREASE CORRELATION SIZE

Question 4 (1 point total) (EXAM)
Imagine that you want to know whether people are willing to drive at least 10 miles to shop at Trader Joe’s.
To do this, you send potential Trader Joe’s shoppers a survey that asks them three different questions:1.   How far are you willing to drive to shop at Trader Joe’s? [Open Ended]2.   Are you willing to drive at least 10 miles to shop at Trader Joe’s? Yes or No3.   How willing are you to drive at least 10 miles to shop at Trader Joe’s? Definitely would not, Probably would not, I don’t know, Probably would, or Definitely would
For Question 1, 8% of people gave a number larger than 10 miles.
For Question 2, 10% of people answered “Yes.”
For Question 3, 15% of people said either “Probably would” or “Definitely would.” We will assume that these people would drive 10 miles if they had to.a.   Given these results, what is your best guess of the true proportion of people who would drive 10 miles to shop at Trader Joe’s? (0.5 points)b.   Explain your answer to part a. (0.5 points)
   

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
