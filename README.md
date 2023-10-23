# Simon-game 

**HTML and CSS:**

- The HTML appears to contain buttons with different colors.
- The CSS styles the game elements, including the buttons, background, fonts, and game-over screen.
  
![image](https://github.com/SpatikaP/Simon-game/assets/79979665/83bc5ce2-c967-42f8-bf27-3c799252685c)

**JavaScript:**

1. `buttonColours`: An array of colors used in the game.

2. `gamePattern`: An array to store the randomly generated color sequence.

3. `userClickedPattern`: An array to store the colors clicked by the user.

4. `started`: A boolean variable to track if the game has started.

5. `level`: A variable to keep track of the current level.

6. `$(document).keypress()`: A jQuery event handler for starting the game when a key is pressed. It initializes the game by changing the game title and calling the `nextSequence()` function.

7. `$(".btn").click()`: A jQuery event handler for when a color button is clicked by the user. It records the user's color choice and calls functions to play sounds, animate the button press, and check the user's answer.

8. `checkAnswer()`: A function that compares the user's clicked pattern with the game pattern. If the user's pattern matches the game pattern, it proceeds to the next level. If not, it ends the game.

9. `nextSequence()`: A function to generate the next color in the game pattern. It increments the level, displays the new level, and plays animations and sounds.

10. `animatePress()`: A function to add and remove a "pressed" class to an element, creating a visual effect.

11. `playSound()`: A function to play a sound associated with a color.

12. `startOver()`: A function to reset the game when it's over.

**Game Logic:**

- The game starts when a key is pressed (`$(document).keypress()`).
- Users are required to repeat the color pattern by clicking on the buttons.
- The game keeps track of the sequence and the user's input.
- If the user's input matches the generated pattern, the game proceeds to the next level.
- If the user makes a mistake, the game displays "Game Over" and allows restarting.

The game is based on the classic Simon memory game, where the player needs to remember and repeat a sequence of colors. It demonstrates the use of event handling, animation, and sound effects in a simple browser-based game.
