Here's my solution to Assignment 1 of the course.
The were 3 goals:


" -Randomize the gap between pipes (vertical space), such that they’re no longer hardcoded to 90 pixels." For this one, I took the variable GAP_HEIGHT and moved it to PlayState.lua where it's going to be randomized with math.random frame by frame.

"-Randomize the interval at which pairs of pipes spawn, such that they’re no longer always 2 seconds apart." I created a variable called randomSpawn which I am randomizing to later compare the self.timer with it for the spawning of the pipes, self.timer has to be bigger than randomSpawn and randomSpawn has to be bigger than 1 because we don't want the pipes to be drawn right next to each other.



"-When a player enters the ScoreState, award them a “medal” via an image displayed along with the score; this can be any image or any type of medal you choose"   I created three png's of the medals, gold, silver and bronze. If the user scores 3+, gets the gold medal, if scores 2 gets the silver medal and if scores 1 or less gets the bronze medal.

"-Implement a pause feature (...)" In PlayState I created a condition for detecting is pause is set to true to stop the scrolling and the music or to resume everything if the user presses p again. I also added the png of the pause symbol which is drawn in the render function of PlayState.lua and added the pause.wav sound effect. 



I used sfxr for creating the sound effect and pixel online app for creating the medals!
