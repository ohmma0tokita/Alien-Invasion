# Alien-InvasionMY FIRST GAME: i gave it almost all my time ngl, and i am kinda proud of the result, as
i was always compairing my past self and me now, and how i improved.
MADE WITH PYGAME

03/09/2021
Started the project
04/09/2021 04:05 (AM)
finished the rolling screen, and the bg music
finished the ship: texture + mouvement
finished the bullets (2 types): texture + sound + mouvement
04/09/2021 19:51
finished the home_screen: bg/sound/animations/planets/asteroids
finished home_button
05/09/2021 22:33
finished everything all remaining is styling and making the guide
06/09/2021 12:44
GAME IS DONE, and has places to improvements

GUIDE:
1) Files:
files are for sounds in game, non animated objects, and sprites: for animated objects,
because pygame main idea is: put a square, blit corresponding image.

2)Modules.py
i wanted to seperate the classes/functions from main game script so it looks cleaner,
classes main idea is: create a parent class that has some features common to all other
children classes, then create a seperate class for each differently responding child
example: bullets from fighter ship go upwards, bullets from alien ships go downward,
they are both bullets, but each one has it seperate class for this reason,
pygame.sprites.Sprites class helped a lot, you just create a group of bullets for exapmle,
and update it in the game loop, and each element in that group will update selon its own
update function in its class
Animation is in parent class,

3)main.py
this is the main game script, we import from Modules.py all + other modules, 
then it tells the game story
=>then goes to the home screen:
fixes the screen, puts start button on screen, etc...
=>and then to the game loop:
animated screen, check for collisions, shows stats, etc...
=>finally the game over screen:
simply shows stats
=====NOTES:
pygame.sprite.groupcollide(), made things way easier
