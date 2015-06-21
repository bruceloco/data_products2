---
title       : Using the my Iris species app to visualize combinations
subtitle    : The apps allows the user to see visually what type of species this iris will become
author      : Bruno Gomes
job         : 
framework   : io2012 #revealjs
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap, quiz]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---&radio

## Enter the presentation

Prove that you are not a robot, what is a+b?

1. "a"+b 
2. "a"+"b" 
3. "ab" 
4. _ab_ 

*** .hint
ignore the quotes

--- 

## Initial design of the application

This application started out basic, developed nicely and was made basic again, I will list the reasons:

> * First I just wanted to add some charting and change from colored to non colored
> * But since prediction is fun, I added random forest predictors for the Iris dataset.
> * It works fine on my local machine, gave an accuracy of roughly 95% and displayed the predicted Iris species
> * Saddly, after uploading to shinyapps.io, the incompatibilities started manifesting as dependency hell
> * I added a library, uploaded, another was missing(this due to caret), then we came to the chicken and egg situation
> * I cannot install modGbm for caret because I run R 3.2, shinnyapps lists it as a dependency and won't work without it
> * So it was made basic again and just displays and updates the model in the pairs chart.

---  &multitext

## Basic maths

Just checking if the presentation did not make you fall asleep yet:

1. What is the square root of 9?
2. Multiplied by 15?

*** .hint
click the explanation

*** .explanation
the square root if 9 is <span class="answer">3</span>
It them becomes <span class="answer">45</span>


--- 

## Charting through the waters

You will find the following chart which you can turn from black and white to colored:

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png) 

--- 

## Conclusion

The application is actually quite interesting when the prediction is done.
If you check **github** and look at the previous branch you will be able to download and execute the predictive application independent from shinyapps.io.

Thank you for your time


