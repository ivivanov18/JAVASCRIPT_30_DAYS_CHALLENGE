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
