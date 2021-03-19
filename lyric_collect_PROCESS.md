# Lyric Collection Process
- This is the coding process that I used to download 100 songs from each of the artists.
- Further explanation of this code and methods is found [here](https://github.com/johnwmillr/LyricsGenius)

1. **Make an account with Genius API and collect your information (i.e. Client Access Token)** <br>
  - You must do this to be able to use the `lyricsgenius` package.

2. **You must install the lyricsgenius package to Python3 using:** <br>
`pip install lyricsgenius` or <br>
`pip install git+https://github.com/johnwmillr/LyricsGenius.git` (to get the latest version from GitHub)

3. **Import the library:** <br>
`import lyricsgenius`

4. **Initialize Genius:** <br>
`genius = lyricsgenius.Genius("GENIUS_CLIENT_ACCESS_TOKEN")`

5. **Set Parameters within Genius Class:** <br>
- Remove Section Headers from Lyrics (e.g. [Chorus]) from lyrics when searching <br>
`genius.remove_section_headers = True`
- Exclude songs with certain words in their title <br>
`genius.excluded_terms = ["(Remix)", "(Live)"]`
    - added terms as I saw fit for each artist to get better song lyrics results

6. **Search for Artists:**
- Excluded songs where the artists are features on the song (i.e. feat. Jay-Z) <br>
`artist = genius.search_artist("ARTIST_NAME", max_songs=100, sort="title", include_features=True)`

7. **Save song lyrics:** <br>
- Save the song lyrics from the search in a JSON file
`artist.save_lyrics()`
