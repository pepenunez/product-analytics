# Data analytics for Product Management

**GitHub repo:** https://github.com/pepenunez/project-4

**Time frame** for the project: 1-week

## File structure

- **/data**:
  - **clean-data**:
    - **sub-categories**: This folder contains a .csv per each sub-category that we will be analysing.
    - **categories-post.csv**: Category, Sub-category, Keyword,Search Vol (min), Search Vol (max), Number of templates
    - **categories-post.xlsx**: same as categories-post.csv but in excel format.
    - **priotities.csv**: Sub-category, Search Vol, Recommended templates, Number of templates, Templates to create
    - **trends-all.csv**: Date, Trend, Category, Sub-category, Keyword,Search Vol (min), Search Vol (max), Number of templates, Search Vol (avge), Search Vol, isPartial, index
  - **temp-data**:
    - **canva.txt**: https://www.canva.com/create-a-design html in txt format
    - **categories-pre.csv**: Category, Sub-category, Keyword
- **/presentation-resources**: This folder contains some of the resources that I've used for the presentation.

- **01_data-gathering.ipynb**: The goal of this notebook is to gather, clean and manipulate all the data that we will be using during the project.
- **02_data-analysis.ipynb**: The goal of this notebook is to explore the data, identify interesting insights and perform the analysis.
- **presentation.pdf**: This is the presentation with the approach, main takeaways and recommendations.
- **tableau**: The goal is to visualize the analysis performed. There are some graphs that are not in any other place. 

## Introduction

For this project I wanted to see validate that data can have a direct impact on product management and product decisions. To do so, I choose a digital product that I regularly use, know and that I could think of a potential challenge that they could have in order to do my project. I decided to choose www.canva.com. Canva creates unique templates that users can use and adapt. After doing some research I've found out that they have +100 sub-categories with a total of +60.000 templates. With this project, I wanted to do an analysis that could help Canva's template team to priotitise, adapt to the upcoming trends and improve user engagement.

## Initial hypothesis

1. Is there a correlation between Search Volume (google) and the Number of templates that Canva is offering?
2. Are categories displayed in Canva's website sorted by Search Volume (google)?

## Assumptions

- I do not have access to Canva's data, so I will use Google's search trends data and assume that it can be transferred to Canva's users interests.
- User engagement increases with greater available templates. 

## Data sources

1. www.canva.com
2. Google trends (API) | Google trends - pytrend | pyp|  https://pypi.org/project/pytrends/#interest-over-time
3. Google Adwords | Google Adwors - googleads | conda | https://github.com/googleads/googleads-python-lib

## Main findings

There is a moderate positive correlation between the Search Volume (google) and the Number of templates. The model can explain 35% of the variance of the Number of templates. It is recommended to analyse which are the other factors that are influencing to the correlation. 

![linear regression](http://url/to/img.png)


## Recommendations

- Prioritise and Analyse in-depth the subcategories in 'priorities.cvs'.  
- A/B test displaying category by Search Volume (https://www.canva.com/create-a-design)
- Adapt priorities and displays to seasonality 

## Next steps | Further analysis

- Classify actual sub-categories by growth phase so we could visually detect which are the categories where we should be prioritising.
- Spot new trends by searching for similar keywords  

## Particularities

- There where some keywords that didnt have trend info.

## Goals and Requirements for the project
The **goal** of this project is to practice creating and interpreting different types of visualizations using real world data as well as statistical analysis.

The **technical requirements** for this project are as follows:

- Select a dataset or multiple dataset from a public source.
- Create Jupyter notebooks to analyze the data
- Using your data, create a minimum of 4 types of plots (ie: scatter plot, histogram, box plot and bar graph).
- Explain what insight or information is inferred from these visualizations.

