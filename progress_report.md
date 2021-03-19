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
