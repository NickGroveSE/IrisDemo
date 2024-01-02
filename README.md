# What is Iris?

Iris is going to be a web app that creates an iridescent representation of the music you listen to, and this Github Repo is the Frontend Demo. The way it will work is you login to your Spotify and using your top ten songs from your last month of listening it will create your "Iris". Your Iris is an everchanging visual representation of the prevalent colors found in album artwork of you song you love. You will be able to change the timeframe that Spotify pulls from, letting you see your Iris over the last 6 Months or All Time Iris. I also wanted to give the user the ability to look into the colors of the songs, so every song will show a palette of the colors it contributes to the Iris and the palette is linked to coolors.co so you can look into the colors more in-depth.

## How Far Along is the Project?

I am currently going to be starting on the Backend functionality of Iris. Currently with the Frontend Demo the songs and colors are hardcoded, so with the Backend I will be working with ImageMagick to get the colors of the album artworks, and using Spotify APIs to extract listening or users.

## Frontend Backlog

This section includes what more I need to do for the Frontend, but these are parts of the Frontend that do not involve the Backend at all (tasks like this will be a priority when working with the final repo).

- Check How Frontend looks on all Browsers
- Animate Components when Mounted (CSS)
- Morph Shapes of Glimpse within Iris (Sass)
- Create a Timed Function Call to Vary the Movement of Glimpses (Sass)