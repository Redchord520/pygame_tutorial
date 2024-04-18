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


### How to Run:
1. Ensure you have Python installed on your system.
2. Clone this repository to your local machine.
3. Navigate to the project directory.
4. Run `main.py` using Python to start the game.

### Controls:
- Use the left and right arrow keys to move.
- Additional controls will be added in future commits.

### Contributing:
- Contributions are currently not open for external contributions, as the project is primarily for personal learning purposes. However, feel free to explore the codebase, provide feedback, or use it as a learning resource. Thank you for your understanding!

### Future Plans:
- Implement game mechanics such as scoring, enemy entities, and level progression.
- Enhance graphics and add sound effects.
- Improve user interface and menu screens.

Stay tuned for further updates and features!
