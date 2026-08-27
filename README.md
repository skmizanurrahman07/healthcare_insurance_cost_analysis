<p align="center">
 <img width="100%" src="./images/project-banner.png " align="center" alt="Project banner" />
 <h1 align="center">Health Insurance Cost Analysis</h1>
 <p align="center">Analysing health insurance cost data from Kaggle.</p>
</p>

<p align="center">
  <br/>
  <a href="https://www.python.org/" title="Python official website">
    <img alt="Python Logo" height="30px" src="./images/python-logo.png" />
  </a>
  <a href="https://pandas.pydata.org/" title="Pandas official wesbite">
    <img alt="Pandas Logo" height="30px" src="./images/pandas-logo.png" />
  </a>
   <a href="https://matplotlib.org/stable/" title="Matplotlib offical website">
    <img alt="Matplotlib Logo" height="30px" src="./images/matplotlib-logo.png" />
  </a>
  <a href="https://seaborn.pydata.org/" title="Seaborn offical website">
    <img alt="Seaborn Logo" height="30px" src="./images/seaborn-logo.png" />
  </a>
  <a href="https://plotly.com/python/" title="Plotly offical website">
    <img alt="Plotly Logo" height="30px" src="./images/plotly-logo.png" />
  </a>
  <a href="https://www.kaggle.com/" title="Kaggle offical website">
    <img alt="Kaggle Logo" height="30px" src="./images/kaggle-logo.png" />
  </a>
  <br />
</p>

<p align="center">
  <a href="https://github.com/users/petedanielsmith/projects/2">Project Board</a>
  &nbsp;&nbsp;-&nbsp;&nbsp;
  <a href="./jupyter_notebooks/data_cleanup.ipynb">Data Cleanup</a>
  &nbsp;&nbsp;-&nbsp;&nbsp;
  <a href="./jupyter_notebooks/data_visualisation.ipynb">Data Visualisation</a>
   &nbsp;&nbsp;-&nbsp;&nbsp;
  <a href="#conclusions">Conclusions</a>
  <br/><br/><br/>
</p>

<details>
<summary>Table of contents (Click to show)</summary>

- [Dataset Content](#dataset-content)
- [Business Requirements](#business-requirements)
- [Hypothesis](#hypothesis)
- [Project Plan](#project-plan)
- [The rationale to map the business requirements to the Data Visualisations](#the-rationale-to-map-the-business-requirements-to-the-data-visualisations)
- [Analysis techniques used](#analysis-techniques-used)
- [Ethical considerations](#ethical-considerations)
- [Unfixed Bugs](#unfixed-bugs)
- [Development Roadmap](#development-roadmap)
- [Conclusions](#conclusions)
- [Main Data Analysis Libraries](#main-data-analysis-libraries)
- [Credits](#credits)
  - [Content](#content)
  - [Media](#media)
- [Acknowledgements](#acknowledgements)

</details>

<p>

</p>

<details>
<summary>How to use this repo (Click to show)</summary>

**Make sure you have:**

- Python installed, this project used V3.12,
- VS Code latest

**Inside VS Code:**

Open Extensions (Ctrl+Shift+X or ⇧⌘X on macOS)
Install these extensions if you don't have them:

- Python extension (by Microsoft in the Extensions Marketplace)
- Jupyter extension (also by Microsoft)

**From the terminal:**

Open the folder in a terminal where you want the project to be saved

#### Run git clone:

```
git clone https://github.com/petedanielsmith/HealthcareInsuranceDataAnalyticsProject.git
```

#### Navigate in to the new folder:

```
cd HealthcareInsuranceDataAnalyticsProject
```

#### Setup a virtual enviroment:

Create a virtual enviroment for the project.

Linux / Mac:

```
python3 -m venv .venv
source .venv/bin/activate
```

Windows CMD:

```
python3 -m venv .venv
.venv\Scripts\activate
```

Windows PowerShell:

```
python3 -m venv .venv
.\.venv\Scripts\Activate.ps1
```

#### Install the dependancies:

This will install all the dependancies needed for the project in to the virtual enviroment if it is setup, rather than globally

```
pip install -r requirements.txt
```

#### Select the Kernel

There is a drop down at the top of the notebooks to select your kernal that will run the Python.
If you setup a virtual enviroment then make sure you pick the venv one.

---

</details>

<p>
<br/>
</p>

## Dataset Content

The dataset used in this project can be downloaded from [Kaggle: Healthcare Insurance Dataset](https://www.kaggle.com/datasets/willianoliveiragibin/healthcare-insurance). It contains information on the relationship between personal attributes, geographic factors, and their impact on medical insurance charges

**Columns include:**

- `age` - The insured persons age.
- `sex` - Gender (male or female) of the insured.
- `bmi` - (Body Mass Index): A measure of body fat based on height and weight.
- `children` - The number of dependents covered.
- `smoker` - Whether the insured is a smoker (yes or no).
- `region` - The geographic area of coverage.
- `charges` - The medical insurance costs incurred by the insured person.

## Business Requirements

Analyse healthcare insurance data to understand how personal attributes and geographic factors influence insurance costs.

## Hypothesis

- Smokers have higher insurance charges
- People with higher BMI have higher insurance charges
- Geographic region influences insurance charges
- Sex of a person influences insurance charges
- Including children on an insurance plan increases charges
- Age of a person influences insurance charges

## Project Plan

The prjoject follows the following steps:

1. `Extract` - Extract the data from Kaggle.
2. `Load` - Load the CSV via Pandas.
3. `Transform` - Clean and process the data using Pandas, adding new columns and checking for missing or duplicated values.
4. `Visualise` - Creating charts with Matplotlib, Seaborn and Plotly to visualise trends.
5. `Analyse` - Interpret what the visualisations displayed.
6. `Document` - Record findings and conclusions.

## The rationale to map the business requirements to the Data Visualisations

- Smokers have higher insurance charges
  - Use histogram to show smokers vs overall charge distribution
  - Correlation matrix to show the correlation
  - Violin plots to show the distributions
  - Scatter and 3D scatter charts to show the distribution
  - Box plot to show the distribution
- People with higher BMI have higher insurance charges
  - Correlation matrix to show correlation
  - Violin plot to show the distribution
  - Scatter and 3D scatter to show the distribution
- Geographic region influences insurance charges
  - Violin plot to show the distribution
  - Scatter chart to show the distribution
- Sex of a person influences insurance charges
  - Violin plot to show the distribution
  - Box plot to show the distribution
- Including children on an insurance plan increases charges
  - Bar chart to show the average sales charges
- Age of a person influences insurance charges
  - Correlation matrix to show correlation
  - Violin plot to show the distribution
  - 3D scatter to show the distribution

## Analysis techniques used

1. Methods Used:

   - Descriptive statistics (`.describe()`, `.info()` etc.)

   - Segmentation (used bins for age group and bmi group)

   - Visual analytics (`Matplotlib`, `Seaborn`, `Plotly`)

2. Limitations & Alternatives:

   - Limited data points availble in the csv, other factors could influence the decsion such as medial history etc.

3. Structure Justification:

   - Data cleanup and transform notebook as the first part.

   - Visualisation notebook for the second part.

4. Use of Generative AI:

   - AI supported: GitHub copilot extention was installed and so did speed up some repetative tasks.

## Ethical considerations

- The data was already anonymised and contained no data that could be used to identify an individual so there were no ethical concerns.

## Unfixed Bugs

- No unfixed bugs remaining

## Development Roadmap

Challenges faced:

- Having a separate notebook for clean and visualise meant i had to repeat the categorisation steps once importing the cleaned csv as the csv fileformat I used doesn't persist this data. If doing again I would investigate what other file formats data can be saved out to.
- Creating a shared legend for multi chart plots rather than a repeating legend required ChatGPT to help me.
- Adding layout styles and moving the intial camera on Plotly 3D charts required ChatGPT to help me.
- GitHub static preview of notebooks does not display Plotly chart images so I added a link to the expored chart images.

Next steps:

- Create a feature engineering pipeline to normalise and transform the data.
- Create a predictive model that can predict insurance costs from given parameters.
- Create a full interactive [Plotly Dash](https://dash.plotly.com/) charts app that have filter options that apply across multiple charts at once.

## Conclusions

- Smokers have higher insurance charges
  - Smoking clearly has the biggest effect on charges of all the data points available.
- People with higher BMI have higher insurance charges
  - BMI had less of an effect on the charges than i expected, but did have an effect if the person was obese or severly obese and also a smoker.
- Geographic region influences insurance charges
  - Geographic region didn't affect the charges to any note.
- Sex of a person influences insurance charges
  - Sex didn't affect the charges to any note.
- Including children on an insurance plan increases charges
  - Including children on the plan did have a very small increase. 4 and 5 children plans were coming in a bit lowerbut due to the small number of data points recorded for these values, nothing could be read in to this.
- Age of a person influences insurance charges
  - Age did slowly increase the charges as they got older but wasn't by a huge amount.

Overall smoking was the biggest influence by far on insurance charges, especially if they were obese and severly obese smokers. Charges with age also slowly increased as the people got older. This is all very well displayed in this chart from the visualisation notebook:

![Violin plot of all the distributions](./charts/distribution_of_charges_violin.png)

## Main Data Analysis Libraries

The libraries used for data analysis were:

1. `Pandas` - For data loading, transforming and cleaning.
2. `NumPy` - For data transforming in to categories.
3. `Matplotlib` - For overall multi chart layouts.
4. `Seaborn` - For a lot of the individual charts.
5. `Plotly` - For interactive charts.

## Credits

### Content

- [Code institute](https://codeinstitute.net/) - The intial project structure.
- [Kaggle](https://www.kaggle.com/) - Providing the data set used.
- [NHS website](https://www.nhs.uk/conditions/obesity/) - Providing the BMI category definitions.
- [KFF](https://www.kff.org/affordable-care-act/state-indicator/marketplace-plan-selection-by-age/?currentTimeframe=0&sortModel=%7B%22colId%22:%22Location%22,%22sort%22:%22asc%22%7D) & [State Health Compare](https://statehealthcompare.shadac.org/table/4/health-insurance-coverage-type-by-age#1/5,4,1,10,86,9,8,6,3,12,13,20,25,14,21,22,23,24,11/76/7,8) - Information on insurance age group definitions.
- [ChatGPT](https://chatgpt.com/) - Help getting handles and making a single legend on a multi chart plots and adding layout changes to Plotly charts.
- [SimpleSteps.guide](https://simplesteps.guide/guides/technology/machine-learning-ai) - My notes I recorded from the Code Institute course.

### Media

- [Midjourney AI](https://www.midjourney) - AI Generated banner logo.
- [Code Institute](https://codeinstitute.net/) - Code Institute logo.
- [Python](https://www.python.org/) - Python logo image.
- [Pandas](https://pandas.pydata.org/) - Pandas logo image.
- [Matplotlib](https://matplotlib.org/) - Matplotlib logo image.
- [Seaborn](https://seaborn.pydata.org/) - Seaborn logo image.
- [Plotly](https://plotly.com/python/) - Plotly logo image.
- [Kaggle](https://www.kaggle.com/) - Kaggle logo image.
