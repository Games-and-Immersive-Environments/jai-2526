# Lab 02

- The marble drop game
- Creating a Basic First-Person Shooter

## The marble drop game

Open Unity Hub and create a new 3D project called MarbleDropGame. Download the [marbleDropGame-urp.unitypackage](../packages/MarbleDropGame-urp.unitypackage), go to your Assets section and import it to the project (right click > import package).

Press **PLAY** to run the game.

Explore the Assets folder and try to understand how and why everything works. Open the
scripts to understand how they work and when they are called.

Try to answer the following questions.

### Physics

- Why is the ball affected by gravity?
<!-- it contains a Rigigbody component with mass and it is set to "Use Gravity" -->
- What happens if you change the inclination of the board?
<!-- it changes the physics of the ball while it is falling. Some inclination values may even allow the ball to escape the board since there is no "glass" to prevent the ball from bouncing away from the board plane.-->
- The ball is a liitle bit bouncy It doesn't feel like being made of solid metal.Where are the properties that control the behaviour of the collisions? Adjust them in a way that resembles a metallic ball hitting wood pins.
<!-- The properties are inside the Rigidbody component of the Sphere object. It may help to increase its mass and also its angular damping coefficient to help keep the ball on the board when it hits the bottom. -->
- How does the ball reset?
<!-- Through the ResetState() method that places the ball in the original position. It gets called when a collision between the ball and the Slot prefab is detected. -->

### Scene Graph

- Where and how are the table pins created? Can you have a board with a different number of pins easily?
<!-- The pins are created inside the TableScript. Yes, the number of pins can be easily changed. The number of pins is controlled by the public variables Rows and Columns.-->
- In this example we have used the `localPosition` and `localScale` to place and size the instantiated objects. This requires thinking in the **Local Coordinates** of some object (In this case the "Back" of the board). A "messier" approach would be to work in the **World Coordinates**, using `position` and `scale` and eventually `rotation`. The properties `up`, `right` and `forward` are the axes of the  **Local Coordinates** of the object's transform expressed in **World Coordinates**. They form a left-handed coordinate system. The source code has this alternative approach commented for you to compare both approaches.

- How is the table size obtained? Try to adjust the width of all the table delimiters to a
common different value and see what happens when you run the game.
<!-- The table size is extracted from the Meshilter component of the "Back" object. This object provided access to the mesh, its bounds and size (dimensions). -->

### Game Mechanics

- What mechanism has been used to collect points?
<!-- Points are collected when the ball "collides" with a Slot prefab Sphere Collider. The Slot Sphere Collider is marked as "Is Trigger". When a collision starts, the OnTriggerEnter() method gets called for the object marked with "Is Trigger". The code can be found in the script assigned to the Slot Prefab (Slot Script) -->
- Try turning on the MeshRenderer of the Slot prefab. What happens?
<!-- The slots are shown as cubes. -->
- Switch off the MeshRenderer of the Slot prefab. Press **Play** and, while the game is running, select the Slot instances in the Hierarchy Browser (they should be right at the bottom). What happened?
<!-- The sphere colliders of the slots are now visible. -->
- What is the condition that makes the ball restart?
<!-- When no significant movement has been detected for the ball for 100 consecutive update cycles. -->
- Press **Play**. Now press the **Stats** button on the top right corner of the **Game** Window. How many triangles are in the scene?
<!-- There are around 23k triangles and 27.8 vertices. -->

## Suggestions for improvement:
-  The score is kind of buggy. When a ball bounces in a slot it may collect points more than
once. Why does it happen? Devise and implement a solution to solve this problem.
- Create a ball that is around 70% of the separation between adjacent pins
- This is already a simulation, but not yet a game. There is no purpose or challenge. The
player has no play in it. Let the player control where the ball is released. You can limit
the position to lie on a single horizontal line that crosses the current starting position.
- Rules are meant to be broken! Or bent at least! Let’s have the possibility to slightly
shake the board.
- The score is not visible. Add a score text message to a GUI layer.
- It would be great if slots were marked with the points assigned to them. A texture
painting the board would do nicely.
- Let’s have a finite number of ball tries per game.

## Creating a Basic First-Person Shooter

Open Unity Hub and create a new 3D project called **basicFPS**. Download the lab2-urp.unitypackage, go to your Assets section and import it to the project (right click > import package).

Press **Play** to run the game.
Use the common interface for FPS (WASD+Space+mouse).
Use **ESC** to unlock the mouse.

### Scene Graph

### Input: Camera movement

### Physics: Shooting Bullets

### State and Basic GUI

### Events and Enemies: Targets

## Challenge (1 week)

Create an improved version of the basicFPS game with:
- Better graphics
- If the ball hits a target, create an explosion sphere in the correct spot.
- Add the concept of 3 lifes to the state.
- Switch between 1st and 3rd person with a button.
- Improve the “AI” of the targets.
- **Extra**: Player rotation follows the mouse position and depends on deltaTime.