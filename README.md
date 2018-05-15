# the-blue-alliance-assistant
A voice assistant for The Blue Alliance built with [Dialogflow](https://dialogflow.com)

Currently an experimental work in progress.

## How it works
When a user triggers The Blue Alliance on a voice assistant such as Google Assistant, requests are handled by Dialogflow. Dialogflow pattern matches what the user says with intents, and makes the appropriate requests to https://www.thebluealliance.com/_/api_ai, where are handled [here](https://github.com/the-blue-alliance/the-blue-alliance/blob/master/helpers/apiai_helper.py). With the request resutls, Dialogflow constructs a response for the user.

## Authentication
Requests to https://www.thebluealliance.com/_/api_ai are authenticated with the `X-TBA-APIA-Auth` request header. Make sure you update the URL and header when testing with your own development server.