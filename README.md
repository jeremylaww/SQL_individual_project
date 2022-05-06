# SQL_individual_project

SQL 2022 INDIVIDUAL PORTFOLIO PROJECT
Jeremy Law 
Twitch API Webscrape 

Project Objective: 
I am posing as a twitch creator analyst trying to find notable games/streamers who have a notable following that might deserve special treatment from twitch such as perks, highlights, or even hosting/participating in twitch sponsored events.

I solve this problem by comparing top streamer data from 2020 vs stop streamer data from 2022 to see who has grown the most in those two years. Furthermore, I can join this with the games information I scraped as well to see the most popular games on twitch. Using this information I, as a Twitch Representative, can reach out to growing artists or set up tournaments of the most popular games for twitch consumers to watch. 

Job Description:
Twitch is an live streaming platform where broadcasters can livestream whatever they are doing to an audience they garner over time. This can range from playing video games, just chatting, or even "in real life streams" in which they broadcast doing things outside. It is a platform completely driven by its creators and how well they can gather an audience to watch what they are doing. As a creator analyst for twitch, my job would be to create insights out of creator data to either highlight up and coming creators just making headway or showcase already popular streamers to new viewers. The idea behind this job would be to create insights to drive campaigns to get more people to watch streamers on twitch rather than youtube live or facebook live.

This is where the project comes in. This project shows that I am capable of getting data from the TwitchAPI and creating insights on the most popular streamers, most improved streamers, and most popular games played. This information can be used for recruiting new twitch streamers in to the Twitch Partnership Program, inviting streamers with growing aduiences to attend twitch events to also attract their viewers, and also treating streamers who do a lot of Twitch with respsect so we continue to have a good relationship (instead of taking a contract to facebook live or youtube live). 

Data:
1. https://www.kaggle.com/datasets/aayushmishra1512/twitchdata
2. https://api.twitch.tv/helix/streams
3. https://api.twitch.tv/helix/games/top

Notebooks: 
[Data Collection](http://localhost:8891/notebooks/Desktop/Lontok%20SQL/notebooks/data_collection.ipynb)
This notebook contains all of the python code that was necessary to webscrape the Twitch API as well as push the data into my Amazon AwS RDS Instance 

[SQL_Analysis](http://localhost:8891/notebooks/Desktop/Lontok%20SQL/notebooks/sql_analysis.ipynb#Features-Used:-JOIN)
This notebook detailed my SQL queries and what insights I was able to make using them.

[presentation](http://localhost:8891/notebooks/Desktop/Lontok%20SQL/notebooks/presentation.ipynb#)
This notebook is the two previous notebooks put together in a presentation format. 




Future Improvements: 
The Twitch API is full of resources but a lot of it is locked behind specific tokens that aren't accessible to just anyone. For instance, if you wanted to get data on twitch Entitlements, which is data on twitch viewers receiving rewards for watching someones stream, you need to have the token for that specific streamer. This goes for a lot of the infomration avaiable actually. However, you can still do a lot with what Twitch offers to all of its users. If I had more time, I would've fixed my scraper to be able to record viewship counts over the span of a day more accurately. Twitch is weird about caching viewer count data (small streamers get their view count cached every 5-7 min while big streamers who are more volatile get their viewer count data cached every 30-50 min). 
