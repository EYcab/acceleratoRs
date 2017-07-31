# Data Science Accelerator - *Solar power forecasting with Cognitive Toolkit in R*

## Overview

This repo reproduces CNTK tutorial 106 B - time series forecasting with
Long Short-Term Memory (LSTM) in R, by using Keras R interface with
Microsoft Cognitive Toolkit in Azure Data Science Virtual Machine (DSVM)

The repository contains three parts

- **Data** Solar panel readings collected from Internet-of-Things (IoTs)
    devices are used.
- **Code** Two R markdown files are available - the first one titled
    **SolarPanelForecastingTutorial** provides a general introduction of
    the accelerator and codes for setting up an experimental environment
    on Azure DSVM; the second one titled **SolarPanelForecastingCode**
    wraps codes and step-by-step tutorials on build a LSTM model for
    forecasting from end to end. 
- **Docs** Blogs and decks will be added soon. 

## Business domain

The accelerator presents a tutorial on forecasting solar panel power
readings by using a LSTM based neural network model trained on the
historical data. Solar power forecasting is a critical problem, and a
model with desirable estimation accuracy potentially benefits many
domain-specific business such as energy trading, management, etc.

## Data science problem

The problem is to predict the maximum value of total power generation in
a day from the solar panel, by taking the sequential readings of solar
power generation at the current and past sampling moments.

## Data understanding

The data set used in the accelerator was collected from IoT devices
incorporated in solar panels. The data is available at the
[URL](https://guschmueds.blob.core.windows.net/datasets/solar.csv).

## Modeling

Model used in this accelerator is based on LSTM, which is capable of
modeling long-term depenencies in time series data. By properly
processing the original data into sequences of power readings, a deep
neural network formed by LSTM cells and dropout layers can capture the
patterns in the time series so as to predict the output.

## Solution architecture

The experiment is conducted on a Ubuntu DSVM. 