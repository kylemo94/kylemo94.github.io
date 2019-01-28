---
layout: project
type: project
image: images/numbers.jpg
title: GuessInteger
permalink: projects/guessInt
# All dates must be YYYY-MM-DD format!
date: 2017-11-20
labels:
  - Random
  - Atom
  - python
  - game
summary: A little game where the user guesses the random integer generated for ICS 215.
---

<img class="" src="">

GuessInteger is a program that I created for ICS 215. It implements the use of import and random function.

The game randomly picks an integer between 1 and 10. Then the user tries to guess the number in 5 tries otherwise the game
automatically exits and the appropriate message is displayed. The program tells the user if the guess inputted is either
too high or too low, thus the player is able to deduce the number easily.

For this project I used atom to write my code, which is a program that supports many programming lanugages. Since this was
the first python assignment for this class I was able to see the similarities and differences between other programming 
languages.

Example code below:

while(attempt != 5 and guess != randomNum):
  #if guess is less than randomNum
  if(guess < randomNum):
    print("Too low, try again.");
    #prompt user again
    guess = input("Enter an integer between 1 and 10: ");
    guess = int(guess);
    #increment count
    attempt += 1;
  #if guess is greater than randomNum
  if(guess > randomNum):
    print("Too high, try again.");
    #promt user again
    guess = input("Enter an integer between 1 and 10: ");
    guess = int(guess);
    #increment count
    attempt += 1;

Source code provided on request.
