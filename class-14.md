# Reading notes 14a

## CSS Transforms

### Transform Syntax

``` js
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
// includes the transform property followed by the value. The value specifies the transfomr type followed by specific amount inside parentheses.
```
- both two dimensional and three dimensional syntax
- 2D works on x and y axis.
- 2d rotate value provides ability to rotate from 0 to 360

### 2d/3d Scale 
- changes appeared size of element.
- default scale value is 1. Anything smaller makes scale smaller and reverse is also true.
- possible to scale on height and width axis value first, followed by a comma  and y axis value.

### 2d/3d Translate
- works similar to relative positioning, pushing or pulling element in differing directions.
- you can translate x or y values.
- distance values can be any common length of measurement

### 2d/3d Skew
- used to distort elements on x or y axis, or both.
- value is measured in degrees.
- 3d can be translated to z axis

### Backface visibility
- when an object rotates 180 degrees, you are able to set backface-visibility value as hidden.

## Transitions and Animations

### Transitions
- for transition to take place, element must have a change in state, different styles must be identified for each state.
``` js
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
// example above will change the background color over the course of 1 second for the transition.
```
- transitional properties can include:
background-color 
background-position 
border-color 
border-width 
border-spacing 
bottom 
clip 
color 
crop 
font-size 
font-weight 
height 
left 
letter-spacing 
line-height 
margin 
max-height 
max-width 
min-height 
min-width 
opacity 
outline-color 
outline-offset 
outline-width 
padding 
right 
text-indent 
text-shadow 
top 
vertical-align 
visibility 
width 
word-spacing 
z-index

### Animation keyframes
- Can set up multiple points for a keyframes transition to take place. from 0% to 50% to 100% for instance.

``` js
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
1s;.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
  animation-timing-function: ease-in-out;
  animation-delay: .5s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}
this will adhere to the rules of the keyframe in the specified duration.
```


