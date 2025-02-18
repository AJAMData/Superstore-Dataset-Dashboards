# Superstore Dataset Looker (Not Studio) Dashboard


## Overview

Having recently left my role as a Senior Data Analyst at Feefo I was given permission to use our Looker instance to create a portfolio dashboard project. Having used the Superstore dataset when learning Tableau nearly 5 years ago I decided to revisit it. The priority here has been to evidence my understanding of the whole Looker ecosystem from modelling to visualisation. 

The scope of this project is very limited, I only had a very short amount of time before losing access to the team's Looker instance. To allow for a quick build the main purpose of this dashboard is to communicate my ability to utilise Views, Explores and Looks for functional dashboards. For speed I have created a 'combined' dimension table, which although not correctly normalised allows me to demonstrate joining a dimension view in the model alongside a simple fact view. 

I would normally ideate the build around a user persona. This would focus on the value to the end user and normally center around a strategic, operational, analytical or tactical design approach. In this instance, again, I have not had time. The visuals are a fairly random mix, chosen to display my skills as a technical developer and not designed from a product perspective. 

Testing has been non-existant due to the rush so I'm confident beyond the nice visuals there will be errors that need correcting. 

![Superstore Pic 1](https://github.com/user-attachments/assets/0185485e-a9fd-4da1-8642-d042a3aece11)


## Data Source

https://www.kaggle.com/datasets/vivek468/superstore-dataset-final

An opensource sample dataset providing transactional retail shopping records.

## Build Process

1. Downloading and inspecting the file. I uploaded the raw .csv file to BigQuery and determined it's size and shape. I carried out basic checks for missing values/nulls, duplicates and the data types.
2. I then decided to split the file into a simple 'combined' dimension table for attributes and a fact table for the transactional records using SQL.
3. Next I mirrored the BQ tables in Looker as views using the import option in the development section and to demonstrate my understanding of dimensions and measures I added new columns and summary fileds to be used as key KPIs, for example the Net Profit Margin. I then joined these tables together in a single model. 
4. Using the explore from the model I then created the dashboard, starting with a bar chart, adding filters and then creating more visuals.
5. Lastly I rearranged the mess to make it slightly more visually appealing and uploaded all relevant files into this repository. 

## Future Improvements

- Introduce an intial ideation stage and design the dashboard based on a hypothetical business need and with specific user personas in mind.
- Complete QA, check all figures are accurate, functionality is correct and document accordingly. 
- Adding a date switching filter between order and ship date as well as a date granularity filter to give access to a date hierarchy of Year > Quarter > Month > Week > Day.
- Add explanatory information buttons.
- Replace the bar charts with a single combined bar and line chart.
- Add the subcategory product filter.
- Visualise sales as the equivalent of turnover; a combination of profit and costs.
- Split the combined dimension table into normalised customer, date, product and geographical dim tables. 











