# Pisa2012 Data Exporation

## by David Owino

## Project Overview

This project has two parts that demonstrate the importance and value of data visualization techniques in the data analysis process.

- Part I, **Exploratory data visualization**, I will use Python visualization libraries to systematically explore the pisa2012 dataset, starting from plots of single variables and building up to plots of multiple variables.

- Part II, **Explanatory data visualization**, I will produce a short presentation that illustrates interesting properties, trends, and relationships discovered in the dataset by transforming your exploratory visualizations from the first part into polished, explanatory visualizations.

## What do I need to install?

- Anaconda distribution to install Python, since the distribution includes all necessary Python libraries as well as Jupyter Notebooks. 
- NumPy
- pandas
- Matplotlib
- Seaborn

## Why this project?

Data visualization is an important skill that is used in many parts of the data analysis process.

Exploratory data visualization occurs during and after the data wrangling process and is the main method that is used to understand the patterns and relationships present in the data. This understanding helps in statistical analysis, building conclusions, and findings. During this process, additional data cleaning will still be performed.

Explanatory data visualization techniques are used after generating findings and are used to help communicate results to others. Besides producing good visualizations, this project will also help me be a good consumer of visualizations.


## Part 1 - Exploratory Data Analysis

In this part, I will conduct an exploratory data analysis on the pisa2012 dataset using Python data science and data visualization libraries to explore the dataset’s variables and understand the data’s structure, oddities, patterns, and relationships. The analysis in this case is structured, going from simple univariate relationships to multivariate relationships.

I will begin with preliminary data wrangling to understand the data structure and brainstorm some more questions and record which features are of interest to the investigation and those which will help support that investigation. I will adopt the _Question-Visualization-Observations_ framework, which involves asking a question from the data, creating a visualization to find answers, and then recording observations and systematically follow Univariate, Bivariate, and Multivariate Data Exploration.

## Part 2 - Explanatory Data Visualization

This involves updating the README file, summarising the steps used in data exploration and writing the key Insights for Presentation. Two methods are used in this case; 

- **Generating Explanatory Data Visualizations** I will generate explanatory data visualizations to tell a story about the data explored. 
- **Creating Slide Deck** by converting the notebook file.

## Dataset

The data, which is a csv file is contained in a compressed zip file. The csv file is 2.75GB when extracted. It contains data from 485490 sampled students with 636 features. The dataset contains the results from mathematics, science, readings, and financial literacy examinations as well as students' age, country of residence, family possessions, school, and home ICT facilities, first language, education level of the father and mother, occupations, and students' interests and motivations. The dataset can be found in the Udacity servers [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip), with feature documentation available [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisadict2012.csv). Feature documentation, named pisadict2012.csv is 35.4kB containing 636 coded column names and their descriptions.

International Student Assessment (PISA) is a program initiated by OECD member states to measure how well 15-year-old students at the end of their compulsory schooling are prepared to meet today’s challenges affecting societies. The assessment, which takes place after every three years only focuses on the student's ability to use the skills and knowledge acquired at school to solve real-life challenges. PISA is an age-based survey, assessing 15-year-old students in school in grade 7 or higher. About 510,000 students in 65 economies took part in the PISA 2012 assessment of reading, mathematics, science, and financial literacy representing about 28 million 15-year-olds globally. The database also includes students' responses to Questionnaires that they completed as part of the assessment. Of those economies, 44 took part in an assessment of creative problem solving and 18 in an assessment of financial literacy.[here](https://www.oecd.org/pisa/pisaproducts/PISA-2012-technical-report-final.pdf)


## Summary of Findings

The project investigates how different factors influence performance among students in different regions, which are either members of OECD or Non-OECD. In the exploration, I found that there was a strong linear relationship between student scores and social, economic, and cultural status. This relationship was investigated using only countries in the transcontinental region, which are members of OECD. Moreover, further exploration through multivariate visualization reveals that the the choice of a school play into academic performance as such students scores are high in schools with desktop computer, which are used by students. It is also observed that in grade 12, students who access or are in schools with desktop computers but don't use them have the lowest scores as compared to the performance of students who are in schools with no desktop computers. The score for students who use school computers has remained high in all the grades.

Other interesting results I found using the same logarithmic transform of the score is that perseverance has a slight effect on student performance among countries in Northern Europe while home possessions have a positive impact on student performance among OECD countries in Western Europe. In addition, teacher-student relations and student sense of belonging to school also influence students' scores in certain regions. This is because, a lot of data tend to concentrate from zero to 1, which may suggest that positive relations between students and teachers, as well as teachers' support, have a positive impact on student scores. However, it is important to note that, there is no significant difference in performance among females and males as well as between OECD and non-OECD.

Outside of the main variables of interest, I verified the relationship between parental educational level and student performance, which indicated that students who scored high have parents who attained either post-secondary or post-graduate education. It is also significant to note that in the case of gender, about 33 percent of female students access and use desktop computers at school compared to 32 percent of male students. In addition, whereas the median performance is the same in both OECD and Non-OECD countries, many students scored between 25% and 75% scores in non-OECD than in OECD countries. Comparing home possessions and parent level of education, it is clear from the visualization that a lower education level implies a low score for home possession.


## Key Insights for Presentation

At first, I introduce the distribution of scores on a histogram plot followed by a box plot for other numeric attributes that affect scores. These attributes include perseverance, student sense of belonging to a school, ICT usage at school, teacher-student relations, teacher support, social, economic, and cultural status index, and home possessions. 

I then introduce counts for the parent level of education using a donut chart for the father's education and waffle counts for the mother's education level. I also create a bar plot for the percentage proportion of students who took the Pisa test per grade and then I compare the counts for home and school desktop computer usage on a heatmap followed by the scatterplot pattern for numeric attributes that affect student scores in different regions.
 
Afterward, I introduce the performance of each of the categorical variables one by one and pairwise. To start, I use the bar plots for gender, OECD, and country performance. I then use a point plot to compare if there are any variations in performance between gender and grade, and between grade and school computer usage. I also examine whether perseverance, teacher-student relations, and a sense of belonging to school affect gender scores using hist2d and lmplot, and finally whether parent level of education influences student scores. I've made sure to use different color palettes for each quality variable to make sure it is clear that they're different between plots.

## Socio-Economic and Social status index vs. Performance

![image](https://user-images.githubusercontent.com/7541585/193127426-dc8c5f46-971f-44ef-a5b7-b4601b4d7769.png)

## Home possessions vs. Score

![image](https://user-images.githubusercontent.com/7541585/193128370-77da5824-6187-4e5f-85de-f7de65c2acbf.png)

## What I have learnt?

I am able to:

- Supplement statistics with visualizations to build understanding of data.
- Choose appropriate plots, limits, transformations, and aesthetics to explore a dataset, allowing you to understand distributions of variables and relationships between features.
- Use design principles to create effective visualizations for communicating findings to an audience.
