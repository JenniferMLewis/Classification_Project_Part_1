# <a name="top"></a>Telecom Customer Churn
![]()

by: Jennifer M Lewis

<p>
  <a href="https://github.com/JenniferMLewis" target="_blank">
    <img alt="Jennifer" src="https://img.shields.io/github/followers/JenniferMLewis?label=Follow Jenn&style=social" />
  </a>
</p>


***
[[Project Description](#project_description)]
[[Project Planning](#planning)]
[[Data Dictionary](#dictionary)]
[[Conclusion](#conclusion)]
___

<img alt="*** Photoshop resize this image!! ***" src="https://images.unsplash.com/photo-1659219870520-1008aba7dd64?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2080&q=80">

## <a name="project_description"></a>Project Description:
[[Back to top](#top)]

Document the code, process, findings, and key takeaways of the Telco Dataframe, analysing the different circumstances that lead to Customer Churn, and provide concise and coherent information for the forming of decisions that will lead to increased Customer Retention.

- Why are customers churning?
        
        
    - MVP: Broadly, I estimate Tenure and Monthly Charges play the most obvious role.
        - Further, I'd like to compare the role different services and their price play in the amount paid Monthly, as well as any role the average price of service for the elderly might affect the chance to Churn, since they typically require different types of services (ie. would including something like tech support on a senior plan help with senior churn [if senior churn is actually significant.])

***
## <a name="planning"></a>Project Planning: 
[[Back to top](#top)]

### Project Outline:

- Create Readme.md with Initial Hypotheses and/or questions of the data, Data Dictionary, Project and Business Goals.
- Create a function to automate the process of Acquring the data from the Codeup Database and Saving it as a .CSV then save the function to acquire.py for importing into the final report.
- Clean and prepare data for the MVP run through the pipeline. Create functions for the cleaning and preparation, save them in pepare.py to import into the final report.
- Define two Hypotheses, set alpha, run statistical tests, reject or fail to reject the Null Hypothesis, then document findings.
- Establish Basseline Accuracy.
- Train three different classification models.
- Evaluate models on train and validate datasets.
- Choose the model that preforms the best and evaluate that single model on the test dataset.
- Create .csv with the evaluated data columns, probably of the target values, and model's prediction for each entry in __test__ dataset.
- Document conclusions and recommendations in final report.
        
### Hypothesis

[MVP Hypothesis, the higher monthly charges and low tenure play a role in customer churn, as customers are more likely to leave if paying too much, and less loyal if they've not been a customer long. Contracts also play a role in how long a customer is mostlikely going to stay until they churn. Will have proper H0 and Ha Hypothosis later I hope!]

### Target variable

- Baseline accuracy of 73%

### Need to haves (Deliverables):

1. Git Hub Repo:
    - Readme(.md) [This Hopefully!]
        - Project Description w/ Goals
        - Initial Hypotheses and/or questions of the data, ideas.
        - Data Dictionary
        - Project Planning (Layout the Process Through the Data Science Pipeline).
        - Instructions or an explanation of how someone else can reproduce this project and findings (What would someone need to be able to recreate this project on their own?)
        - Key findings, recommendations, and takeaways
    - Final_Report.ipynb

***

## <a name="dictionary"></a>Data Dictionary  
[[Back to top](#top)]

### Data Used
---
| Attribute | Definition | Data Type |
| ----- | ----- | ----- |
| monthly_charges | Fees incurred Monthly by customer | 7043 non-null: int64 |
| payment_type_id | How customer Pays: 1 = electronic check 2 = mailed check, 3 = bank tranfer (automatic), 4 = credit card (automatic) | 7043 non-null: int64 |
| tenure | How long the customer has been with the company | 7043 non-null: int64 |
| gender_encoded | customer gender : 1 for Female, 0 for Male | 7043 non-null: int64 |
| senior_citizen | Is customer a Senior : 1 for Yes, 0 for No | 7043 non-null: int64 |

***

### <a name="conclusion"></a>Executive Summary : Conclusions and Next Steps
[[Back to top](#top)]


- Of the models created (DecisionTree, RandomForest, and KNeighbors), the predictions were fairly similar, within a percent or two, all above my Baseline Accuracy of 73%.
- DecisionTree and RandomForest preformed the best, and closest. At 77% and 78%.
- Some initial exploration and statistical testing revealed the possibility that payment type as well as various services offered might play a larger role, and with more time should be explored further.

***

###### ReadMe template by: <a href="https://github.com/mdalton87" target="_blank">Mathew Dalton</a>
</p>
