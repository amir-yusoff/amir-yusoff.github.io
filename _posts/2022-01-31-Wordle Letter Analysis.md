---
layout: post
title: "Wordle Letter Analysis"
date: 2022-01-31 12:45:00 +0800
categories: [Python, Data Analytics]
---

## What is Wordle? 

[Wordle](https://www.powerlanguage.co.uk/wordle/) is a free game where you have six tries to guess a five-letter word through deduction. There is one word every day, which is the same for everyone. The new puzzle is released every day at midnight. Each time you guess a word, the letters will turn green, yellow or grey to indicate if it is in the correct spot. Green means the letter is in the right position, yellow means the letter appears somewhere in the word but not in the current position, and grey means the letter isn’t in the word at all.


## Letter analysis

Wordle will ever use are apparently all served to your device whenever you visit the webpage. The game only shows you the word for the current day however.

So, I decided to loop through all 2000+ words and plot the most frequently used letters. I used Python (specifically numpy and matplotlib + seaborn) to make the plot in a jupyter notebook which you can find in the GitHub repo linked below.

GitHub: https://github.com/amir-yusoff/wordle-letter-distribution

Word/Answer key: https://www.powerlanguage.co.uk/wordle/main.e65ce0a5.js

## Top 10 Letters Used

![Most frequently used letters in Wordle Answers](https://raw.githubusercontent.com/amir-yusoff/wordle-letter-distribution/main/TheDistribution.png)

## Tips

IRONS and CLEAT are good words to start off the game with.
