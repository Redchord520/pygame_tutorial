**Game Development README**

This repository contains the source code for a game under development. Below are the key features and changes made so far:

### Commits Summary:

1. **Initial Commit: Implement Basic Game Window, Key Events, and Collision Detection**
   - Creation of a game window.
   - Addition of event handling for up and down key presses.
   - Implementation of collision detection.

2. **Refactor: Separate Concerns, Introduce Entity Management, and Implement Player Movement**
   - Removal of collision detection demonstration code from `main.py`.
   - Introduction of two new scripts: `entities.py` and `utils.py`.
   - `entities.py` encapsulates entity management, including the `PhysicEntity` class with update and render functions.
   - Integration of the `load_image` function in `utils.py` for centralized image loading.
   - Addition of the player sprite and left/right movement upon key press.

3. **Enhancement: Implement Pixel Art Effect Through Upscaling Rendered Sprite**
   - Utilization of the `.Surface` function in `main.py` to render the sprite on a half-resolution display.
   - Upscaling the rendered sprite to fit the larger resolution screen, creating a pixel art effect.

4. **Feature Addition: Implement Tilemap Generation and Rendering**
   - Introduction of `tilemap.py` script for generating and rendering on-grid and off-grid tiles.
   - Addition of the `load_images` function to `utils.py` for efficient loading of multiple images.
   - Integration of various assets including decor, grass, large_decor, and stone into the `main.py` assets folder.
   - Creation and rendering of the tilemap in `main.py`, setting the stage for diverse game environments.

5. **Enhancement: Introduce Advanced Collision Detection and Gravity Mechanics**
   - Implementation of `tiles_around` function in `tilemap.py` to retrieve surrounding tile locations.
   - Creation of a function utilizing pygame's `Rect` function for collision detection in `tilemap.py`.
   - Introduction of gravity mechanics in the `update` function of `entities.py` with a terminal velocity of 5.
   - Addition of a `rect` function in `entities.py` for entity-to-rect conversion for collision detection.
   - Implementation of collision detection against tile entities in the `update` function of `entities.py`, with player reset upon collision.
   - Introduction of a `collisions` boolean dictionary in `PhysicsEntity` for efficient collision detection.
   - Integration of tile map into `player.update` function in `main.py`, allowing for key press on the up arrow to trigger jump velocity.

6. **Feature: Introduce Camera Follow Functionality and Parallax Background Effect**
   - Implementation of a camera system for dynamic player follow.
   - Introduction of background scrolling to create a parallax effect.
   - Addition of cloud movement for enhanced visual depth.
   - Creation of a camera class to manage scrolling and offset.

7. **Feature: Implement Animation Class, Player Actions, and Enhanced Rendering**
   - Introduction of an `Animation` class for managing frame sequences.
   - Implementation of player action handling and rendering optimization.
   - Creation of a `Player` class to inherit from `PhysicsEntity` for improved control.
   - Enhancement of animation and player movement synchronization.

8. **Feature: Introduce Level Editor with Asset Cycling, Placement, and Camera Movement**
   - Development of a level editor with mouse and keyboard controls.
   - Implementation of asset cycling, placement, deletion, and camera movement.
   - Introduction of save/load functions for tilemap data.
   - Implementation of autotiling algorithm for efficient tilemap creation.


### How to Run:
1. Ensure you have Python installed on your system.
2. Clone this repository to your local machine.
3. Navigate to the project directory.
4. Run `main.py` using Python to start the game.

### Controls:
- Use the left and right arrow keys to move.
- Use the up arrow key to jump.
- Additional controls will be added in future commits.

### Contributing:
- Contributions are currently not open for external contributions, as the project is primarily for personal learning purposes. However, feel free to explore the codebase, provide feedback, or use it as a learning resource. Thank you for your understanding!

Stay tuned for further updates and features!
