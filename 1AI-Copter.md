---
layout: post
title: AI Copter
description: AI that learns to play the classic Copter game
image: https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/9-score.gif
nav-menu: true
show_tile: true
---


# AI Copter
AI that learns to play Classic Copter game.

<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/9-score.gif"/>

### Pygame window and copter pixel image on it
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/1.png" alt="copter" width="300"/>

### Copter with gravity effect
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/2-gravity.gif" alt="copter with gravity" width="300">

### With jumping implemented
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/3-jumping.gif" alt="copter jumping" width="300"/>

### Copter game with obstacles
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/4-obstacles.gif" alt="copter with obstacles" width="300"/>

### With collision
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/5-collision.gif" alt="copter game with collision" width="300"/>

### Multiple Copters generation using NEAT
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/6-copters.gif" width="300"/>

### Copter AIs sticking to the top of the screen
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/7-toprider.gif" width="300"/>

### When top of the screen was made collidable with copter
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/8-working.gif" width="300"/>

### When fitness of the Copter AIs is increased with increment in score
<img src="https://raw.githubusercontent.com/VipinindKumar/AI-Copter/main/progress/9-score.gif" width="300"/>

- made score more important by increasing fitness 
  - definitely increased performance generation 6 reached score of 19

- change input to nnets from absolute value to -ve and +ve
  - generation 5 copter reached score of 25+

- added 1 hidden layer
  - generation 7's two copters reached score 22
  - change helped?
  - maybe, need deeper dive and running for a fixed saturated amount of time
  
- Can make the game run faster, by increasing the FPS constant
