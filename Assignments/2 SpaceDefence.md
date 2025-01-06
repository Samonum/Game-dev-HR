# 2 Space Defence
Finish the Space defence game.

The Space Defence game is a game in which the player controls a space ship. In the game the player can shoot bullets at aliens theat are invading earth to defeat them. The player can get a temporary upgrade by shooting down a crate. Hitting the crate will turn the ship's cannon into a laser.

Use the Game found at `<TODO: add link>`. You may add extra methods, but do not change the signature (method name, parameters or return type) of the methods given in the template.

Finish the game by adding the following:

### Functionality:
Implement the following functionality:

The spaceship uses the following static methods from the `LinePieceCollider` class to aim:
1. `float GetAngle(Vector2 direction)`
2. `Vector2 GetDirection(Vector2 point1, Vector2 point2)`

Add player movement:
1. Allow the spaceship so move using **both** the WASD keys and the arrow keys.
2. Rotate the space ship in the direction it is moving.

Add movement to the enemies:
1. For the Alien class, whenever it moves, pick a random point exactly 200px away from its spawn position. Make the alien move between this point and its spawn position.


### Collision:
In the Collision folder are several collider classes for different shapes. Rectangles, circles and line pieces, but the intersection logic is still missing. How to calculate intersection is described in `<TODO: Add link>` 
The Circle collider describes a circle using a location, described by 2 floats for the X and Y coordinates respectively and a radius. Everything that is less than the Radius away from the circle is considered to be within the circle.
In the `CircleCollider` class add:
1. Logic to calculate the intersection between two circles in the `Intersects(CircleCollider other)` method.
2. Logic to calculate the intersection between a circle and a rectangle in the `Intersects(RectangleCollider other)` method.

A LinePiece is described by two Vector2, Start and End. Everything that is on the line between Start and End is on the Line. 
In the `LinePieceCollider` class add:
1. Logic to calculate the intersection between a line piece and a circle in the `Intersects(CircleCollider other)` method. (Hint: you may use the `NearestPointOnLine` method)
2. Logic to calculate the intersection between a line piece and a rectangle in the `Intersects(RectangleCollider other)` method.
