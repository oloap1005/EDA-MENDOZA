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
#### For the noticeable outliers, we shall first compute for the boundaries of the data, then we will define the outliers. and after that we shall plot the data I asked for the help also of ai to write the code and made it explain the codes.:
#### ![image](https://github.com/user-attachments/assets/4ea73afd-8fb6-4b18-9b54-49841fa7a76f)
#### now the code for visualizing the outliers.
#### ![image](https://github.com/user-attachments/assets/7c54d4f1-7a45-4060-8f22-1017cf64fdc1)
#### the output:
#### ![image](https://github.com/user-attachments/assets/e94ba04d-1928-4bd7-9dfe-3ead5a9dc000)
#### This plot illustrates artist count data, highlighting outliers and statistical boundaries. Light blue dots represent individual data points, while red dots indicate outliers—values that lie beyond typical bounds. The green and blue dashed lines mark the first (Q1) and third (Q3) quartiles, showing the spread of the central 50% of the data. The orange and purple dashed lines depict the lower and upper bounds, calculated using the interquartile range (IQR) method, which helps in identifying data points considered as outliers. This visualization provides a clear overview of the data distribution and any anomalies present.

## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Top Performers
#### *Which track has the highest number of streams? Display the top 5 most streamed tracks.
#### To get the top 5 streamed trackes we'll have to sort the data set based on their stream values using the following code.
#### ![image](https://github.com/user-attachments/assets/f93a291f-3ed8-474f-8cdb-884d80311b7f)
#### Based from the output of the code the top 5 streamed tracks are Blinding Lights-The Weeknd, Shape of You-Ed Sheeran, Someone You Loved-Lewis Capaldi, Dance Monkey-Tones and I, Sunflower - Spider-Man: Into the Spider-Verse-Post Malone, Swae Lee

#### **Who are the top 5 most frequent artists based on the number of tracks in the dataset?
#### For this one we will use this following code.
####![image](https://github.com/user-attachments/assets/40de3737-cfb0-4fdf-b8c7-fed3a569bbb9)
#### ![image](https://github.com/user-attachments/assets/d02cf516-f18f-48d1-b946-b6ce4f137cbf)
#### as we can see here are the top 5 artists on the dataset based on tracks.
## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Temporal Trends
#### * Analyze the trends in the number of tracks released over time. Plot the number of tracks released per year.
#### To begin, we need to calculate the number of tracks released each year. After obtaining this data, we should arrange it chronologically to make the plot more interpretable. The code for this process is shown in the image below.
#### ![image](https://github.com/user-attachments/assets/9df82892-3b53-43d0-9c4c-a8974c04bb16)
#### here we used a code that counts tracks per year, then it sorts its by the time of the track released.
####![image](https://github.com/user-attachments/assets/3bc127c6-e9d8-46a8-8ce1-3956aabc7810)
#### this is the code for plotting the data that was recovered.
#### then here is the output.
#### ![image](https://github.com/user-attachments/assets/e0586d1b-9559-4caf-a713-68feb92fec2a)
#### The plot shows that from 1940 to the early 2000s, the number of tracks released each year stayed low and steady. Around the 2000s, releases began to increase gradually, with a sharp rise in the 2010s, peaking around 2020. This trend likely reflects the growth of digital music and changes in the industry.

#### **Does the number of tracks released per month follow any noticeable patterns? Which month sees the most releases?
#### First we need to convert the release date to get the exact month of tracks.
####![image](https://github.com/user-attachments/assets/d6968e54-3692-4fa9-8094-bfd42b74efd3)
#### then we will plot the data using a bar graph.
#### ![image](https://github.com/user-attachments/assets/a21d8adb-993f-4c5a-9fe8-d00a828c5b67)
#### ![image](https://github.com/user-attachments/assets/6a5e01e4-4f77-4f88-89f0-60b5eeb019e5)
#### observing the graph we can see that January has the most tracks released.
####  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Genre and Music Characteristics
#### Examine the correlation between streams and musical attributes like bpm, danceability_%, and energy_%. Which attributes seem to influence streams the most?
#### In this code snippet it shows the calculation for the correlation of different attributes
#### ![image](https://github.com/user-attachments/assets/db85fc21-5435-40ce-aa13-9c1d8fe443a1)
#### with the help of ai i asked it to help me to answer the follow up question "Which attributes seem to influence streams the most?"
#### ![image](https://github.com/user-attachments/assets/fae55bbe-e35a-48cd-a00a-264b5b346e3f)
#### **Is there a correlation between danceability_% and energy_%? How about valence_% and acousticness_%?
#### we first calculated for the correlation of danceablity and energy using this code:
#### ![image](https://github.com/user-attachments/assets/14e301d2-71e7-431c-b448-67214a91d257)
#### After that I visualized it using a scatterplot. Why a scatterplot you ask, after doing some internet surfing scattersplots help identify and visualize the relationship between two numeric variables. In this code I used Ai to help me get a better code.
#### ![image](https://github.com/user-attachments/assets/6a310855-e45e-4099-9ed4-02e4c42805b8)
#### ![image](https://github.com/user-attachments/assets/67384296-8fe5-45bf-94f1-6b705a517879)

#### The scatter plot shows a weak positive correlation between danceability_% and energy_%, meaning that as danceability slightly increases, energy tends to increase as well, but the relationship is not strong.
#### for the valence_% and acousticness_% this is the code snippet
#### ![image](https://github.com/user-attachments/assets/0951a9ce-f11d-47d1-b996-cd8c922d31e3)
#### ![image](https://github.com/user-attachments/assets/a1a39c5f-6afe-43b4-9755-bf1e5e05f3aa)
#### The scatter plot shows no strong correlation between valence_% (positivity) and acousticness_% (acoustic quality), as points are scattered widely across both axes without a clear trend.
## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Platform Popularity
#### How do the numbers of tracks in spotify_playlists, spotify_charts, and apple_playlists compare? Which platform seems to favor the most popular tracks?
#### For calculating the numbers of tracks here is the code and it shows the table of values of wanted data.
#### ![image](https://github.com/user-attachments/assets/ac7ed592-d8fa-4616-aa59-0fa89236cc27)
#### now I plotted it to have a better observation.
####  ![image](https://github.com/user-attachments/assets/50e299b2-82d4-4d3b-a53d-0e8f3c0d2124)
#### The box plot shows that tracks appear in many more spotify_playlists compared to spotify_charts and apple_playlists, with a large number of outliers reaching up to 50,000 playlists, indicating that Spotify playlists favor popular tracks heavily
#### For Which platform seems to favor the most popular tracks here is the code i made with help of Ai
####![image](https://github.com/user-attachments/assets/702b2cd0-2d05-4a87-aaf7-8e8a13cb161e)
#### The data shows that the maximum count for in_spotify_playlists is exceptionally high at 52,898, indicating that some tracks are included in many Spotify playlists, likely reflecting their widespread appeal or relevance across various playlists on the platform.
## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  Advanced Analysis
#### Based on the streams data, can you identify any patterns among tracks with the same key or mode (Major vs. Minor)?
#### Firs that i did was i coded to calculate for  the tracks for key and mode
#### ![image](https://github.com/user-attachments/assets/2c19be78-f62a-484b-bce0-aca426429783)
#### The bar chart shows the count of songs by musical key and mode, revealing that Major keys generally have higher counts than Minor keys, with B Major, C# Major, and G Major being particularly popular. Some keys, like D# Major and F# Minor, have notably low counts, indicating less frequent use.
#### Do certain genres or artists consistently appear in more playlists or charts? Perform an analysis to compare the most frequently appearing artists in playlists or charts.
####  Group  data for playlist and chart appearances.
#### ![image](https://github.com/user-attachments/assets/f2522824-6f40-4534-ae42-3187df4e909f)
####  Select top 5 artists for playlist and chart appearances
#### ![image](https://github.com/user-attachments/assets/e568a20d-37d4-4f3a-857a-06c64835b7aa)
#### for the playlist appearances here is the plot
#### ![image](https://github.com/user-attachments/assets/ba54121b-7180-46f1-ad13-098793eb9a4d)
#### For chart appearances
#### ![image](https://github.com/user-attachments/assets/7aa6c502-2800-4f0c-a886-d4b3b5869d76)
#### Base from the graph, C# Major emerged as the most frequently used key and mode across tracks. The Weeknd was the leading artist in terms of playlist features, with his songs appearing over 140,000 times on Spotify playlists. In contrast, Taylor Swift held the top spot for chart presence, achieving more than 1,750 appearances on Apple Music charts.


## END.






