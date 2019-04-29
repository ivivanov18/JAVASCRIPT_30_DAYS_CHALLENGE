# 30 DAYS JAVASCRIPT CHALLENGE

## PURPOSE OF THE COURSE

Improve on my JS skills.

## NOTES

### DAY 1 - JAVASCRIPT DRUM KIT

#### How to play audio

Select the `<audio>` tag and use `play()` method. To return the audio from the beginning set the `currentTime` property to 0.

### DAY 2 - CSS + JS Clock

#### How to animate minutes, hours or second hands

Use `setInterval` function along with the `transform` property of the selected hand to `rotate(<number_of_degrees>deg)`.

#### How to rotate the hands not by the middle of the hand but by the end

Use the `transform-origin` property to offset the origin by 100%.

### DAY 3 - Playing with CSS variables and JS

#### DATASET OBJECT

Use `dataset` to access all the `data-` attributes for a particular DOM element.
Example from lesson:

- In order to access the attribute _data-sizing_ from `<input data-sizing="px"/>` use `dataset.sizing`.

#### Variables in CSS

Define them the following way: From the example provided in the course, at the **:root** DOM element, we declare 3 variables

```
      :root {
        --base: #ffc600;
        --spacing: 10px;
        --blur: 10px;
      }
```

To use them:

```
      img {
        padding: var(--spacing);
        background: var(--base);
        filter: blur(var(--blur));
      }
```

### DAY 4 - Array Cardio Part 1

#### CONSOLE.TABLE

Better way to log arrays and objects representating in visual table looking way.

#### JS ARRAY FUNCTIONS

- map
- filter
- reduce
- sort

### DAY 5 - FLEX PANELS IMAGE GALLERY

#### CSS TOGGLE CLASS

`<dom element>.classList.toggle(<class name>)`

#### CSS SELECT

#### FLEX

- `flex: 1` tells the children items in the parent flex container to occupy the whole space within the parent equally. This property can be used to animate a given item by setting it to higher number, as done in the example.

### DAY 6 - AJAX TYPE AHEAD

#### CHANGE EVENT

Change event only fires when we go out of the input. If we want an event to fire on keyup use `keyup` event.

#### `THIS` value in functions called from events listeners

#### TIP - GET DATA FIRST

Useful tip in the workflow: `Get the data first and then worry how to hook to events listeners and display it`.

### DAY 7 - Array Cardio Part 2

#### JS ARRAY FUNCTIONS

- `some`: returns `true` if at least one element meets the given condition
- `every`: returns `true` if all the elements meet the given condition
- `find`: returns the element that meets the given condition
- `findIndex`: returns the index of the element that meets the given condition
- `splice` modifies the current array by deleting the number of elements specified from the specified index.
- `slice` is another way to do it without modifiying the original array. The same as `<array>.splice(index, 1)` can be achieved the following way with `slice`:

```
  const newComments = [
    ...comments.slice(0, index), // takes from 0 to index - 1 and spreads it
    ...comments.slice(index + 1) // takes from index + 1 till end and spreads it
  ];
```

Personally, I prefer the second way which is a more functional programming way to do and that is without modifiying the initial object.

#### CONSOLE.LOG({<variable>})

Logs the following way:
`{<variable>: true}` instead of just `true`.

### DAY 8 - Fun with HTML5 Canvas

#### Events

- `mousedown`: start drawing
- `mousemove`: draw
- `mouseup`: stop drawing
- `mouseout`: stop drawing

#### HTML canvas and methods

- `canvas` dom element
- `const ctx = canvas.getContext("2d");`
- Context properties:
  - `strokeStyle`: color
  - `lineJoin`:
  - `lineCap`:
  - `lineWidth`:

#### HSL

- Hue: degree on the color wheel from 0 to 360. 0 is red, 120 is green, 240 is blue.
- Saturation: percentage value, 0% means a shade of gray and 100% is the full color.
- Lightness: percentage value, 0% is black, 100% is white.

### DAY 9 - 14 Must Know Dev Tools Tricks

#### How to find modifiers, event listeners JS functions

In the console, click on given DOM elements and select `Break on --> attribute modifications`. When code is executed, the source of the page will be opened and the execution stopped on the function that is modifiying the attribute

#### How to style a console.log

Add a `%c` in the console.log in front of the element that needs to be styled, and add a second argument containing the style that you want to apply. As an example:
`console.log("%c i am some great text","font-size:50px; background: teal");`

#### CONSOLE.DIR(<dom element>)

Displays all the available methods of the given dom element and generally and of the stuff that lives within the given dom element.

#### CONSOLE.GROUP

To group the console.log of the different properties and/or information of the given object. The import is to use `console.group(<obj property>)` at the beginning of the group
and `console.groupEnd(<same variable or obj property used at beginning>)`. `console.group(<obj property>)` can be replaced by `console.groupCollapsed(<obj property>)` to collapse all the displays by default.

```
        console.group(`${dog.name}`);
        console.log(`Dog age is${dog.age}`);
        console.log("${dog.name} is a ${dog.age * 7} dog years old");
        console.groupEnd(`${dog.name}`);
```

#### CONSOLE.COUNT(<string>)

To count all the times that the console.count has been logged out with the given string.

#### CONSOLE.TIME

Start with `console.time(<string indicating what we are measuring>)` , do the action, then at the end finish with `console.timeEnd(<same string as in the beginning of timer>)`

### DAY 10 - Hold Shift To Check Multiple Checkboxes

#### Click event on checkbox

Will fire even if you use your keyboard.
