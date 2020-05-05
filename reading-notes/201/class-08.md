# HTML layout
CSS treats each element as if it were in a box.  This box can either be **inline** or **block** level. 
- **Block** level boxes start on a new line
- **Inline** level boxes flow between surrounding text

If one block sits inside another box, the outer box as known as it's **containing** or **parent** element.

## Positioning

Positioning properties allow you to control the layout of the page:
- `position: static`: This is the default position. Every block level element appears on a new line
- `position: relative`: Shifts the element top, right, left, or down based on where it would normally be positioned
- `position absolute`: Positions the element in relation to its containing element
- `position: fixed`: A form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element 
- `position: float (left or right)`: Allows you to take the element out of normal flow and position it to the far left or right of a containing box
