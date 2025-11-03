# Data Visualization

## Assignment 3: Final Project

### Requirements:
- We will finish this class by giving you the chance to use what you have learned in a practical context, by creating data visualizations from raw data.
- Choose a dataset of interest from the [City of Toronto’s Open Data Portal](https://www.toronto.ca/city-government/data-research-maps/open-data/) or [Ontario’s Open Data Catalogue](https://data.ontario.ca/).
- Using Python and one other data visualization software (Excel or free alternative, Tableau Public, any other tool you prefer), create two distinct visualizations from your dataset of choice.

##
#### Dataset chosen for this assignment
- **URL:** https://open.toronto.ca/dataset/polls-conducted-by-the-city/
- **Title:** _Polls conducted by the City_
- **Description:** "The City Clerk's Office is responsible for conducting polls on behalf of City divisions. Polls are conducted to establish the opinions of residents and businesses on various topics covered by a City by-law (Chp190).
Poll engagement is the primary data provided in this set. Daily data updates occur upon the closing and certification of each poll. The collection of data starts from April 1, 2015." (Source: the URL above.)

#### Visualization 1 (using Python)
![Alt text](viz_01_ballots_cast_vs_needed_with_python.png 'Ballots Cast vs. Ballots Needed -- Traffic Calming')

#### Visualization 2 (using Google Sheets)
![Alt text](viz_02_polls_results_versus_years_with_google_sheets.png 'Poll by Result over the Years (2015-2024) -- Traffic Calming')

- For each visualization, describe and justify:
##
    > What software did you use to create your data visualization?
The first visualization is created by coding in Python (using Pandas, Matplotlib, and Seaborn). The second visualization is produced using Google Sheets.

    > Who is your intended audience?
Python visualization: The intended audience of this visualization are primarily the City of Toronto officials who are responsible administring these polls, and who are interested in seeing voter engagement and turnout. They can see what's the turnout for polls that proceeded to a decision versus those that didn't proceed due to lower than required number of ballots cast.

Google Sheets visualization: The intended audience are primarily people concerned with City of Toronto, and who are interested in the outcomes of the various polls conducted by the City for applications that affect people living or working in Toronto.

Both visualizations can also inform other audiences such as city officials,  policy makers, urban planners, etc.

    > What information or message are you trying to convey with your visualization?
Python visualization: This visualization is a scatter plot that shows the number of ballots cast (on y-axis) versus the number of ballots needed to proceed with a poll (on x-axis) for **Traffic Calming** applications polls conducted by the City of Toronto between 1-Apr-2025 to 31-Oct-2025. If a poll has fewer than required ballots cast, then that poll is invalidated. This results in wasted effort and resources.  Of course, futher investigation would be need to identify other factors which could be causing low turnout, such as, particular neighbourhoods, or the time of year when the poll was conducted, the underlying application type, etc. This visualization can serve as a starting point provinding a high-level view of the overall effectiveness of all the polls conducted for a selected application type.

Google Sheets visualization: This is a grouped bar chart showing the poll results (In Favour, Opposed, Low Response) for all the polls for **Traffic Claming** applications over the years 2016 to 2024. It shows that from 2020 (post-Covid) onwards, the number of polls conducted for **Traffic Calming** has been far fewer than in previous years, as most people worked remotely (from home) during this time. It also shows that each year, most polls don't proceed to a decision because of the ballot response not being met.

    > What aspects of design did you consider when making your visualization? How did you apply them? With what elements of your plots?
Python visualization: The choice of scatter plot colour coded by poll outcome to show at a glance voter engagement in polls. The visualization uses color-blind friendly pallette, with clear axis labels, main title, and legend. Girdline and reference line (x=y equality line) are added to help viewers quickly identify which polls met or fell short of rquired ballots.

Google Sheets visualization: A grouped bar chart visualization was selected to compare poll numbers by result over time, showing trends across years. The visualization uses color-blind friendly pallette, with clear axis labels, main title, and legend.

    > How did you ensure that your data visualizations are reproducible? If the tool you used to make your data visualization is not reproducible, how will this impact your data visualization?
Python visualization: The entire end-to-end analysis and visuailzation is reproducible, because each step is documentd, coded in Python (saved as assignment_3_code.ipynb) in a Jupyter notebook. Anybody can simply run the notebook and generate the exact same visualizations each time. Howerver, it is assumsed that the required environment and packages are setup. In any case, the setup for the environment and package requirements and dependencies can also be scripted and reproduced.

Google Sheets visualization: This lacks full reproducibility because tools like Google Sheets or Excel don't track and provide a step by step log of all the steps taken to generate a visualization from raw data. To increase reproducibility documenting (e.g., in a text file) all preprocessing steps would be essential.

    > How did you ensure that your data visualization is accessible?
Both Python and Google Sheets visualizations: Use predefined colour pallette with good contrast and colour-blind friendly hues. The top title and axis-labels are descriptive, and shown in easily readible fonts. Legend is included to guide the viewer. The visualization can be exported into portable formats such as PNG, SVG.

    > Who are the individuals and communities who might be impacted by your visualization?
Both Python and Google Sheets visualizations: The impact is primarily on people who are residents of or work in Toronto, as they are the ones most affected by community polls determinig street level modifications. Additionally, city staff and planners are affected because they rely on voter participation to allocate resoucres and make policy decisions.

    > How did you choose which features of your chosen dataset to include or exclude from your visualization?
Python visualization: After doing some data analysis, it appeared that voter engagement differs significanlty by application type (Front Yark Parking, Boulevard Restaurant, Traffic Calming, Permit Parking, etc.). So, this visualization focuses shows the turnout and engagement (ballots cast vs. ballots required) for a selected application type.

Google Sheets visualization: This considers all the polls for a given application type over the complete years from 2016 - 2024. The polls for 2015 and 2025 were filtered out as they were only partially covered in the dataset.

    > What ‘underwater labour’ contributed to your final data visualization product?
Python visualization: The source data quality was already high (> 90%), but still some data preprocessing was required such as re-ordering columns, converting columns to appropriate data types (datetime, category, etc.).

Google Sheets visualization: The aggregated data for poll results over the years 2014 - 2025 was produced in Python, and a table with the required data was generated as a CSV file, which was then imported and visualized in Google Sheets. In retrospect, this was not a good practice from the point of view of an end user of the Google Sheet / Excel visualization because it significantly reduces data accessiblity, and provides only the limited data necessary for the particular visualization. The preprocessing could've been done in Google Sheets, but then this would have reduced the reproducibility.

- This assignment is intentionally open-ended - you are free to create static or dynamic data visualizations, maps, or whatever form of data visualization you think best communicates your information to your audience of choice!
- Total word count should not exceed **(as a maximum) 1000 words**

### Why am I doing this assignment?:
- This ongoing assignment ensures active participation in the course, and assesses the learning outcomes:
* Create and customize data visualizations from start to finish in Python
* Apply general design principles to create accessible and equitable data visualizations
* Use data visualization to tell a story
- This would be a great project to include in your GitHub Portfolio – put in the effort to make it something worthy of showing prospective employers!

### Rubric:

| Component         | Scoring  | Requirement                                                                 |
|-------------------|----------|-----------------------------------------------------------------------------|
| Data Visualizations | Complete/Incomplete | - Data visualizations are distinct from each other<br>- Data visualizations are clearly identified<br>- Different sources/rationales (text with two images of data, if visualizations are labeled)<br>- High-quality visuals (high resolution and clear data)<br>- Data visualizations follow best practices of accessibility |
| Written Explanations | Complete/Incomplete | - All questions from assignment description are answered for each visualization<br>- Explanations are supported by course content or scholarly sources, where needed |
| Code              | Complete/Incomplete | - All code is included as an appendix with your final submissions<br>- Code is clearly commented and reproducible |

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 11/02/2025`
* The branch name for your repo should be: `assignment-3`
* What to submit for this assignment:
    * A folder/directory containing:
        * This file (assignment_3.md)
        * Two data visualizations
        * Two markdown files for each both visualizations with their written descriptions.
        * Link to your dataset of choice.
        * Complete and commented code as an appendix (for your visualization made with Python, and for the other, if relevant)
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/visualization/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [x] Create a branch called `assignment-3`.
- [x] Ensure that the repository is public.
- [x] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [x] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
