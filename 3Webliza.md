---
title: Webliza
layout: post
description: Implementation of ELIZA in python, with user-interface to chat with the bot
image: https://github.com/VipinindKumar/Webliza/raw/master/webliza.gif
gif: https://github.com/VipinindKumar/Webliza/raw/master/webliza.gif
show_tile: true
nav-menu: true
---

Implementation of ELIZA(https://en.wikipedia.org/wiki/ELIZA) in python, with interface to chat with the bot.

[Static part of the project deployed on github pages](https://vipinindkumar.github.io/Webliza/)

Created as a final project for CS50 course.

    - scripts.js shows the content of "#message-box"(content you type) in the box as a sended message
    - and then use ajax to make a POST call to /message with the message you typed in #message-box
    - application.py recieves the call to /message with POST method
    - and check if a certain pattern is recieved from the form,
    - if does exist it returns a video frame
    - else it calls analyze() function from eliza.py with message as argument
    - analyze() function in eliza.py matches the statement with pre-defined patterns
    - and if matched, it returns a formated random response attached to the matched pattern
    - when scripts.js recieves this returned value as data, it runs an anonymous function
    - that displays it, scrolls to bottom(inside box) and then empty the typing #message-box.


[Github Repository - Webliza](https://github.com/VipinindKumar/Webliza)

