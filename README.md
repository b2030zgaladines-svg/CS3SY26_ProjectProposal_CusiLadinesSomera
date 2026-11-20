# CS3SY26_ProjectProposal by Carl Gabriel Cusi, Zander Gelo Ladines, and Charlie Sean Somera from 9-Beryllium 2030 of PSHS


## Project Proposal Template:
### Project Title or Name of the Application	:  Asteroids Game
### Section			   	      : 9-Beryllium
### Group Members			    : Carl Gabriel Cusi, Zander Gelo Ladines, Charlie Sean Somera
### Date (Proposal Date)  : Nov 13, 2026
### Project Description:

Our project is a game built in the python turtle module based on the arcade game Asteroids. It’s a fun game, and we’d like to make our port of it special by allowing its code to be seen and used as reference by other people. One small difference between the actual Asteroids is that ours does not have the flying saucers that also shoot projectiles.

The classes and mechanics are structured through a clear set of inheritance and association relationships. The foundational Base class establishes the core identity of all game objects by defining shared physical attributes like position, velocity, health points, and size, along with key methods for movement, drawing, and collision detection, which forms the basis for interaction. Directly inheriting from this are the primary game entities: the player-controlled Spaceship and the Bullet class, which extend the base functionality with specific attributes like score and damage value. The relationship between the Spaceship and the Bullet is defined by a composition association, where the Spaceship is responsible for creating and managing a list of activeBullets. This allows the ship's firing mechanic, +shootBullet(), to instantiate new Bullets that carry their own +killAsteroid() method to inflict damage on targets. Furthermore, the Asteroid class, which also inherits from Base and is specifically targeted by the player's projectiles, introduces its own properties like asteroidSize and split states. It is designed with methods to +attackShip() and +takeDamage(), completing the interaction loop between the player and obstacles. Finally, the Control class is linked directly to the top level Base class to act as the overall game manager, coordinating these diverse interactions. By linking to the base of all entities, the Control class is able to manage global statistics like bulletCount and asteroidSpawnRate, oversee object creation via +manageSpawn(), and handle game logic, including +handleCollisions() across all subclasses, ensuring cohesive gameplay.

Of course, we’re mainly targeting people who want to just have fun, but our secondary audience is other inexperienced coders similar to us and want to see how they can build a functioning game with the knowledge up to OOP.

Sample Diagram:
<img width="1340" height="800" alt="image" src="https://github.com/user-attachments/assets/bbf889f8-6140-4387-b651-e359bc5c9bdf" />


### Goals:

Describe the long term outcomes of your project followed by a couple of objectives to meet the goals stated in this paragraph

- Objective 1: Playable Character.
- Objective 2: Working Obstacles with collision.
- Objective 3: Working Bullets with collision.
- Objective 4: The ability to reload the game without closing the window.
- Objective 5: The walls of the map should warp you to the other side.
- Objective 6: The game should run at a reasonable speed without much lag.


[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
