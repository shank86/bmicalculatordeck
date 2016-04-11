---
title       : Body Mass Index Classification in Adulta
subtitle    : Developing Data Products (Coursera)
author      : Sangar A.
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
ext_widgets : {rCharts: [libraries/HighCharts]}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

### Intro & Motivation

Body Mass Index (BMI) is a simple index of weight-for-height that is commonly used to classify underweight, overweight and obesity in adults. It is defined as the weight in kilograms divided by the square of the height in metres (kg/m2).  

Key facts:  
* Worldwide obesity has doubled since 1980.  
* In 2008, more than 1.4 billion adults, 20 and older, were overweight. 
* 35% of adults aged 20 and over were overweight in 2008, and 11% were obese.  
* 65% of the world's population live in countries where overweight and obesity kills more people than underweight. 
* Obesity is preventable.

Good Nutrition and regular phisical activity are vital for good health and disease prevention. Overweight and obesity are serious and costly health problem worldwide; it's very important people to be informed and aware of overweight and obesity trends.


--- .class #id 

## Shiny App: BMI Calculator

<div style='text-align: center;'>
    <img src='Snap1.jpg' />
</div>   
[BMI Classification in Adults App Hosted by shinyapps.io](https://asquare.shinyapps.io/BMICalculator/)  

---

## Features

User can enter their weight, height, gender and country to get informed!


<div id = 'chart1' class = 'rChart highcharts'></div>
<script type='text/javascript'>
    (function($){
        $(function () {
            var chart = new Highcharts.Chart({
 "dom": "chart1",
"width":            800,
"height":            400,
"credits": {
 "href": null,
"text": null 
},
"exporting": {
 "enabled": false 
},
"title": {
 "text": null 
},
"yAxis": [
 {
 "title": {
 "text": "MeanBMI" 
} 
} 
],
"series": [
 {
 "data": [
 [
 1980,
          23.1 
],
[
 1981,
          23.1 
],
[
 1982,
          23.1 
],
[
 1983,
          23.1 
],
[
 1984,
          23.1 
],
[
 1985,
          23.1 
],
[
 1986,
          23.1 
],
[
 1987,
          23.1 
],
[
 1988,
          23.1 
],
[
 1989,
          23.1 
],
[
 1990,
          23.2 
],
[
 1991,
          23.2 
],
[
 1992,
          23.2 
],
[
 1993,
          23.3 
],
[
 1994,
          23.3 
],
[
 1995,
          23.3 
],
[
 1996,
          23.4 
],
[
 1997,
          23.4 
],
[
 1998,
          23.4 
],
[
 1999,
          23.4 
],
[
 2000,
          23.4 
],
[
 2001,
          23.4 
],
[
 2002,
          23.4 
],
[
 2003,
          23.4 
],
[
 2004,
          23.4 
],
[
 2005,
          23.3 
],
[
 2006,
          23.3 
],
[
 2007,
          23.2 
],
[
 2008,
          23.2 
],
[
 2009,
          23.1 
] 
],
"name": "Female",
"type": "line",
"marker": {
 "radius":              3 
} 
},
{
 "data": [
 [
 1980,
          22.5 
],
[
 1981,
          22.6 
],
[
 1982,
          22.6 
],
[
 1983,
          22.7 
],
[
 1984,
          22.8 
],
[
 1985,
          22.8 
],
[
 1986,
          22.9 
],
[
 1987,
          22.9 
],
[
 1988,
            23 
],
[
 1989,
          23.1 
],
[
 1990,
          23.2 
],
[
 1991,
          23.2 
],
[
 1992,
          23.3 
],
[
 1993,
          23.4 
],
[
 1994,
          23.5 
],
[
 1995,
          23.6 
],
[
 1996,
          23.6 
],
[
 1997,
          23.7 
],
[
 1998,
          23.8 
],
[
 1999,
          23.8 
],
[
 2000,
          23.9 
],
[
 2001,
          23.9 
],
[
 2002,
          23.9 
],
[
 2003,
          23.9 
],
[
 2004,
          23.9 
],
[
 2005,
            24 
],
[
 2006,
            24 
],
[
 2007,
            24 
],
[
 2008,
            24 
],
[
 2009,
            24 
] 
],
"name": "Male",
"type": "line",
"marker": {
 "radius":              3 
} 
} 
],
"xAxis": [
 {
 "title": {
 "text": "Year" 
} 
} 
],
"subtitle": {
 "text": null 
},
"id": "chart1",
"chart": {
 "renderTo": "chart1" 
} 
});
        });
    })(jQuery);
</script>

*Plot: Mean body mass index(crude estimate) trend by gender in Singapore*   

---

## Features

*Plot: BMI indicators in Georgia, USA*  

<div id = 'chart2' class = 'rChart highcharts'></div>
<script type='text/javascript'>
    (function($){
        $(function () {
            var chart = new Highcharts.Chart({
 "dom": "chart2",
"width":            800,
"height":            400,
"credits": {
 "href": null,
"text": null 
},
"exporting": {
 "enabled": false 
},
"title": {
 "text": null 
},
"yAxis": [
 {
 "title": {
 "text": "Value" 
} 
} 
],
"series": [
 {
 "data": [
 [
 "Underweight",
             2 
],
[
 "Normal.Weight",
          33.3 
],
[
 "Overweight",
          35.5 
],
[
 "Obese",
          29.1 
] 
],
"type": "bar",
"marker": {
 "radius":              3 
} 
} 
],
"legend": {
 "enabled": false 
},
"xAxis": [
 {
 "title": {
 "text": "Indicator" 
},
"categories": [ "Underweight", "Normal.Weight", "Overweight", "Obese" ] 
} 
],
"subtitle": {
 "text": null 
},
"id": "chart2",
"chart": {
 "renderTo": "chart2" 
} 
});
        });
    })(jQuery);
</script>
