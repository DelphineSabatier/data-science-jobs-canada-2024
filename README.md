# Data Science Jobs in Canada on Jan 2024
Explore the landscape of Data Science job opportunities in Canada in January 2024. \
The dataset is an export from LinkedIn from Jan 19th 2024. \
Dataset can be found on Kaggle here : [Dataset](https://www.kaggle.com/datasets/kanchana1990/linkedin-canada-data-science-jobs-2024/data)

## Overview of quality of data set 
There are 275 jobs listed. \
Overall quality is quite good! (no duplicates, few missing values except for salary). \
However, 95% of salary values are missing (most linkedin job opportunities usually do not have this information). -> I decided to remove this column. \
4% of contract type, sector, work type are missings -> I decided to drop these rows.

## Roadmap
- [x] Explore the dataset and identify main findings.
- [x] Map all opportunities on a map
- [ ] Shed light on new patterns using external data (such as population density)
- [x] Identify job categories
- [x] Utilize transformers to detect languages in description column and confirm everything is in English
- [ ] Identify the most common skills in description column


## Main findings:
Job opportunities are situated in Ontario and Vancouver area.

### Job opportunities were published from May 23 to Jan 24. 
Most recent is Jan 19th 2024, which is extraction date. \
Average job posting duration 38 days. \
![Job opp publish date](https://github.com/DelphineSabatier/data-science-jobs-canada-2024/assets/146428961/a4fe0fa4-bfde-4966-9c50-00160d86fbe0)

### Mapping the job opportunities on a map: 
The cities were extracted from the location column, and Geopy was used to obtain GPS coordinates. These coordinates were then plotted using Folium, along with a heatmap. \
Main opportunities are located in Ontario region. \
<img width="1000" alt="Canada Map" src="https://github.com/DelphineSabatier/data-science-jobs-canada-2024/assets/146428961/e9f10943-c753-4cf2-b1b2-94d80b28d1cf">

### Sectors recruiting
Top 3 sectors represents 47.5% and Top10 is 77.2% of overall job market. \
![Top10 sectors](https://github.com/DelphineSabatier/data-science-jobs-canada-2024/assets/146428961/88f19bbf-0df5-49e1-b04c-1a076fed82ae)

### Companies recruiting
Top3 companies represents 20.8% and Top10 companies represents 35.9%. \
![Top10 Company hiring](https://github.com/DelphineSabatier/data-science-jobs-canada-2024/assets/146428961/8cb11d96-6a27-43e6-a3b8-ff5b46310d92)

### Experience level 
Mid-senior jobs represents 54.8% of total Canadian market. \
![Job Search Queries by Experience Level](https://github.com/DelphineSabatier/data-science-jobs-canada-2024/assets/146428961/8c7148d4-3ee3-4c66-8608-876a4e5f02fb)

### Contract type
Full-time contract are 88.8%. \
![Job Search Queries by Contract Type](https://github.com/DelphineSabatier/data-science-jobs-canada-2024/assets/146428961/8249a725-8f76-4785-8c56-365624ad2be9)

### Job Categories
5 job categories are defined: Data Science, Machine Learning, NLP, Data Analysis, Engineering. 
Engineering represents 62.0% of total job opportunities. \
![Job opp by Job Category](https://github.com/DelphineSabatier/data-science-jobs-canada-2024/assets/146428961/dec753df-3188-48d5-b5ea-0fd5b7b53bc5)


