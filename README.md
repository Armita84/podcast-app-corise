# podcast-app-corise
Summary Castbox podcasts in a written form using OpenAI products

## Description: 
- This project is part of the Uplimit ###'Building AI Products With OpenAI'### Workshop.
  
-The project is developed with ###Streamlit app### to show a Newsletter to the Podcast Listeners and it uses ###Modal Cloud as Backend###.

-The main core of the job is to get the latest podcast of an episode, transcribe the episode and create
a summary for the readers in the newsletter, and provide as much as info that is discussed in the talk to the uesr.

## How to Find the App:
Here you can see the app and read the Castbox podcast summary : 

(https://podcast-app-corise-armita-raz.streamlit.app/)


## How the project is done:
1- Instead of RSS feed to get the episodes of an podcast, BeautifulSoup Python library is used 
and the episodes of a podcast are collected only by passing the Castbox Podcast URL.

2- By the help of ###'OpenAI Whisper Speech To Text Model'###, the transcription of the audio is done and now we have the full text of that talk

3- Using ###'gpt-3.5-turbo'### API from OpenAI, the podcast summarization is completed and also get guest info and key moments of the talk.

4- A "rate/score" and a "short review" are provided not by the user or explicit info in the talk, but by AI itself!

5- The podcast episode summary, the episode title, image and the guest info and highlighted moments; as well as the review and rate done by AI are 
shown in the newsletter page in the Streamlit app.  

Users can navigate to different episodes from the left sidebar of the app and read the summary of that episode.
You can listen to the Podcast Audio in the app as well.

## Files/Folders in the Repo:

1- ##.stremlit ## : the Streamlit app config file
2- ## podcast_frontend.py ## : the frontend file for app development in Streamlit 
3- ## requirements.txt ## : required libraries for running the project 
4- ##style.css ## : the style of app 
5- ##json files## : the result of the OpenAI models for each episode to be fed into frontend


