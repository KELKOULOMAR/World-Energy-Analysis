# World-Energy-Analysis

In this project we answered some question in order to understand well the energy distribution in some world countries. 

### Step 1:

First we load the energy data, which is a list of indicators of [energy supply and renewable electricity production] from the [United Nations](http://unstats.un.org/unsd/environment/excel_file_tables/2013/Energy%20Indicators.xls) for the year 2013, and we put into a DataFrame with the variable name of **Energy**.


Then we Convert `Energy Supply` to gigajoules (**Note: there are 1,000,000 gigajoules in a petajoule**).

Finally, we load the [Sciamgo Journal and Country Rank data for Energy Engineering and Power Technology](http://www.scimagojr.com/countryrank.php?category=2102) , which ranks countries based on their journal contributions in the aforementioned area.

We join the three datasets: GDP, Energy, and ScimEn into a new dataset (using the intersection of country names). We use only the last 10 years (2006-2015) of GDP data and only the top 15 countries by Scimagojr 'Rank' (Rank 1 through 15). 

### Step 2:
What are the top 15 countries for average GDP over the last 10 years?

### Step 3:
By how much had the GDP changed over the 10 year span for the country with the 6th largest average GDP?

### Step 4:
What is the mean energy supply per capita?

### Step 5:
What country has the maximum % Renewable and what is the percentage?

### Step 6:
What is the maximum value of the ratio of Self-Citations to Total Citations, and what country has the highest ratio?

### Step 7:
After estimating the population using Energy Supply and Energy Supply per capita. 
What is the third most populous country according to this estimate?

### Step 8:
What is the correlation between the number of citable documents per capita and the energy supply per capita?

### Step 9:
We create a new column with a 1 if the country's % Renewable value is at or above the median for all countries in the top 15, and a 0 if the country's % Renewable value is below the median.

### Step 10:
We group the Countries by Continent, then create a DataFrame that displays the sample size (the number of countries in each continent bin), and the sum, mean, and std deviation for the estimated population of each country.

### Step 11:
We cut % Renewable into 5 bins. We group Top15 by the Continent, as well as these new % Renewable bins. How many countries are in each of these groups?

### Step 12:
We convert the Population Estimate series to a string with thousands separator (using commas). We use all significant digits.



