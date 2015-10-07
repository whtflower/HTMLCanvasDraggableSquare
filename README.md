# HTML5 Canvas Square

## Objective
Create a square on Canvas which is draggable

## Directions
  1. Create a 300x300 pixel Canvas object
  2. Render a 40x40 pixel square into the Canvas object
  3. Make the square draggable

## How the code works
- Draw a 40*40 square from the cordination of (0,0).
- When user moves mouse over(mousemove in jQuery) and click to the square(mouseDown in jQuery), initial square will be cleared and re-draw a sqaure at the point where a user let go of mouse click(mouseUp in jQuery)

### Bug Fix
Issue: Even a user click out of square, the square is still draggable. Should not allow a user to be able to drag a square if pointer is out of the square. 
Solution: Added a code to remember last cordinates where a mouseup event(jQuery) happend. Then checks if the last cordinates matches with current cordinates when a user clicks.

