# Setup

  Create a BigQuery dataset with the name ```[fist-initial-last-name]-proj-1``` under the ```york-cdf-start``` project. Store any tables needed for this project under this new dataset. 
  
  The pipeline for this project should be created under the Data Fusion ```york-data-source``` instance.
  
# Project

Create a new data pipeline in Google Data Fusion that will sort and store records from the ```bigquery-public-data:hacker_news.stories``` table.

  1. Grab all the records from the stories table
  2. Filter the results from the table to only records with an author in the cloud storage file ```subscribed_authors.csv```. It can be found in the ```york-project-bucket```.
  3. Store the results in a table called ```subscribed_user_stories```. (all fields should be copied over)
  4. Group the ```subscribed_user_stories``` data to create a list of story authors and the ```sum``` of all the points from there posts.
  5. Store the list of author and there points into a Big Query table called ```author_rankings``` (you only need to keep the athors name and the sum of the points from there stories).
  6. Store the list of author and there poitns into a CSV file in Cloud Storage called ```author_rankings.csv```.
  
  
  ![image](https://user-images.githubusercontent.com/31535228/146306729-b8580690-27c5-4153-8227-a44e1302e27f.png)

  
 
