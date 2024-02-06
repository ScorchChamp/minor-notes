# What is CRISP-DM?
> [Source: www.datascience-pm.com](https://www.datascience-pm.com/crisp-dm-2/)
> 
The **CR**oss **I**ndustry **S**tandard **P**rocess for Data Mining (CRISP-DM) is a process model that serves as the base for a data science process. It has six sequential phases:
1. Business understanding – What does the business need?
2. Data understanding – What data do we have / need? Is it clean?
3. Data preparation – How do we organize the data for modeling?
4. Modeling – What modeling techniques should we apply?
5. Evaluation – Which model best meets the business objectives?
6. Deployment – How do stakeholders access the results?

## I. Business Understanding
Any good project starts with a deep understanding of the customer’s needs. Data mining projects are no exception and CRISP-DM recognizes this.

The Business Understanding phase focuses on understanding the objectives and requirements of the project. Aside from the third task, the three other tasks in this phase are foundational project management activities that are universal to most projects:

Determine business objectives: You should first “thoroughly understand, from a business perspective, what the customer really wants to accomplish.” (CRISP-DM Guide) and then define business success criteria.
Assess situation: Determine resources availability, project requirements, assess risks and contingencies, and conduct a cost-benefit analysis.
Determine data mining goals: In addition to defining the business objectives, you should also define what success looks like from a technical data mining perspective.
Produce project plan: Select technologies and tools and define detailed plans for each project phase.
While many teams hurry through this phase, establishing a strong business understanding is like building the foundation of a house – absolutely essential.

## II. Data Understanding
Next is the Data Understanding phase. Adding to the foundation of Business Understanding, it drives the focus to identify, collect, and analyze the data sets that can help you accomplish the project goals. This phase also has four tasks:

Collect initial data: Acquire the necessary data and (if necessary) load it into your analysis tool.
Describe data: Examine the data and document its surface properties like data format, number of records, or field identities.
Explore data: Dig deeper into the data. Query it, visualize it, and identify relationships among the data.
Verify data quality: How clean/dirty is the data? Document any quality issues.

## III. Data Preparation
A common rule of thumb is that 80% of the project is data preparation.

This phase, which is often referred to as “data munging”, prepares the final data set(s) for modeling. It has five tasks:

Select data: Determine which data sets will be used and document reasons for inclusion/exclusion.
Clean data: Often this is the lengthiest task. Without it, you’ll likely fall victim to garbage-in, garbage-out. A common practice during this task is to correct, impute, or remove erroneous values.
Construct data: Derive new attributes that will be helpful. For example, derive someone’s body mass index from height and weight fields.
Integrate data: Create new data sets by combining data from multiple sources.
Format data: Re-format data as necessary. For example, you might convert string values that store numbers to numeric values so that you can perform mathematical operations.

## IV. Modeling
What is widely regarded as data science’s most exciting work is also often the shortest phase of the project.

Here you’ll likely build and assess various models based on several different modeling techniques. This phase has four tasks:

Select modeling techniques: Determine which algorithms to try (e.g. regression, neural net).
Generate test design: Pending your modeling approach, you might need to split the data into training, test, and validation sets.
Build model: As glamorous as this might sound, this might just be executing a few lines of code like “reg = LinearRegression().fit(X, y)”.
Assess model: Generally, multiple models are competing against each other, and the data scientist needs to interpret the model results based on domain knowledge, the pre-defined success criteria, and the test design.
Although the CRISP-DM Guide suggests to “iterate model building and assessment until you strongly believe that you have found the best model(s)”,  in practice teams should continue iterating until they find a “good enough” model, proceed through the CRISP-DM lifecycle, then further improve the model in future iterations.

## V. Evaluation
Whereas the Assess Model task of the Modeling phase focuses on technical model assessment, the Evaluation phase looks more broadly at which model best meets the business and what to do next. This phase has three tasks:

Evaluate results: Do the models meet the business success criteria? Which one(s) should we approve for the business?
Review process: Review the work accomplished. Was anything overlooked? Were all steps properly executed? Summarize findings and correct anything if needed.
Determine next steps: Based on the previous three tasks, determine whether to proceed to deployment, iterate further, or initiate new projects.

## VI. Deployment
“Depending on the requirements, the deployment phase can be as simple as generating a report or as complex as implementing a repeatable data mining process across the enterprise.”

–CRISP-DM Guide

A model is not particularly useful unless the customer can access its results. The complexity of this phase varies widely. This final phase has four tasks:

Plan deployment: Develop and document a plan for deploying the model.
Plan monitoring and maintenance: Develop a thorough monitoring and maintenance plan to avoid issues during the operational phase (or post-project phase) of a model.
Produce final report: The project team documents a summary of the project which might include a final presentation of data mining results.
Review project: Conduct a project retrospective about what went well, what could have been better, and how to improve in the future.
Your organization’s work might not end there. As a project framework, CRISP-DM does not outline what to do after the project (also known as “operations”). But if the model is going to production, be sure you maintain the model in production. Constant monitoring and occasional model tuning is often required.

## Is CRISP-DM Agile or Waterfall?
Some argue that it is flexible and agile and while others see CRISP-DM as rigid. What really matters is how you implement it.

**Waterfall**: On one hand, many view CRISP-DM as a rigid waterfall process – in part because of its reporting requirements are excessive for most projects. Moreover, the guide states in the business understanding phase that “the project plan contains detailed plans for each phase” – a hallmark aspect of traditional waterfall approaches that require detailed, upfront planning.

Indeed, if you follow CRISP-DM precisely (defining detailed plans for each phase at the project start and include every report) and choose not to iterate frequently, then you’re operating more of a waterfall process.

**Agile**: On the other hand, CRISP-DM indirectly advocates agile principles and practices by stating: “The sequence of the phases is not rigid. Moving back and forth between different phases is always required. The outcome of each phase determines which phase, or particular task of a phase, has to be performed next.”

**Thus** if you follow CRISP-DM in a more flexible way, iterate quickly, and layer in other agile processes, you’ll wind up with an agile approach.


## Most used development cycles
![KDnuggets poll](https://www.datascience-pm.com/wp-content/uploads/2020/10/kdnuggets-polls.png)
*KDnuggets poll, visualized by datascience-pm: https://www.kdnuggets.com/2014/10/crisp-dm-top-methodology-analytics-data-mining-data-science-projects.html*

![datascience-pm poll](https://www.datascience-pm.com/wp-content/uploads/2021/04/dspm-poll-2020-10.png)
*datascience-pm poll: https://www.datascience-pm.com/crisp-dm-2/*

# In our own words:
> by Lars Cornelissen
1. **What** do we want to **achieve** as a **business**?
2. Do we already have some **useful data** to achieve our **goal**?
3. How do we **organize** the data to get some **information** out of it?
4. What **modelling techniques** should we apply to the data?
5. **What model** gets the **best result** for our goal in step 1?
6. How should the **business** see the **result**?