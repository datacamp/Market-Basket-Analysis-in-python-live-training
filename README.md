# **Live training session name**<br/>by **Instructor**

Live training sessions are designed to mimic the flow of how a real data scientist would address a problem or a task. As such, a session needs to have some “narrative” where learners are achieving stated learning objectives in the form of a real-life data science task or project. For example, a data visualization live session could be around analyzing a dataset and creating a report with a specific business objective in mind _(ex: analyzing and visualizing churn)_, a data cleaning live session could be about preparing a dataset for analysis etc ... 

As part of the 'Live training Spec' process, you will need to complete the following tasks:

Edit this README by filling in the information for steps 1 - 4.

## Step 1: Foundations 

This part of the 'Live training Spec' process is designed to help guide you through session design by having you think through several key questions. Please make sure to delete the examples provided here for you.

### A. What problem(s) will students learn how to solve? (minimum of 5 problems)

> _Here's an example from the Python for Spreadsheeets Users live session_
>
> - Key considerations to take in when transitioning from spreadsheets to Python.
> - The Data Scientist mindset and keys to success in transitioning to Python.
> - How to import `.xlsx` and `.csv` files into Python using `pandas`.
> - How to filter a DataFrame using `pandas`.
> - How to create new columns out of your DataFrame for more interesting features.
> - Perform exploratory analysis of a DataFrame in `pandas`.
> - How to clean a DataFrame using `pandas` to make it ready for analysis.
> - Apply common spreadsheets operations such as pivot tables and vlookups in Python using `pandas`.
> - Create simple, interesting visualizations using `matplotlib`.


### B. What technologies, packages, or functions will students use? Please be exhaustive.

> - pandas
> - matplotlib
> - seaborn

### C. What terms or jargon will you define?

_Whether during your opening and closing talk or your live training, you might have to define some terms and jargon to walk students through a problem you’re solving. Intuitive explanations using analogies are encouraged._

> _Here's an example from the [Python for Spreadsheeets Users live session](https://www.datacamp.com/resources/webinars/live-training-python-for-spreadsheet-users)._
> 
> - Packages: Packages are pieces of software we can import to Python. Similar to how we download, install Excel on MacOs, we import pandas on Python. (You can find it at minute 6:30)

### D. What mistakes or misconceptions do you expect? 

_To help minimize the amount of Q&As and make your live training re-usable, list out some mistakes and misconceptions you think students might encounter along the way._

> _Here's an example from the [Data Visualization in Python live session](https://www.datacamp.com/resources/webinars/data-visualization-in-python)_
> 
> - Anatomy of a matplotlib figure: When calling a matplotlib plot, a figure, axes and plot is being created behind the background. (You can find it at minute 11)
> - As long as you do understand how plots work behind the scenes, you don't need to memorize syntax to customize your plot. 

### E. What datasets will you use? 

Live training sessions are designed to walk students through something closer to a real-life data science workflow. Accordingly, the dataset needs to accommodate that user experience. 
As a rule of thumb, your dataset should always answer yes to the following question: 
> Is the dataset/problem I’m working on, something an industry data scientist/analyst could work on? 

Check our [datasets to avoid](https://instructor-support.datacamp.com/en/articles/2360699-datasets-to-avoid) list. 

## Step 2: Who is this session for?

Terms like "beginner" and "expert" mean different things to different people, so we use personas to help instructors clarify a live training's audience. When designing a specific live training, instructors should explain how it will or won't help these people, and what extra skills or prerequisite knowledge they are assuming their students have above and beyond what's included in the persona.

- [ ] Please select the roles and industries that align with your live training. 
- [ ] Include an explanation describing your reasoning and any other relevant information. 

### What roles would this live training be suitable for?

*Check all that apply.*

- [ ] Data Consumer
- [ ] Leader 
- [ ] Data Analyst
- [ ] Citizen Data Scientist
- [ ] Data Scientist
- [ ] Data Engineer
- [ ] Database Administrator
- [ ] Statistician
- [ ] Machine Learning Scientist
- [ ] Programmer
- [ ] Other (please describe)

### What industries would this apply to?

*List one or more industries that the content would be appropriate for.*


### What level of expertise should learners have before beginning the live training?

*List three or more examples of skills that you expect learners to have before beginning the live training*

> - Can draw common plot types (scatter, bar, histogram) using matplotlib and interpret them
> - Can run a linear regression, use it to make predictions, and interpret the coefficients.
> - Can calculate grouped summary statistics using SELECT queries with GROUP BY clauses.


## Step 3: Prerequisites

List any prerequisite courses you think your live training could use from. This could be the live session’s companion course or a course you think students should take before the session. Prerequisites act as a guiding principle for your session and will set the topic framework, but you do not have to limit yourself in the live session to the syntax used in the prerequisite courses.


## Step 4: Session Outline

A live training session usually begins with an introductory presentation, followed by the live training itself, and an ending presentation. Your live session is expected to be around 2h30m-3h long (including Q&A) with a hard-limit at 3h30m. You can check out our live training content guidelines [here](_LINK_). 


> _Example from [Python for Spreadsheet Users](https://www.datacamp.com/resources/webinars/live-training-python-for-spreadsheet-users)_
>
> ### Introduction Slides 
> - Introduction to the webinar and instructor (led by DataCamp TA)
> - Introduction to the topics
>   - Discuss need to become data fluent
>   - Define data fluency
>   - Discuss how learning Python fits into that and go over session outline
>   - Set expectations about Q&A
>
> ### Live Training
> #### Exploratory Data Analysis
> - Import data and print header of DataFrame `pd.read_excel()`, `.head()`
> - Glimpse at the data to
>   - Get column types using `.dtypes`
>   - Use `.describe()`, `.info()`
> - **Q&A** 
> #### Data Cleaning and making it ready for analysis
> - Convert date columns to datetime `pd.to_datetime()`
> - Change column names
> - Extract year, month from datetime `.strftime()`
> - Drop an irrelevant column `.drop()`
> - Fill missing values with `.fillna()`
> #### Creating a report
> - First report question: What is our overall sales performance this year? `.groupby()`, `.plt.plot()`
> - Second report question: What is our overall sales performance this year? `.merge()`, `.groupby()`, `plt.plot()`
> - Third report question: What is our overall sales performance this year? `.merge()`, `.groupby()`, `plt.plot()`
> - **Q&A**
>
> ### Ending slides
> - Recap of what we learned
> - The data science mindset
> - Call to action and course recommendations

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
