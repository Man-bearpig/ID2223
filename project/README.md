# Goal

Predict the AQI in Helsinki for the next 7 days.

# Hugging Face url


To see the predictions, press "Submit" with random input.

# Data Source

## Air Quality

https://aqicn.org//here/

## Weather Conditions

https://www.visualcrossing.com/

# Project Architecture

The project include the following steps:

1. Request API-key in order to request data from data source, store the API-key in the .env configuration file.
2. Use to automatically download Helsinki's weather data from data source.
3. Use to create feature pipelines.
4. Use to combine feature piplines into a feature view and generate training pipline.
5. Use to start a Gradio app and predict AQI in Helsinki in the next 7 days.
