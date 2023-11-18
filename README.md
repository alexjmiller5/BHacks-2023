# BHacks-2023

# Initial Brainstorming
-Alarm app with picture if you sleep in that’s sent to all your friends
-Gardening connection to connect gardeners and farmer’s markets
-SNAKE
    -Snake game where to the tiles are musical keys – the score you get is based off the quality of the music
    -Snake game where the computer is trying to cut you off as another snake’
-Google calendar (student link chrome extension) → switch to this maybe? (pivoted to this idea)
-Fashion matching app (initially selected)

# Failed Idea: ML Color Style Image Recognition Mobile App

- Our app would have the user take a picture of themselves in their outfit, and then the app would use machine learning to determine the color scheme of the outfit to tell them if the color matches

## Research

-After reasearch many apis to see if they could determine the color of the outfit of a person in an image, we found that they either had signifcant paywalls such as [Imagga](https://imagga.com/solutions/color-api) and [folio](https://www.folio3.ai/prebuilt-models/apparel-detection/#:~:text=Clothing%20Detection%20Solution%20Accurately%20detect,recognize%20apparel%20types%20in%20images), or that they simply failed to work like [Farba's color extractor for apparrel](https://rapidapi.com/farba/api/color-extractor-for-apparel-2/)
-We found a outfit compatibility predictor to determine whether the color schemes of outfit, but the dependencies were outdated
-After more research, we found three main models to determine the color scheme and its stylishness of an outfit
    1. GAN (Generative Adversarial Network) to remove the background and skin of the image as done in this [article](https://towardsdatascience.com/clothes-and-color-extraction-with-generative-adversarial-network-80ba117e17e6)
    2. CNN (Convolutional Neural Network) to determine the color scheme of the outfit as done in this [article](https://towardsdatascience.com/color-identification-in-images-machine-learning-application-b26e770c4c71) OR implement KMeans clustering algorithm to determine the color scheme of the outfit using the elbow method as well
    3. Ask ChatGPT to help us write a program to determine if the color scheme found is stylish by color theory as done in this [article](https://www.canva.com/colors/color-wheel/)
- Ultimately, these models were too complex to implement in the time frame of the hackathon, so we decided to pivot to a new idea

# Pivot Point: Student Link GCal Exporter Chrome Extension

## User Stories

1. Downloads chrome extension
2. Clicks on extension icon
3. Prompted to sign in via Google OAuth
4. Signs in via Google OAuth
5. Create a mesasage that says we need to be able to access your calendar
6. Sign in is successful; if not -- prompt to sign in again
7. Give step by step instructions on how to navigate to the course schedule apge on student link
8. When on the course schedule page, present button to export course schedule to Google Calendar
9. Export to Google Calendar successfully!


Features to add:
-Chrome extension should light up red when on a page that has a student link calendar
-Button to export should only appear when on correct student link course schedule page

## Timeline

1. Figure out how to develop Chrome extensions