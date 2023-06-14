# lifeexp-who-analysis
Life Expectancy Analysis for WHO data set

The World Health Organization (WHOGlobal )'s Health Observatory (GHO) data repository monitors each nation's health status as well as a number of other relevant variables. The WHO data repository website was used to acquire the data set pertaining to life expectancy, health factors for 193 nations, and its corresponding economic data was obtained from the United Nations website.

WHO considers various other factors that effect or which are critical for computation of the Life expectancy rate. The dataset that we have finalised comes directly from the official WHO website which is accurate and upto date. The dataset includes various factors such as Schooling duration, Infant mortality, Alcohol consumption and various other factors. The benefit of this assignment is that since WHO provides the data, you will learn about the variables they consider when determining a country's Life Expectancy.

## Data Dictionary

Country: Country
Year: Year considered
Status: If the country is developed or Developing
Life expectancy: It displays the average life expectancy of the country in that particular year
Adult Mortality: Adult Mortality Rates of both sexes (probability of dying between 15 and 60 years per 1000 population)
infant deaths: Number of Infant Deaths per 1000 population
Alcohol: Alcohol, recorded per capita (15+) consumption (in litres of pure alcohol)
percentage expenditure: The amount spent on health in relation to the GDP per capita(%)
Hepatitis B: Hepatitis B (HepB) immunization coverage among 1-year-olds (%)
Measles: It shows the number of Measles cases reported per 1000 population
BMI: Average Body Mass Index of entire population
under-five deaths: Number of under-five deaths per 1000 population
Polio: Polio (Pol3) immunization coverage among 1-year-olds (%)
Total expenditure: General government expenditure on health as a percentage of total government expenditure (%)
Diphtheria: Immunization rate for DTP3 (diphtheria, tetanus, and pertussis) among one-year-olds
HIV/AIDS: Deaths per 1 000 live births of HIV/AIDS (0-4 years)
GDP: Gross Domestic Product per capita (in USD)
Population: It shows the population of the country
Income composition of resources: It shows the Human Development Index based on the income composition of resources whose index ranges from 0 to 1)
Schooling: Average number of years in schooling spent by individuals in that particular country.
We have considered to take immunization and GDP as these factors have a relationship with life expectancy rate.

## Project Aim and Objectives
Governments and world leaders are in charge of bettering the lives of their citizens. Government officials create laws and policies that have an impact on people's quality of life. The development of effective laws takes planning and requires research. Understanding what increases a population's lifespan is an essential move to start these inquiries. To fulfil this need, our project will demonstrate the variables or factors that are considered and have an impact on a person's life expectancy. Our reports can also look at the variables or circumstances that indicate or foretell a population's unfavourable effects. Predictions of the Life Expectancy of the Selected Region are now more prominent in demand by the Governmental Bodies and the Private Bodies and their Policy-Making With the advancement in new systematic, accurate, efficient, and result-oriented techniques in the field of Data Science.

The data that we use is being classified into 4 categories: 
1) Social factors: Social factors such as Alcohol consumption, schooling etc
2)Economic factors: Such as GDP, Income composition
3)Mortality: Adult mortality rates of both sexes
4)Immunization

The outcome variable which will be examined is life expectancy.

Inorder to find the relation between the variables we used or constructed a heat Map that will indicate the amount of corelation or how much of that particular factor is showing a positive impact on Life expectancy rate.

## Specific Objective(s)
Listed below are the specific objectives that we decided to analyse and learn more about

1)Analysation of life Expectancy of all the Countries in the period 2000-2015

When examined has the life expectancy of all the countries together increased/ decreased from the start of 2000 – 2015? Justify why has it increased/reduced

2)Schooling's impact on Life expectancy

Do you believe that the teaching of a healthy lifestyle in schools is having an impact on the life expectancy rate?

3)Developed vs Developing nations

When compared and analysed which among them have a higher average life expectancy rate(Developing vs Developed)? Justification of the result

4) Linear Regression on Schooling vs Life expectancy and HDI vs Life expectancy rate.

Upon analysing explain what measures the government should take to increase their country's overall life expectancy rate?

## Architecture

<img width="133" alt="image" src="https://github.com/bochiwalritik/lifeexp-who-analysis/assets/79448462/32df2f4c-4725-454f-bd5a-cc45af53d1d0">

At first we retrieved the life expectancy dataset from the WHO website called GHO Data. Then, the data was processed and cleaned using pandas and excel. Then, the data was classified into different groups to perform cluster analysis. Next, A Heat map was created to find corelation between different parameters within our dataset and life expectancy. Then the data was visualised using Matplot libraries inorder to get a broader picture of the dataset. Finally the dataset was divided into training and testing set and our model was generated, and we can conclude that factors like schooling duration and Adult mortality has a greater impact on Overall life expectancy.

## Processing Modules and Algorithms
Heat map Construction: We started investigating the life expectancy data set with the Pearson Coefficient Correlation matrix in order to better understand the variables in the dataset. We used this to obtain a sense of the stronger correlations between our variables so that we could start our study from there. The correlation number will be close to +1 or —1 if there is a strong link between two attributes. The heatmap highlights some noteworthy findings, such as the positive correlation of 0.86 between education and the income mix of resources. This suggests that the relationship is relatively linear. Education therefore, increases together with the income composition of resources. Additionally, life expectancy in education has a significant linear association. The strong negative correlation between life expectancy and HIV/AIDS suggests that as life expectancy increases, HIV/AIDS declines.

### Outliers:

Outliers can skew data, which can have an impact on the results. So, we search for anomalies. However, we will only exclude outliers for the sake of valid data. For instance, it is feasible that a country has an abnormally high population, but we should still ignore it and remove it from our dataset.

### Linear regression:

Linear Regression is the most basic form of regression method. The dependent variable in this technique is continuous in nature. It is expected that the dependent variable and independent variables have a linear relationship. We have performed simple linear regression which uses only one dependent and one independent variable.

It performs a regression task. Regression models a target prediction value based on independent variables. It is mostly used for finding out the relationship between variables and forecasting. We plotted the number of schooling years across the life expectancy. There is clearly a linear upward trend i.e more the number of years of schooling, higher will be the average life expectancy. We have fit a linear model represented by the red line

## Project Outcome

### Overview

Our project used various visualisation and cleaning techniques to analyse the WHO Life expectancy dataset which consisted of 2938 rows and 22 columns. Our findings show that there are certain parameters which have a direct or indirect impact on Life Expectancy. Some of the major parameters which had a direct link with life expectancy rate are Schooling duration and Indirect link such as Adult mortality, AIDS as seen in our visualisations. 

### Objective 1

1)Analysation of life Expectancy of all the Countries in the period 2000-2015.

After analysis and operation, we found out that the Average life expectancy of the countries has increased. In the year 2000 the average life expectancy was 66.5 years, whereas in 2015 it rose sharply to 71.6 by 5.1 years. This shows a significant improvement in the countries' life expectancy rate.
The increase in the life expectancy rate was possible only due to the collective rise in Schooling duration of the individuals, Total expenditure or spending of the government on healthcare systems, GDP, Income Composition and immunisation. The collaborative efforts of government bodies on healthcare systems and facilities have paved the way for medical institutions to provide quality treatment to patients with the help of sophisticated healthcare machinery and tools. Additionally, there was a significant increase in the average number of years that people spent on their education, which increased their capability to land a promising career and be financially stable to maintain a healthy lifestyle. 

<img width="673" alt="image" src="https://github.com/bochiwalritik/lifeexp-who-analysis/assets/79448462/9a5d34f9-a82f-4ff2-bad0-7f2149e4fa8f">

### Objective 2

2)Schooling's Impact on Life expectancy

From the analysis and operation of data, we can clearly see that the countries with children who undergo schooling for a longer duration have a higher life expectancy than the countries which do not. 
This isa because school education provides the basic knowledge of a healthy lifestyle and the care to be taken right from the beginning of their lives. It induces a sense of responsibility in the child or student to take care of their health and avoid unhealthy eating and drinking habits.
Further or higher education is also essential for a child as this helps them to attain their career goals so that they can be financially stable to be able to get nutritious food, live in a well-built house, and invest in good medical care and services. People with higher edcation use their knowledge, facts, and previous experiences to eliminate health-related risk factors and practice health-improving habits including quitting smoking, drinking alcohol, and exercising frequently.
Countries such as Congo, Finland, Australia, and the Netherlands, which have people with an average schooling duration of Eighteen and Seventeen years, respectively, have a higher life expectancy. It is because when a child advances or gets promoted to higher levels of education, they will learn or be taught more complex or advanced research on the healthcare system and why it works the way it works. It helps students understand the human body's basic working and care for their body and health independently.
There is a good relationship between an individual's mortality rate and the educational duration because a country with a proportion of individuals with a good schooling duration will automatically reduce the proportion of individuals with a low schooling duration, consequently increasing the overall health of the population and life expectancy. 

<img width="670" alt="image" src="https://github.com/bochiwalritik/lifeexp-who-analysis/assets/79448462/0601fca8-4877-48dd-b8ca-fa74eca6e356">
### Objective 3

Although the average human life expectancy has improved worldwide, there is still a significant difference in average life expectancies between various countries.
After examining a nation's condition and life expectancy. The average life expectancy for the "Developed" column is 79 years. The average lifespan in emerging nations is 67 years. The findings show a 12-year increase in the life expectancy in developed nations. Developing countries could not spend more on the healthcare systems than the Total expenditure on healthcare systems by the developed countries.
The most serious development challenge our world currently faces is healthcare. Infectious disease outbreaks and other avoidable health problems are crippling nations all over the world. They must initially attend to their inhabitants' more urgent, immediate demands, which prevents them from focusing entirely on other development issues like education and economic sustainability. Without greater access to and availability of healthcare, global progress and the goal of international development will not be achievable.

<img width="748" alt="image" src="https://github.com/bochiwalritik/lifeexp-who-analysis/assets/79448462/9554667b-cf06-4991-95a2-dc35b6c7fb45">

### Objective 4 

Linear regression
A linear regression model, which identifies the best-fit linear line between the independent and dependent variables, can ascertain the linear relationship between the dependent and independent variables.
In our case, it determines the relationship between life expectancy and education. We plotted the number of years spent in education versus the typical lifetime. There is undeniably an increasing linear trend, which means that the average life expectancy will rise as more years are spent in school. The red line shows the fit of a linear model. 
When examining life expectancy and the effects of pandemics over the course of a lifetime, WHO heavily depends on algorithms like the linear regression model.
Here we used simple linear regression model whih contains only one dependent and one independent variable. In our linear regression model, the x axis, which is the Schooling duration, is a dependent variable, and the Y-axis which is the Life expectancy, is the Independent variable. We can clearly see from the figure that schooling duration is strongly related to Life expectancy.
Additionally with the help of linear regression, we discovered that HDI(Human Development Index) has a positive impact on Life expectancy rate that means change life expectancy is directly proportional to change in HDI. This concludes that the official Government bodies should consider HDI and schooling to be an integral part in their overall country's growth not only in terms of Life expectancy but overall Nation's growth.

<img width="744" alt="image" src="https://github.com/bochiwalritik/lifeexp-who-analysis/assets/79448462/9edd9b0e-bd2f-40c0-9ca6-3591e5a89755">

## Conclusion 

### Achievements

Our project successfully found out the life expectancy trend and factors affecting it. With the help of the pearson coefficient matrix we were able to identify the positively and negatively impacting factors on Life expectancy rate. For example from our analysis and operations on the dataset we found out that Schooling, Total expenditure etc and factors such as adult mortality, AIDS and population have negative relationship. This helps the medical and official bodies to better understand the reasons behind the change in life expectancy and take measures to improve it more. 

### Limitations

The globe has experienced a lot since 2015, and we were unable to work on the data beyond that year. Many nations were severely impacted by the COVID 19 epidemic in 2020 and the year after that. These impacts are still being felt today. The manufacturing of pharmaceuticals and the operation of healthcare institutions have undergone several modifications, as well as the addition of numerous rules and regulations. Because of COVID 19, many countries saw high death rates, particularly among senior citizens aged over 50. We are unsure if the life expectancy rate was affected by these extra parameters which were introduced and will only be known if the dataset is worked on after 2015.

### Future Work

As discussed in the limitations we would like to work on the dataset after 2015 and merge it with our current dataset and update the values in every parameter and add more factors if needed. This will help us to better understand not only the life expectancy rate of the countries but also how each country was affected by the pandemic interms of education, healthcare and socio economic factors.
