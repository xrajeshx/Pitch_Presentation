---
title       : Pitch Presentation for the Game "Guess The Number!"
subtitle    : (Use arrow keys to navigate)
author      : Rajesh Singh
job         : Developing Data Products Course Project
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Introduction and Motivation Behind the Game

This shiny app/game was created as part of the course project for the
Developing Data Products class under the Data Science Specialization offered by Johns Hopkins Bloomberg School of Public Health and Coursera.

--- .class #id 

## How to Play "Guess The Number!"

This game is pretty self-explanatory! Nevertheless, for the newbie further information on how to play the game is on the game interface itself. Basically, the user/player has to guess a number between 1 and 100 (inclusive) and see if it matches the computer's selection. The game outputs feedback to the player and lets him/her know if the guess is higher or lower than the number. Moreover, the game also lets the user know if the guess is below or above the prescribed limit and makes recommendations about the range for the next guess.

---

## R Code for the Computer's Selected Number

The following line of R code is placed on server.R of the shiny project and is executed once everytime the app is run. The runif(1,1,101) command selects a floating-point number between 1 and 101 and floor() is used to turn it into an integer between 1 and 100.  

```r
floor(runif(1,1,101))
```

```
## [1] 41
```

```r
floor(runif(1,1,101))
```

```
## [1] 90
```

Although there are other blocks of code in the project that may require  further explanation, to me, this seemed to be the single most important one.

---

## Comments about the Game and Acknowledgements
Although I have made some efforts in making the game, please note that it is by no means complete or flawless. For example, among all other bugs that my peers will notice when assessing the app, perhaps the most prominent is that the game doesn't stop even after the player has guessed the number correctly. It is due to my lack of skills/experience with Shiny and app development in general that such a flaw persists in the game. I sincerely apologize for this.

Furthermore, I would like to direct everyone to a more comprehensive, better and visually pleasing version this game (from an awesome developer) at http://www.funbrain.com/guess/

Finally, I would like to thank our Data Science Instructors Drs. Roger Peng, Jeff Leek and Brian Caffo and everyone else behind the screen for their great effors with the Data Science Specialization classes.

A special and more relevant thanks to Dr. Caffo for his contribution on the Developing Data Products class. It was due to his instructions and directions that the creation of this game was made possible.

