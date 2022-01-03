# Reinforcement Learning for Atari games

## Breakout Atari

In this environment, the observation is an **RGB image** of the screen, which is an array of shape **(210, 160, 3)** Each action is repeatedly performed for a duration of *k* frames, where *k* is uniformly sampled from {2, 3, 4}. 

This will be further explained in **explore the environment** section

### Game rules

Breakout begins with eight rows of bricks, with each two rows a different color. The color order from the bottom up is **yellow**, **green**, **orange** and **red**.   

Using a single ball, the player must knock down as many bricks as possible by using the walls and/or the paddle below to ricochet the ball against the bricks and eliminate them. If the player’s paddle misses the ball’s rebound, he or she will lose a turn. The player has three turns to try to clear two screens of bricks. 

Color to points:
- Yellow bricks earn one point each 
- Green bricks earn three points 
- Orange bricks earn five points 
- The top-level red bricks score seven points each

The paddle shrinks to one-half its size after the ball has broken through the red row and hit the upper wall. Ball speed increases at specific intervals: after four hits, after twelve hits, and after making contact with the orange and red rows.


<img src="https://raw.githubusercontent.com/Kyushik/Unity_ML_Agent/master/Images/Breakout.png" width="400px" height="500px" />


*Rules description taken from [wikipedia](https://en.wikipedia.org/wiki/Breakout_%28video_game%29)*


### 1. Install necessary packages/libs
```bash
pip install 'stable-baselines3[extra]'
pip install tensorboard==1.15.0
python -m atari_py.import_roms rars
```
**NOTE**:  ROMS are predownloaded and included in the repository.

You can also download them yourself from [Atari ROMS](http://www.atarimania.com/rom_collection_archive_atari_2600_roms.html)


## CarRacing visual example 

#### Random agent
<img src="./res/dummy_example.gif"/>

#### Trained agent
<img src="./res/trained_300k.gif"/>

### All further instruction are in corresponding IPython notebooks
