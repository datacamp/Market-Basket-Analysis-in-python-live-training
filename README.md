# **Market Basket Analysis**<br/>by **Isaiah Hull**

Live training sessions are designed to mimic the flow of how a real data scientist would address a problem or a task. As such, a session needs to have some “narrative” where learners are achieving stated learning objectives in the form of a real-life data science task or project. For example, a data visualization live session could be around analyzing a dataset and creating a report with a specific business objective in mind _(ex: analyzing and visualizing churn)_, a data cleaning live session could be about preparing a dataset for analysis etc ... 

As part of the 'Live training Spec' process, you will need to complete the following tasks:

Edit this README by filling in the information for steps 1 - 4.

## Step 1: Foundations 

This part of the 'Live training Spec' process is designed to help guide you through session design by having you think through several key questions. Please make sure to delete the examples provided here for you.

### A. What problem(s) will students learn how to solve? (minimum of 5 problems)

- Prepare data for use in Market Basket Analysis.
- Identify patterns in consumer decision-making with `mlxtend`.
- Use metrics to evaluate the properties of patterns.
- Construct association rules that provide concrete recommendations for businesses.
- Perform pruning to identify useful rules.
- Visualize patterns and rules using `seaborn` and `matplotlib`.

### B. What technologies, packages, or functions will students use? Please be exhaustive.

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `mlxtend`

### C. What terms or jargon will you define?

- Transaction: A set of items purchased together.
- Itemset: A collection of unique items.
- Association rule: an "if-then" statement of association between two itemsets. For instance, "if coffee then milk" is an association rule that implies that customers who purchase coffee are also likely to purchase milk.
- Metric: The numerical measure of the intensity of an association between itemsets.
- Pruning: The removal of itemsets or rules that perform poorly according to a metric.

### D. What mistakes or misconceptions do you expect? 

- I expect students to be confused about the definitions of metrics and how to interpret them.
- Students are likely to be confused about how the Apriori algorithm works and what it achieves.

### E. What datasets will you use? 

- Brazilian E-Commerce Public Dataset by Olist: https://www.kaggle.com/olistbr/brazilian-ecommerce

## Step 2: Who is this session for?

Terms like "beginner" and "expert" mean different things to different people, so we use personas to help instructors clarify a live training's audience. When designing a specific live training, instructors should explain how it will or won't help these people, and what extra skills or prerequisite knowledge they are assuming their students have above and beyond what's included in the persona.

- [x] Please select the roles and industries that align with your live training. 
- [x] Include an explanation describing your reasoning and any other relevant information. 

### What roles would this live training be suitable for?

*Check all that apply.*

- [ ] Data Consumer
- [ ] Leader 
- [x] Data Analyst
- [ ] Citizen Data Scientist
- [x] Data Scientist
- [ ] Data Engineer
- [ ] Database Administrator
- [x] Statistician
- [x] Machine Learning Scientist
- [ ] Programmer
- [ ] Other (please describe)

Reasoning: Market Basket Analysis has limited overlap with popular methods in machine learning and data science (e.g. deep learning, gradient boosting, clustering, etc.). As such, learning the basics of Market Basket Analysis will open up an entirely new toolset for many data analysts, data scientists, statisticians, and machine learning scientists.

### What industries would this apply to?

- Industries: Retail, e-commerce, streaming services.
- Reasoning: Market basket analysis can be used to analyze associations between itemsets in any domain. While it is typically applied in retail settings, it can also be used in other applications, such as building recommender systems for e-commerce sites or streaming services.

### What level of expertise should learners have before beginning the live training?

*List three or more examples of skills that you expect learners to have before beginning the live training*

- Can define and manipulate an `array` in `numpy`.
- Can define a `DataFrame` in `pandas`, create columns, and apply basic methods, such as `.mean()` and `.sum()`.
- Can use `.apply()` and `lambda` functions to transform columns in a `DataFrame`.
- Can generate basic plots in `matplotlib`.

## Step 3: Prerequisites

List any prerequisite courses you think your live training could use from. This could be the live session’s companion course or a course you think students should take before the session. Prerequisites act as a guiding principle for your session and will set the topic framework, but you do not have to limit yourself in the live session to the syntax used in the prerequisite courses.

[Data Manipulation with Pandas](
https://www.datacamp.com/courses/data-manipulation-with-pandas)

[Market Basket Analysis in Python](https://learn.datacamp.com/courses/market-basket-analysis-in-python)

## Step 4: Session Outline

A live training session usually begins with an introductory presentation, followed by the live training itself, and an ending presentation. Your live session is expected to be around 2h30m-3h long (including Q&A) with a hard-limit at 3h30m. You can check out our live training content guidelines [here](_LINK_). 


**Introduction Slides**
- Introduction to the webinar and instructor (led by DataCamp TA).
- Summary of webinar topics.
	- Define Market Basket Analysis.
	- Discuss applications.
	- Introduce packages used in webinar.
	- Set expectations about Q&A.

**Data Preparation**
- Discuss Brazilian e-commerce dataset.
- Import data using `pd.read_csv()`.
- Define transaction and itemset.
- Identify transactions in dataset using `pandas`
and `numpy` methods.
- Convert transactions to list of lists.
- Q&A

**Association Rules, Metrics, and Pruning**
- One-hot encode transactions using 
`TransactionEncoder` from `mlxtend`.
- Use `.mean()` to compute support for 
individual items.
- Use `.mean()` to compute support for
itemsets.
- Compute confidence using `lambda` function.
- Visualize results in `matplotlib` and `seaborn`.
- Q&A

**The Apriori Algorithm**
- Introduce `apriori` and `association_rules`
from `mlxtend`.
- Use `min_support`, `max_len`, and `min_threshold` to
perform pruning over itemsets and association rules.
- Identify useful association rules in e-commerce dataset 
through the use of pruning.
- Visualize results in `matplotlib` and `seaborn`.
- Q&A

**Ending Slides**
- Summarize webinar topics.
- Reference DataCamp course on MBA.
	- Explain additional topics covered.
- Provide additional supporting material and appendices.

## Authoring your session

To get yourself started with setting up your live session, follow the steps below:

1. Download and install the "Open in Colabs" extension from [here](https://chrome.google.com/webstore/detail/open-in-colab/iogfkhleblhcpcekbiedikdehleodpjo?hl=en). This will let you take any jupyter notebook you see in a GitHub repository and open it as a **temporary** Colabs link.
2. Upload your dataset(s) to the `data` folder.
3. Upload your images, gifs, or any other assets you want to use in the notebook in the `assets` folder.
4. Check out the notebooks templates in the `notebooks` folder, and keep the template you want for your session while deleting all remaining ones.

You can author and save your progress on your notebook using **either** of these methods.

_**How to author your notebook: By directly saving into GitHub**_

1. Preview your desired notebook, press on "Open in Colabs" extension - and start developing your content in colabs _(which will act as the solution code to the session)_.  :warning: **Important** :warning: Your progress will **not** be saved on Google Colabs since it's a temporary link. To save your progress, make sure to press on `File`, `Save a copy in GitHub` and follow remaining prompts.
2. Once your notebooks is ready to go, give it the name `session_name_solution.ipynb` create an empty version of the Notebook to be filled out by you and learners during the session, end the file name with `session_name.ipynb`. 
3. Create Colabs links for both sessions and save them in notebooks :tada: 

_**How to author your notebook: By uploading notebook into GitHub**_

1. Preview your desired notebook, press on "Open in Colabs" extension - and start developing your content in colabs _(which will act as the solution code to the session)_.  Once you're done, press on `file` - `download .ipynb` file - and overwrite the notebook by uploading it into GitHub. 
2. Once your notebooks is ready to go, give it the name `session_name_solution.ipynb` create an empty version of the Notebook to be filled out by you and learners during the session, end the file name with `session_name.ipynb`. 
3. Create Colabs links for both sessions and save them in notebooks :tada: 


You can check out either of those methods in action using this [recording](https://www.loom.com/share/1eeb148129244edd93fbc34bf5dc7f0d).
