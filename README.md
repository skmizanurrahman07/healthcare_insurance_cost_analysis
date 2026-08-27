# Healthcare Insurance Cost Analysis Project

This project set out to explore how Data Analytics and AI tools can be use to extract inside information from raw datasets into meaningful insights that utilise for prediction and decesion manking in data driven organisation and for business success. The healthcare Insurance Cost Analysis Project seeks empirically to explore systematic approach to analyse raw datasets and its rationale to identify how different age, gender, habit and health condition affect health insureance cost in various location. In this Jupyter notebook, therefore, performing the steps data cleaning and  data visualisation. 


# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Dataset Content

* Data collected from (https://www.kaggle.com/datasets/willianoliveiragibin/healthcare-insurance?select=insurance.csv)

## Business Requirements

* Identify the factors that affect insurance cost

## Hypothesis and how to validate?

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

* - Smokers have higher insurance charges
  - Use histogram to show smokers vs overall charge distribution
  - Correlation matrix to show the correlation
  - Box plot to show the distribution
- People with higher BMI have higher insurance charges
  - Correlation matrix to show correlation
  - Geographic region influences insurance charges
    - Scatter chart to show the distribution
- Sex of a person influences insurance charges
    - Box plot to show the distribution
- Including children on an insurance plan increases charges
- Age of a person influences insurance charges
  - Correlation matrix to show correlation
  
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
## Ethical considerations (optional)
- The data was already anonymised and contained no data that could be used to identify an individual so there were no ethical concerns.

## Unfixed Bugs

* - No unfixed bugs remaining

## Development Roadmap
Challenges faced: some of image can not be visualize in githubyour project experience? 


## Main Data Analysis Libraries

The libraries used for data analysis were:

1. `Pandas` - For data loading, transforming and cleaning.
2. `NumPy` - For data transforming in to categories.
3. `Matplotlib` - For overall multi chart layouts.
4. `Seaborn` - For a lot of the individual charts.
5. `Plotly` - For interactive charts.

## Credits
- [Code institute](https://codeinstitute.net/) - The intial project structure.
- [Kaggle](https://www.kaggle.com/) - Providing the data set used.
- [NHS website](https://www.nhs.uk/conditions/obesity/) - Providing the BMI category definitions.
- [ChatGPT](https://chatgpt.com/) - Help getting handles and making a single legend on a multi chart plots and adding layout changes to Plotly charts.
- [SimpleSteps.guide](https://simplesteps.guide/guides/technology/machine-learning-ai) - My notes I recorded from the Code Institute course.
- copilot
- code institute students
## Acknowledgements (optional)

* Thank the people who supported this project.
