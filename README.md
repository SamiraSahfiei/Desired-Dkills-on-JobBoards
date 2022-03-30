# Scraping for desired skills on JobBoards

This project helps business analytics and data analytics students in their career development journey by identifying and ranking actual desired skills listed in role-targeted, real-world job listings

The project is based on web-scraping job listings from ten cities in the USA that are known for having many tech-based careers, such as Chicago, New York, San Francisco, etc.
I used the web scraping software platform, Apify, that automatically scrapes and extracts from websites to pull key skill sets from the aforementioned job-listings and run them through N Grams. 
I analyze tool, soft, and hard skills among all the listings, and rank the top skills needed. 


# Data source: 

The data is from a popular job posting portal: www.indeed.com. I limited the analysis to skills related to Data Analytics, and used the keyword ‘Data Analyst’ to filter the job postings. 
The data was scraped using a free, online web-scraping platform called Apify.com. The extracted data is in JSON format. 
There was a limitation of extracting approximately 1000 job postings from each city. All the data was scraped on 27th October 2021. 

The raw dataset contains a total of 9 attributes. The description of each attribute is provided below:
<img width="634" alt="image" src="https://user-images.githubusercontent.com/93683920/160919164-b780332f-efe3-49d4-a4b4-948389894144.png">


# N-grams
I performed unigram, bigram, and trigram analysis on the data. The results showed a lot of unnecessary n grams and very few useful ones. 
If we went with those results, we would have had to do a lot of cleaning and pick out the ones that are considered a skill set. So, I created lists of skills: tool skills, hard skills, and soft skills and divided them into lists of one word and two words to be able to search for them in our unigram and bigram dataframes.

According to the analysis bigrams performed the best, giving us the greatest amount of information with two word grams:
 - The top 5 tool skills: sql, tableau, Python, r, power bi
 - The top 5 hard skills: reporting, database, testing, statistical, data vusualization
 - The top 5 soft skills: project management, attention to detail, problem solving, critical thinking, decision making

Morover, I categorizized skills, based on Data Analyst Functions Areas
- Finance and Accounting
- Marketing
- Operation

