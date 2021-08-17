# CSS
## CSS Transforms

The `transform` property comes in two different settings, **two-dimensional** and **three-dimensional**.

1. **2D Transforms**: two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.

**2D Transform Operations**:
- **Rotate**: to rotate use `transform: rotate(valuedeg)`.
- **Scale**: to scale use `transform: scale(value)`. You can also scale by axis using either `scaleX(value)`, `scaleY(value)` or `scale(Xvalue, Yvalue)`.

- **Translate**: it is used to push the position of the elements. To translate use `transform: translateX(value)`,  `transform: translateY(value)` or `transform: translate(Xvalue, Yvalue)`.

- **Skew**: it is used to distort elements on the horizontal axis, vertical axis, or both. To skew use `transform: skewX(valuedeg)`, `transform: skewY(valuedeg)` or `transform: skewX(Xvaluedeg, Yvaluedeg)`.

- **Origin**: to use it you need to use `transform-origin: value value`.

- **Prespective**: to use it you need to use `transform: prespective(value)`.


2. **3D Transforms**: three-dimensional transforms work on both the x and y axes, as well as the z axis, known as length, width and depth.

**3D Transform Operations**:
- **Rotate**: to rotate use `transform: prespective(value) rotateX(valuedeg)`, `transform: prespective(value) rotateY(valuedeg)` or `transform: prespective(value) rotateZ(valuedeg)`.

- **Scale**: to scale use `transform: perspective(value) scaleZ(value) rotateX(valuedeg);`.

- **Translate**: to translate use `transform: perspective(value) translateZ(value);`.

- **Transform Style**: to use it you need to use `transform-style: preserve-3d;`.

- **Backface Visibility**: to use it you need to use `backface-visibility: hidden;`.

## CSS Transitions & Animations

**Transitions** allow the user to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

**Animations** allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

### Transitions:

***There are four transition related properties in total, including***:

- **transition-property**: used to specify the targeted property. **ex**: `transition-property: background;`.

- **transition-duration**: used to specify the duration of the transition. **ex**: `transition-duration: 500ms;`

- **transition-timing-function**: used to specify the way that the transition will happen using predefined functions. **ex**: `transition-timing-function: linear;`.

- **transition-delay**: used to specify a delay period for between the transitions. **ex**: `transition-delay: 200ms;`

### Animations
To set multiple points at which an element should undergo a transition, use the `@keyframes` rule. The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.
**ex**:  

```
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
```
***Animation related properties***:
- **Animation Name**: `animation-name: name;`.
- **Animation Duration**: `animation-duration: 2s;`.
- **Animation Timing Function**: `animation-timing-function: ease-in-out;`.
- **Animation Delay**: `animation-delay: .5s;`.
- **Animation Iteration Count**: `animation-iteration-count: infinite;`.

## Simple Transition/animation Examples
1. **Fade In**:

```
.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}
```

2. **Change color**:

```
.color:hover
{
        background:#53a7ea;
}
```

3. **Grow & Shrink**:

```
.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}
```

4. **Swing**:

```
@-webkit-keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
       transform: translateX(-5px);
    } 
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
@keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
        transform: translateX(-5px);
    }
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
--------------------
.swing:hover
{
        -webkit-animation: swing 1s ease;
        animation: swing 1s ease;
        -webkit-animation-iteration-count: 1;
        animation-iteration-count: 1;
}
```
.


