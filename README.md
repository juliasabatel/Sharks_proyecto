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
We modify the column 'CaseNumber' so that the data appears in date format yyyy/yyyy/yy, eliminating the '/' and changing it to '-'.

🌟 Our target column has been cleaned up by naming all irrelevant countries that were repeated less than 50 times as "Unknown"

🌍 Know which are the countries with more shark deaths

<img width="1066" alt="Captura de Pantalla 2022-11-01 a las 8 41 25" src="https://user-images.githubusercontent.com/29893993/199184218-443e4978-4f65-43ed-bd2a-794443d581f8.png">

🦈 Shark attack deaths by sex

<img width="760" alt="Captura de Pantalla 2022-11-01 a las 8 52 44" src="https://user-images.githubusercontent.com/29893993/199186876-5b9a38b1-6c81-447b-9963-330c8361e7b7.png">


🛳 Types of shark deaths

<img width="998" alt="Captura de Pantalla 2022-11-01 a las 8 53 58" src="https://user-images.githubusercontent.com/29893993/199186855-b27a52a0-f0aa-4c97-ae71-5e7691d1b4c9.png">



🌡 Export and analysis






