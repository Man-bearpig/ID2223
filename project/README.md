# Goal
Air quality index (AQI) is a measure used to describe the level of air pollution in a particular area. It is calculated based on the levels of certain pollutants in the air, such as particulate matter, ozone, carbon monoxide, and nitrogen dioxide. The higher the AQI, the more polluted the air is.

Predicting AQI in Helsinki can be useful for a variety of purposes, such as to help people with respiratory issues plan their activities, to inform decisions about transportation modes, and to support policy makers in developing strategies to reduce air pollution.

This project aims at predicting the AQI in Helsinki for the next 7 days based on previous weather and air conditions.

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
3. Use Feature_pipeline.py to create feature pipelines.
4. Use to combine feature piplines into a feature view and generate training pipline.
5. Use to start a Gradio app and predict AQI in Helsinki in the next 7 days.
