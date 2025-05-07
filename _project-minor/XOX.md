---
title: "Tic Tac Toe Player CNC Pen Plotter"
img: projects/cover-pictures/XOX.webp
collection: project
date: 2020-05-03 
---
<div align="justify">
Me and my teammates built a CNC Pen Plotter that uses image processing to play Tic-Tac-Toe with a real person. The player has a predefined amount of time to play their move, then the machine takes the picture of the board and detects the layout. The layout is then passed to a Python script that computes the next move. Machione then plays the move by sending the corresponding moves G-Code to the Ardunio that controls the servo motors.

This was a term project for ME331 at Bogazici University during the peak time of Covid that is why most parts of the machine had to be improvised. It was chosen as the best project in the class.
</div>

<center>
<video style="width:80.0%;border-radius:2px;margin-top:8px;margin-bottom:8px;margin-top:8px;" controls poster="/images/XOX.webp">
  <source src="/videos/tic-tac-toe-player.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</center>

<center>
<img src="/images/projects/xox-workflow.png" alt="General workflow of the system" style="width:80.0%;margin-top:8px;margin-bottom:8px;border-radius:5px;"/>
</center>

<center>
<img src="/images/projects/xox-imageProcessing.png" alt="Image Processing Steps" style="width:90.0%;margin-top:8px;margin-bottom:8px;"/>
</center>
