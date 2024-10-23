# Breakout

W Kavanagh. June Summer 2024

## controls
A/D to move the paddle right and left.
P to pause.

## Powerups
big/small paddle (blue)
fast/slow ball (fancy yellow)
fire ball (green)

# Tasklist

## Suggested fixes
* Fix the compiler issues in the code

## Suggested tasks
* Implement mouse input for pad
* Improved VFX (ball trail, paddle hit response, brick particle destruction)
* Better UI (progress bar rather than timer for countdown).
* GameLoop
* Better ball physics (Box2D)
* Leaderboards
* More ball types (e.g., multiball, sticky ball [where you shoot the ball from the paddle every time], tiny ball, big ball, brick-tracking ball)
* Sounds with increasing tone between bounces.
* Implement commentary with calls to an LLM such as LLama

# Time Details and Changelist
<Add information to this section about the time you've taken for this task along with a professional changelist.>
- Spent 10 minutes familiariasing myself with the codebase
- Spent 10 minutes fixing a circular dependency error which was preventing the game from starting
- Spent 20 minutes adding a trail behind the ball
- Spent 45 minutes adding audio when the ball hits the paddle or bricks
- Spent 30 minutes attempting to add a powerup which made the ball bigger
    - I removed this in a later commit because I couldn't work out how to change the hitbox
      so it would interact with the paddle correctly
- Spent 10 minutes updating the powerup spawning function to use parameters instead of harcoded numbers
- Spent 45 minutes adding screen shake when the player loses a life
- Spent 1 hour adding a progress bar which countsdown how long the powerup has left then fixed a bug
    which caused the broken big ball powerup to still spawning
Total time spent: 3.5 to 4 hours

# Sources
https://www.sfml-dev.org/tutorials/2.6/audio-sounds.php
https://pixabay.com/sound-effects/search/retro%20games/
https://en.sfml-dev.org/forums/index.php?topic=27891.0
https://en.sfml-dev.org/forums/index.php?topic=4885.0