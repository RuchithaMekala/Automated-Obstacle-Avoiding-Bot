# Automated-Obstacle-Avoiding-Bot
Built an obstacle avoiding bot as a part of our summer workshop at IIT Kanpur.

Main objective was to detect an obstacle and avoid it successfully by taking appropriate turns.
Important components include:
Two DC Motors for each wheel (Left and Right)
Ultrasonic sensor to make note of distance from the bot to the obstacle

Based on the distance the right wheel velocity and left wheel velocity are calculated and bot can turn accordingly (if left wheel velocity < right wheel velocity then bot takes left turn) and with what angle it would turn will be determined by the magnitude of left and right wheel’s velocity.
Dataset is collected by training the model.
We trained the bot initially by manually controlling it to record Left wheel velocity, right wheel velocity and distance.
We implemented polynomial regression in prediction velocities
2 regression equations for each velocity.
(Distance is our independent variable, LFW and RWV are our dependent variables)

So in testing phase (Now our bot is freely moving on the ground)
For a given distance (i.e how far the bot is from the obstacle), the model determines left wheel and right wheel velocities.

