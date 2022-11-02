#  Sharks_proyecto

First project carried out on database cleaning. Specifically, it consists of obtaining a main objective, which is to know which country has the highest number of people killed by shark attacks. 
In order to reach this objective, the first step was to clean the selected columns through which more information was extracted, such as the type of death or sex.

# Goals

🧹Clean the dataset 

✂️ Maintain at least 6000 rows 

⚙️ Use of five cleaning techniques

🌍 Know which are the countries with more shark deaths

⛵️ Deaths from shark attacks by type

✨ Shark attack fatalities by gender


# Steps

🔎 Data scanning

The first step has been to explore all the information offered by the database and to order the cleaning steps to be followed. To do this we have studied the shape, number of rows and columns, null values, duplicate values, comparisons, exploration in type of value.

👀 Duplicate deletion

After the null scan we perform the elimination of duplicate values, but before, we establish a comparison between the number of the initial rows and how it would be after eliminating the duplicates to verify that we will keep more than 6000 rows.
In addition, this information is represented in a heat map in which the yellow stripes correspond to the null values that we will deal with in the next step.


<img width="825" alt="Captura de Pantalla 2022-11-01 a las 8 40 04" src="https://user-images.githubusercontent.com/29893993/199183997-d3ddd512-f0cc-4188-a6d0-1d8f2fb7cc56.png">


💣 Deletion of null values

Next, we proceed with the cleaning of the null values. The columns with more than 80% of null values will be eliminated, since they do not provide us with relevant information. The rest of the null values will be renamed as "Unknown" since the quality of the data cannot be guaranteed, but it does not meet the requirements to be eliminated.
The following heat plot shows how the initial graph looks like after eliminating the columns with more than 80% of null cases.

<img width="825" alt="Captura de Pantalla 2022-11-01 a las 8 39 00" src="https://user-images.githubusercontent.com/29893993/199184130-dccf7044-aae0-45d3-9a76-55c310a54c93.png">

🔧 Correction of values

The next step will be the correction of values, including null values. This is done in such a way that, by means of the scanning performed, you see those values to be corrected, starting with the correction of the column names, changing the names, eliminating commas, periods... 
Then the null values are renamed as 'Unknown' (already commented in the previous step). 
We modify the column 'CaseNumber' so that the data appears in date format yyyy/yy/yy, eliminating the '/' and changing it to '-'.

🌟 Type column cleaning

To carry out the cleaning of the Type column, the content of the variables was analyzed by naming three of them as a single variable since they shared the same type of information.

🌟 Country column cleaning

The 'Country' column has been cleaned in depth since it is one of the most important points of the analysis. 
After studying the unique values, we see that there are numerous countries that are not representative for the analysis, these will be renamed as 'Unknown' since only 1.052% of the information would be lost. We do this by establishing that if they are repeated less than 50 times they are called 'Unknown'. 

🌟 Fatal column cleaning

The cleaning of the fatal column has been key to this analysis. With this information we can know the number of attacks that have been fatal and those in which people have survived. In this case our focus is on those people killed by shark attacks.

🌟 Sex column cleaning

The cleaning of the 'Sex' column has been carried out with a procedure similar to that performed for the 'Type' column. Our objective was to clean the values that did not refer to a gender, since in future analyses this information will be needed to analyze it together with the 'Fatal' variable.

🛳 Types of shark deaths

The following graph shows how, based on the variable 'Type', the number of deaths due to shark attacks has been given.

<img width="998" alt="Captura de Pantalla 2022-11-01 a las 8 53 58" src="https://user-images.githubusercontent.com/29893993/199186855-b27a52a0-f0aa-4c97-ae71-5e7691d1b4c9.png">

🌍 Know which are the countries with more shark deaths

Below is the table resulting from the search for our target, the number of shark attack fatalities by country. Clearly it can be seen that the USA is the country with the highest number of fatal attacks.

<img width="1066" alt="Captura de Pantalla 2022-11-01 a las 8 41 25" src="https://user-images.githubusercontent.com/29893993/199184218-443e4978-4f65-43ed-bd2a-794443d581f8.png">

🦈 Shark attack deaths by sex

Finally, through the cleaning performed, it is interesting to see the higher number of shark attack fatalities based on the sex of the victim. The following graph clearly shows how the high number of male cases fail to survive a shark attack.

<img width="760" alt="Captura de Pantalla 2022-11-01 a las 8 52 44" src="https://user-images.githubusercontent.com/29893993/199186876-5b9a38b1-6c81-447b-9963-330c8361e7b7.png">


🌡 Export and analysis

Finally we export the database.

📝 One of the most interesting things about this project is that it is infinite so we will continue cleaning and analyzing tables to have the results as concrete as possible.




