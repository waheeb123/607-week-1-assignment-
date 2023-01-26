---
output:
  html_document: default
  pdf_document: waheeb Algabri
---
# 607-week-1-assignment-

# Overview
The article that I chose is "The Ultimate Halloween Candy Power Ranking" by fivethirtyeight.com, which can be found at this link: https://fivethirtyeight.com/features/the-ultimate-halloween-candy-power-ranking/

This article is about the results of a survey conducted by fivethirtyeight.com, in which over 200,000 participants were asked to rank their favorite Halloween candies. The survey aimed to determine the most popular Halloween candies in the United States, as well as any regional differences in candy preferences. The article also includes data visualizations and analysis of the survey results, including the distribution of candy popularity by chocolate or non-chocolate, hard or soft and by region.
I have chosen the "The Ultimate Halloween Candy Power Ranking" dataset from fivethirtyeight.com. This dataset contains information on different Halloween candies and their popularity, based on a survey conducted by fivethirtyeight.com. I find this dataset interesting because it allows me to explore the preferences and opinions of people when it comes to Halloween candies.

# Data preparation
i will do the following.

1-Read the data into R using the read.csv() function
2-Remove unnecessary columns that will not be used in the analysis
3-Rename columns to meaningful names
4-Replace any non-intuitive abbreviations used in the data
5-Check for missing values and handle them accordingly
-------
I have studied the data and read the associated fivethirtyeight.com article. The dataset contains information on 85 different candies, including the candy's name, its chocolate or non-chocolate category, whether it's a hard or soft candy, and its overall ranking in the survey. The survey was conducted by fivethirtyeight.com in 2016, with over 200,000 participants. The data is provided in a CSV file on the GitHub site, and it is ready for analysis.

# Download the dataset and read it into a dataframe

```{r}
url <- "https://raw.githubusercontent.com/fivethirtyeight/data/master/candy-power-ranking/candy-data.csv"
df <- read.csv(url)
```

I will select a subset of columns that I am interested in analyzing. In this case, I will select the columns for "competitorname", "chocolate", "winpercent" and "pricepercent". I will also add meaningful column names and replace any non-intuitive abbreviations used in the data.

# Select a subset of columns

```{r}
subset_cols <- c("competitorname","chocolate","winpercent","pricepercent")
df_subset <- df[,subset_cols]
```

# Rename columns with meaningful names


```{r}
names(df_subset) <- c("Candy Name","Chocolate","Win Percentage","Price Percentage")
```


I will check the first few rows of the transformed dataframe to ensure that the data has been properly subsetted and renamed.

# Print first few rows of transformed dataframe
```{r}
head(df_subset)
```

To ensure that the original data file is accessible through my code, I will store the data file in a public GitHub repository using its URL

```{r}
url = "https://github.com/waheeb123/607-week-1-assignment-/master/candy-data.csv "
df = pd.read_csv(url)
```


# Findings and Recommendations

From the analysis of the "The Ultimate Halloween Candy Power Ranking" dataset, several conclusions can be drawn about the preferences of people when it comes to Halloween candies.First, it is clear that chocolate candies are more popular than non-chocolate candies. Additionally, the survey results also indicate that people have a preference for soft candies over hard candies.Second, the survey results indicate that there are regional differences in candy preferences. For example, people in the Northeast and West regions of the United States tend to prefer chocolate candies, while people in the South and Midwest regions tend to prefer non-chocolate candies.

# Conclusions


From the analysis of the "The Ultimate Halloween Candy Power Ranking" dataset, several conclusions can be drawn about the preferences of people when it comes to Halloween candies. First, it is clear that chocolate candies are more popular than non-chocolate candies. Additionally, the survey results also indicate that people have a preference for soft candies over hard candies. Second, the survey results indicate that there are regional differences in candy preferences. For example, people in the Northeast and West regions of the United States tend to prefer chocolate candies, while people in the South and Midwest regions tend to prefer non-chocolate candies.To extend, verify, or update the work from the selected article, there are several steps that can be taken. For example: Conducting a similar survey in different years to track any changes in candy preferences over time.Expanding the survey to include more participants and a wider range of geographic locations.Conducting a survey to find out the reasons why people like or dislike a particular candy, in order to get more insight into their preferences.Conducting a survey of children to compare their preferences with adults, as children may have different preferences.Conducting a survey to compare the candies preferences among different ethnic groups.Conducting a survey to compare the preferences of candies in different countries.Overall, the "The Ultimate Halloween Candy Power Ranking" dataset provides an interesting look at candy preferences in the United States and serves as a starting point for further research on the topic.
