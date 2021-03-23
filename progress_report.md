# Progress Report

## Log 1: February 17, 2021
  This week I created my GitHub repository which consists of my `README` file that
includes my name, project title, and a brief summary. I also added a `LICENSE` file
that is essentially blank and will be specified later. I have added a `private` file
that will include notes on **Topic Modelling** and put that directories in my
`.gitignore` file, as instructed. I have also added the `progress_report` file
(which is the current file). Lastly, I polished up my project_ideas file from
the previous assignment and fashioned it into my `project_plan`. I added
rephrasing of some sections, as well as, added some links about Topic Modelling
and an example of usage of *John Miller's LyricGenius* code.

## Log 2: March 9, 2021
I reviewed the Terms of Service of Genius to make sure I can use the lyrics for my particular project. I was confused by some of the terminology in it regaring licencing to use the data. I have a feeling that is is just associated with trying to alter what is on their website and not general scraping. However, I e-mailed Lauren Collister to make sure I am in the right before I proceed and am currently waiting on a response from her before I create my Genius API account so that I can proceed with scraping. I'm fairly sure it is fine to scrape for my purposes especially since I am not the only one to do a project such as this using their data. Once I receive the go ahead, I will begin to craft my own License which will be pretty open with directions like previous projects that I have referred to. Lauren replied rather quickly saying that I have a "strong Fair Use case because this is a transformative use". She suggested that I fill out one of the many fair Use checklists to help me document this. She also said that my best bet is to share the "dataset" as a list of the songs that are in my project but not the full lyrics. I can do my Topic Modelling on the full dataset and only share short snippets of the lyrics in a chunk as an illustration like quoting in an essay.

I have updated my `bs4` and installed the `lyricsgenius` library from John Miller's project to be prepared for scraping when the time comes.

## Log 3: March 14, 2021
I tried to make sense of the code to download the lyrics but ran into some roadblocks. Will attempt to reconfigure tomorrow. I'm just a bit lost and I got frustrated with understanding the code to get exactly what I wanted.

## Log 4: March 15, 2021
After talking with Joey and Na-Rae, I discovered that the best way to initialize the Genius API code from *John Miller's LyricGenius* without pushing sensitive data to my repository was to put the token in a `.txt` file and placed into the `.gitignore` in order to not be tracked by GitHub. I will then read the .txt file into the Python script instead of a Jupyter notebook file as originally planned, at the direction of Na-Rae because apparently Jupyter notebook doesn't handle scraping well. I will attempt doing this task tomorrow.

## Log 5: March 18, 2021
After playing around with the code and witnessing how it worked, I decided to limit my artist list to 20 artists, 10 male and 10 female from different eras of Rap (1990s, 2000s, 2010s), with some having careers that spanned all three decades and into the current decade, 2020s. The artists that I chose were handpicked from the Ranker List Best Rap Artists of All Time and also Google for the female rappers since they didn't have a wide presence on the list. I also decided to equalize each artist for up to 100 songs from each artist, acknowledging that some artists may have more or less than others. I am downloading each artists lyrics by hand to mitigate certain terms that should be excluded from each of the song names to make sure I am not getting repeat songs. This a long an tedious process but it will help in the long run when I don't have to throw out a bunch of the songs once I make the data frames. I have downloaded 600 lyrics from 6 of the male artists, and the lyrics are in a directory not tracked by GitHub to not violate Genius TOS. I will continue this effort tomorrow. I also added a markdown file `lyric_collect_PROCESS.md` which details how I scraped my lyrics from Genius using the `LyricsGenius` package. I also changed the name of my Jupyter Notebook to `lyrical_data_analysis.ipynb` to make the file into my analysis page.

## Log 6: March 19, 2021
I downloaded all of my male rappers' lyrics; thus, bringing my current total to 1000 song lyrics from Black male Rappers. Tomorrow I will download half of the Black female rappers' lyrics (5 artists). Hopefully on Sunday, I will be able to start working with cleaning the data and putting it into the following data frames: All artists/lyrics, Male artists and Female artists. Then on Monday, I should be able to do begin learning about LDA Topic Modelling and building word clouds.

## Log 7: March 20, 2021
I have downloaded all of my female rappers' lyrics however 2 artists had less than 100 songs on Genius (Remy Ma-86, Cardi B-76). The total lyrics compiled without limitation or cleaning outside of the excluded terms parameter that I set: **1962**. I am expecting that I will have to filter out lyrics that have **"skit"** and **clean** in the title. I will ahve to filter out duplicate songs I saw a few in the clean section that are duplicates and just the same titles with the names spelled differently. I will look into this tomorrow when I'm cleaning the data. I'm expecting the number of lyrics from each side (male and female) to go down maybe to around **1700**.

## Log 8: March 21, 2021
I went to parse through the lyrical data and realized that I need to compile the lyrical files into Male lyrics and Female lyrics to make the different dataframes necessary for my analysis. I have them in separate files but I need to compile the individual `.json` files. I tried to do some digging and nothing that I tried would work properly. I will ask for help tomorrow and try this task.

## Log 9: March 22, 2021
I cannot get a single file to read into a data frame (see l`yrical_data_analysis.ipynb`). I asked for help, but we will ahve to reconvene another data. Proud that I was able to get all of the files that I wanted onto my computer. Now to just figure out how to read them into a dataframe so that I can begin the cleaning process. I found a tutorial that does LDA topic modelling on [YouTube](https://www.youtube.com/watch?v=wKW8z6zqCFo); however, this works with CSV files and not JSON so still back in the same place I started. Hopefully, I, with help from Na-Rae and Joey, will be able to figure this out. But until then, project on hold.
