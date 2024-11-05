# &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Python---Exploratory-Data-Analysis-on-Spotify-2023-Dataset

### MENDOZA, PAOLO D. &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2ECE-D
####   In this project I will be performing exploratory dataset analysis on data information containing popular tracks on Most Streamed Spotify Songs 2023
####   This project aims to analyze, visualize, and interpret the data so insights can be extracted. 


#### To start this project I downloaded the file that contains the data of the Most Streamed Spotify Songs 2023

#### *importing the libraries that will be used for the entirety of this project.
#### ![image](https://github.com/user-attachments/assets/168dfe8f-b252-409b-8ca0-75c10bdfd4ad)


#### *now loading the file containing the data set. (I used the help of AI to code this part as i was stuck for a while)
#### ![image](https://github.com/user-attachments/assets/ed365032-cea6-4ece-bdb9-e25c48724d98)
#### ![image](https://github.com/user-attachments/assets/4f30aa46-97df-4846-8abc-400c4a87f5a0)
## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; OVERVIEW OF DATASET(GUIDE QUESTIONS)        
#### *How many rows and columns does the dataset contain?
#### To get the number of rows and columns i used the .shape syntax: 
#### ![image](https://github.com/user-attachments/assets/c2adb03c-8505-45e3-8694-52920fdb927a)
#### Output: 
#### ![image](https://github.com/user-attachments/assets/6663194e-b04a-4101-b4cd-9627feea0c3b)
####    As we can see in the photo/while the code is running it shows that it has 953 rows and 24 columns
### **What are the data types of each column? Are there any missing values?
#### Getting the data type of each column i used the .info syntax:
#### ![image](https://github.com/user-attachments/assets/f953378f-3190-4d4c-8566-01c72b53257e)
#### Output: 
#### ![image](https://github.com/user-attachments/assets/f5a45a1f-b7e8-4b80-8f6f-50ae680a5727)
#### Getting/looking for missing/null values:
#### ![image](https://github.com/user-attachments/assets/5664e82a-44a1-4f03-9f48-77a025c8555a)
#### output:
#### ![image](https://github.com/user-attachments/assets/6adf773f-2f39-479a-b789-f9d5caafdf69)
#### We can see in the output the tolal of missing values for each column. It can also be seen using the previous code the .info syntax, but I wanted it to be more organized.
## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Basic Descriptive Statistics
### *What are the mean, median, and standard deviation of the streams column?
#### it took me an ample amount of time to finish this part. I asked AI to help in organizing the output of the code.
#### ![image](https://github.com/user-attachments/assets/fbfc2fd3-3fdb-478a-82e9-4f9e8d447b97)
#### Output:
#### ![image](https://github.com/user-attachments/assets/be72a914-13bf-40a5-b202-0e68789c7d04)
### What is the distribution of released_year and artist_count?
#### The code snippet for this part:
#### For the the distribution of 'released_year'
#### ![image](https://github.com/user-attachments/assets/8558d080-fe1d-4c50-807a-33bd2db2efbc)
#### Output: 
#### ![image](https://github.com/user-attachments/assets/e5610138-4dea-4c19-96cd-351654c96fa5)
#### The histogram shows the distribution of data points across different release years. The x-axis represents the years, while the y-axis indicates the count of entries for each year. From the graph, it's evident that the number of releases has increased significantly in recent years, with a sharp peak around the 2020s. This suggests that most entries in the dataset were released in the 2020s, with relatively few entries in earlier years.
#### For the distribution of 'artist_count':
#### ![image](https://github.com/user-attachments/assets/3d9183a0-adf4-4d2c-a809-9b51a9924b60)
#### Output: 
#### ![image](https://github.com/user-attachments/assets/2f25373f-c0b1-4c6f-9452-e208d90938cd)
#### The histogram reveals a distribution where the majority of entries have an artist count of 1, followed by decreasing frequencies for higher artist counts. This indicates that most entries in the dataset feature a single artist, with far fewer entries having multiple artists. The distribution tapers off sharply, showing very low frequencies for artist counts above 3.


