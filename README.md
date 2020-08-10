## @WeRateDogs
### Jupyter Notebook: Data Visualization Project 

#### The primary focus of this project was Data Wrangling from the @WeRateDogs @Twitter account using Python and documenting the results in a Jupyter Notebook. The account WeRateDogs rates dogs uses humorous commentary to rank their submitted entrants. While the base-rating denominator is usually a 10, the numerators are usually greater than a 10. While some end-users will find it humorous a particular dog is ranked 14/10, this creates a myriad of challenges regarding cleaning the data in order to conduct more effectice data analysis. 

#### Project Details

##### For this project, the focus was only on original ratings (no retweets) that contained images. This is an important distinction because not all of the original tweets in the dataset are dog ratings and some are retweets.

##### Project tasks included - 

- Data wrangling 
- Gathering the data
- Assessing the data
- Cleaning the data
- Storing, analyzing, and visualizing the wrangled data
- Reporting on the data analysis and visualizations 

##### Data

The @WeRateDogs's Twitter archive (for tweets posted through August 1st, 2017) contained basic Tweet data (Tweet ID, timestamp, text, etc.) Udacity provided an "enhanced" csv-file containing columns extracted programatically including the rating numerator, the rating denominator, the dog's name, and the dog stages (doggo, floofer, pupper, and puppo). These columns also needed to be assessed and cleaned as the extraction process was not without challenges due to how the data set was structured and how some of the data was inputted into this csv file.

Finally, their @Twitter archive also lacked some useful information including the retweet count and the favorite count. Using Tweet IDs to query the Twitter API for each Tweet's JSON data was handled using Python's Tweepy library. Storing each Tweet's JSON data and then reading the text file line-by-line using Pandas DataFrame parsed this data subset down to only the desired variables of the retweet count and the favorite count.
