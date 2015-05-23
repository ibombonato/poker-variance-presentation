---
title       : Poker Variance Simulator App
subtitle    : See how long term variance in poker can be
author      : Icaro C. Bombonato
job         : Senior Developer at minhavida.com.br
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : standalone # {standalone, draft}
knit        : slidify::knit2slides
output: 
  html_document: 
    theme: flatly
---



## Purpose

New poker players have problems to understand how variance can impact their results and how it works in the long term.  

This app was created to explain variance for poker players in the long term.  

---

## How it works

Based on two variables that are comom for the players, **Winrate** and **Standard Deviation**, we can plot a simulation of 100k hands played and see the possible outcomes in **Buy-ins**.  

That way, the players can have a clue for what to expect in terms of results (in buy-ins), in a range of 100k hands played based on their win rate and stardard deviation.

---

## What is the results? Real code run example:

After you input your variables, in this case **winrate 4, sd 95 and 25 trials**, you will got a plot like the one bellow:


```r
winrate <- 4;sd <- 95;trials <- 25
plotData(simulateData(winrate, sd, trials), winrate, sd, trials)
```

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3-1.png) 

---

## Screen Shot

And now, one screen shot of the app running at shinyapps.io:

![width](assets/img/shiny.jpg)
