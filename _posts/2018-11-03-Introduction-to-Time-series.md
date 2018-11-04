---
layout: post
title: "Introduction to Time Series Analysis using Python"
featured-img: bgstf
categories: [Machine learning]
---

# THE BASICS OF TIME SERIES ANALYSIS

## WHAT ARE TIME SERIES? 

Time series  is a series of data points indexed (or listed or graphed) in time order. 
Or in other words, a collection of observations of well-defined data items obtained through repeated measurements over time at equal intervals e.g hourly, daily, weekly, quarterly, yearly, etc. It is mostly used to predict future occurrences based on previous observed occurrence or values.

**Examples:**
* Continuous monitoring of a person’s heart rate,
* Hourly readings of temperature or humidity,
* Daily closing stock prices,
* Monthly precipitation in a specific location,
* Yearly sales revenue/figures.

![examples](https://github.com/ninjakx/ninjakx.github.io/raw/master/assets/img/posts/TSEXAMPLE.png)

<p style='color:red'> NOTE: Data collected irregularly are not time series.</p>


## WHY DO WE NEED TIME SERIES?

This is the question that arises in our mind Why do we need to go for times series data?. The answer is very simple as we want to understand the past trends so we can plan for the future.
For example, How do you decide when is the right time to buy something. For instance, take the example of gold. We invest in the gold when we know its price is going to be high in the future but how do we come up with this?. Simply we just look at the historical sales data of it to draw some inference.


## COMPONENTS OF TIME SERIES:

* Trend component - a long-term increase or decrease in the data regularly through time which might not be linear. Sometimes the trend might change direction as time increases and result in varying mean over time.
It is the result of influences such as population growth, price inflation, and general economic changes. There can be Uptrend, Downtrend, Horizontal Trend depending on the pattern.

![trend example](https://github.com/ninjakx/ninjakx.github.io/raw/master/assets/img/posts/trenddef.png)

* Cyclical component - exists when data exhibit rises and falls that are not of the fixed period. Here the average length of cycles is longer than the length of a seasonal pattern. 
In practice, the trend component is assumed to include also the cyclical component. Sometimes the trend and cyclical components together are called as trend-cycle.These kinds of patterns are much harder to predict. 

![cyclic example](https://github.com/ninjakx/ninjakx.github.io/raw/master/assets/img/posts/2_cycl4.jpg)

* Seasonal component - exists when a series exhibits regular fluctuations based on the season (e.g. every month/quarter/year) and results in varying mean over time. Seasonality is always of a fixed and known period. It is the result of influences such as weather conditions, customs of people etc.

* Irregular component – It is the residual time series after the trend-cycle and the seasonal components (including calendar effects) have been removed. It corresponds to the high-frequency fluctuations of the series and is a stationary process.

![all in one example](https://github.com/ninjakx/ninjakx.github.io/raw/master/assets/img/posts/ss.PNG)

## STATIONARITY

A stationary time series is one whose statistical properties such as mean, variance, autocorrelation, etc. are all constant over time. 
As Trends can result in a varying mean over time while that of seasonality can result in a changing variance over time. Thus time series with trends, or with seasonality, is not stationary.
But time series with cyclic behavior (but with no trend or seasonality) is stationary as the cycles are not of a fixed length, we cannot be sure where the peaks and troughs of the cycles will be.

![all the time series type](https://github.com/ninjakx/ninjakx.github.io/raw/master/assets/img/posts/nst.png)

**Let us see which of the following series are stationary.**

**1)** 

  

<p style='color:red'>Non Stationary</p> as there is a trend and seasonality(variance is also increasing). 

<img src="https://github.com/ninjakx/ninjakx.github.io/raw/master/assets/img/posts/st2.png" width="600" height="300">

Solarized dark             |  Solarized Ocean
:-------------------------:|:-------------------------:
 <img src="https://github.com/ninjakx/ninjakx.github.io/raw/master/assets/img/posts/st1.png" width="600" height="300">
 | <p style='color:red'> Non Stationary</p> as there is a trend and seasonality(variance is also increasing).























