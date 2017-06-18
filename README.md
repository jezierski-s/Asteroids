# Asteroids

## Short parameters sheet for GD

### Scripts:
1. Rock (used in all types of Asteroids prefabs)
    - Rock Sprites: array of images, one will be randomly picked to be used as object sprite
    - Speed: initial speed of this object (linear movement), default is 2
    - Smaller Rock: prefab of asteroid which will be instantiated on destroy of this one
    - Pieces Number: number of instances to be created on destroy of this object, default is 2
    - Points Number: how many points the player will get for destroying it, default is 100
2. Warp (used in Bullet, Ship and Asteroids prefabs)
    - Padding: value in viewport units, it's margin that object must pass to be moved to the other edge, default is 0.1
3. Bullet (used in Bullet prefab only)
    - Speed: speed of created bullet, default is 10
    - Life Span: how long (in seconds) the bullet will last on screen, default is 1
4. MenuController (used in Menu Controller prefab)
    - Highscore String: customizable text before the highscore number, default is just "Highscore: "
5. GameOverController (user in Game Over Controller, of course)
    - Highscore String: the same as above, default is "Highscore: "
    - Score String: this time it's text standing before current score number, default is "Your Score: "
6. Ship (used in Ship prefab)
    - Max Velocity: maximal speed at which ship can fly after accelerating, default is 5
    - Rotation Speed: how fast can ship rotate around own axis, default is 250
    - Friction: it's percentage of speed after one update step if engine is off. The higher value, the more intertia the ship will have, default is 0.95
    - Acceleration: how fast the ship will accelerate, default is 5
    - Engine Treshold: it's the treshold of input (axis input is value from range 0-1), under which we shut down the engine, default is 0.1
7. FireBullet (used in Rifle prefab, which is part of Ship)
    - Fire Rate: how many seconds it takes to shoot next bullet, default is 0.1
8. GameController (used in Game Controller prefab) 
    - Offscreen Padding: how far from edges of screen the asteroids will spawn, default is 0.1
    - Start Asteroids Number: how many asteroids will be created on the first level, default is 2
    - Asteroids Per Level: how many asteroids will be added every next level, default is 1
    - Asteroid Object: it's the prefab of the Asteroid that we want to spawn first
    - Level String: it's the text indicating level that we're currently on. Default is simply "Level: "
    - Time To Start: time in seconds how long we must wait before the first Asteroids will be created, default is 2
    - Time To Restart: wait x seconds after crash of the Ship for the game to be restarted, default is 2
    - Start Music Tempo: initial number of seconds between two background beats, default is 2
    - Final Music Tempo: the same number as above, but it's the limit how fast the beat can go, default is 0.5
    - Music Tempo Change: how fast the tempo of music will change from Start to Final point, default is 0.05
    
