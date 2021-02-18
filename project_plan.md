# What Y'all Sellin Ova There?: The Black Experience Commodified in Rap Lyrics

## Project Summary
This project which employs Topic Modeling will look into some prominent Black
American Rap artists and taking a dive into what these rappers are saying in
their music lyrics, including but not limited to, thematic representations or
specific words. I want to look at what they are saying in their songs and if
it corresponds with how popular the song is.

## Project Plan: Data Portion
I plan on making a `.csv` file much like the billboard lyrics corpus we worked on
in class. I would need to include the song, the artist, the album, the year in
which the song was released, the billboard rankings, and the lyrics themselves.
I would need to utilize **John Miller's "LyricsGenius"** web scraper to download
the lyrics and his program for getting Spotify and Billboard data. I believe that
I want to use lyrics drawn from prominent Black American rappers and rap groups.
To retrieve this information, I will be drawing from two user created lists of the
greatest rappers and rap groups of all time, which will be taken from the
direction of **Anders Olsen-Swanson's Natural Language Processing and Rap Lyrics**
project: https://towardsdatascience.com/natural-language-processing-and-rap-lyrics-c678e60073fb

**Ranked Lists:** <br>
https://www.ranker.com/crowdranked-list/the-greatest-rappers-of-all-time <br>
https://www.ranker.com/crowdranked-list/overall-best-hip-hop-crew

I don't have an existing data source per se and will have to mine for my own data.
But, I am taking the direction of **John Miller's programs and provided examples**: <br>
https://github.com/johnwmillr/trucks-and-beer <br>
https://github.com/johnwmillr/LyricsGenius

This is a **Sentiment Analysis of 2017 Rap albums** but it might deem useful: <br>
https://github.com/Hugo-Nattagh/2017-Hip-Hop <br>
- it seems it will be useful for the following excerpt in Hugo's `README.md`:
  - "It’s very useful but unfortunately cannot get all the lyrics for an album,
    I had to do a query for each song. I forked his repo and tried my hand at
    improving his script but realized that his library is using Genius.com’s API,
    which only allows requests for artists and songs. So I worked around it in a
    way that doesnt make my modifications fit with his library. I used Beautiful
    Soup to scrape the songs’ titles from the album page, and made a loop to
    request all those songs with lyricsGenius."
- I can see that the data mining may not be so easy and will be very time
  consuming because of this...

**Information on Topic Modeling:** <br>
https://towardsdatascience.com/end-to-end-topic-modeling-in-python-latent-dirichlet-allocation-lda-35ce4ed6b3e0 <br>
https://www.analyticsvidhya.com/blog/2016/08/beginners-guide-to-topic-modeling-in-python/ <br>
https://www.machinelearningplus.com/nlp/topic-modeling-gensim-python/

## Project Plan: End Goal
My end goal would be to see what Black American Rappers are saying in their most
popular songs, thematically. Ultimately, their lyrics and lyrical structure are what
makes these rappers popular in the first place and either maintains or kills their
careers. I would like to see if certain themes persist or change in these rappers
songs or in rap music across time. A working hypothesis that I have so far is that
the themes in rap music are pretty much maintained (e.g. drugs, sexualizing women,
getting large amounts of money, reflecting on times they didn't have money,
injustices to Black people, etc.). However, I think depending on the rapper's
gender, the themes may vary. I am not planning on doing any predictive analysis
to my knowledge.

## Project Plan: Presentation Portion
I think I will be using Powerpoint/Keynote slides and utilization of different graphs.
I'm not sure which ones will best suit my project right now; however I am leaning
toward some ANOVAs.
