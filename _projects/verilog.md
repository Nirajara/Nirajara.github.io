---
layout: page
title: Simon Memory Game
description: The Simon Memory Game on a Nexys 3 FPGA board
img: assets/img/verilog.jpg
importance: 1
category: code_projects
---

The Simon Memory Game tests a person's ability to remember a sequence. I implemented this game with my lab partners two different ways (difficult and easy mode). Easy mode is your stereotypical game where n LED blinks at n rounds (ex. 1 LED for round 1, 2 LEDs for round 2). The sequence builds off of the previous round. The game shows the player the sequence of lights once and the player flips the corresponding swiches in that order. Once a mistake is made or the timer runs out, the game is over!

The difficult mode is similar, except that the sequence does <i>not</i> build off the previous round. Instead a new sequence is generated every time.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.html path="assets/video/verilog.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>