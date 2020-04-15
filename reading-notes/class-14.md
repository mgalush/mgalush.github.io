# CSS transform

Elements may be distorted, or *transformed*, on both a two-dimensional plane or a three-dimensional plane

Two-dimensional transforms work on the x and y axes

Three-dimensional transforms work on both the x and y axes, as well as the z axis (for depth)

## 2D transform

The `transform` property can be set to:

`rotate`: rotates an element from 0 - 360 degrees.  A positive value will rotate it clockwise whereas a negative value will rotate it counterclockwise. 

```
.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}
```
![rotate](./images/rotate.png)

`scale`: changes the size of an element.  The default size is 1 so any number below 1 makes it smaller and any number above 1 makes it larger.  It changes either the width (`scaleX`) or the height (`scaleY`)

`translate`: changes the position of an element on either the x-axis(`translateX`) or y-axis (`tanslateY`)

```
.box-1 {
  transform: translateX(-10px);
}
.box-2 {
  transform: translateY(25%);
}
.box-3 {
  transform: translate(-10px, 25%);
}
```
![rotate](./images/translate.png)

`skew`: distorts elements on either the x-axis (`skewX`) or y-axis (`skewY`) and is measured in degrees
```
.box-1 {
  transform: skewX(5deg);
}
.box-2 {
  transform: skewY(-20deg);
}
.box-3 {
  transform: skew(5deg, -20deg);
  ```
  ![skew](./images/skew.png)

  `transform-origin`: changes the default `transform` origin the default, which is in the center of the element

## 3D transform

In order for 3D transformations to work, elements need a perspective (vanishing point) in which to transform.  The perspective can be set in two ways:

1. `perspective` property
2. `perspective-origin` property


The same properties can be used for both 3D and 2D

- `transform`: now takes a third value, `rotateZ`
- `scale`: now takes a third value, `scaleZ`
- `translate`: now takes a third value, `translateZ`

as well as additional properties such as:
- `rotate3d`

# CSS Transitions 

**Transitions** provide a change from one state to another, while **animations** can set multiple points of transition upon different keyframes

For a transition to take place, an element must have a change in state, and different styles must be identified for each state, using pseudoclasses such as `:hover`, `:focus`, `:active`, or `:target`

Additional transition properties include:
- `transition-property`: determines which property is altered
- `transition-duration`: time it takes to transition, in s or ms
- `transition-timing-function`: speed at which the transition will happen
- `transition-delay`: delays transition

```
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}
```
The above code will generate a box that will change its `background` over the course of `1` second in a `linear` fashion

You can shorthand these properties using the following: `transition: background 1s linear;`

Only properties that have an identifiable halfway point can be transitioned


### Awesome CSS transitions to try:
 
- fade in
- change collr
- grow & shrink
- rotate elements
- square to circle
- 3D shadow
- swing
- inset border

See examples [here](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/)


# CSS Animations

To determine when an element will undergo a animation, use the `@keyframe` rule, which includes the animation name, any animation breakpoints, and the properties intended to be animated

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

They then must be **assigned** to an element and declare the **length** of the animation:
```
.stage:hover .ball {
  animation-name: slide;
  animation-duration: 2s;
}
```

You can also: 
- delay the animation using `animation-timing-function` and `animation-delay`
- set a specific number of times in which an animation will occur using `animation-iteration-count`
- specify a direction using `animation-direction`
- play or pause the animation using `animation-play-state`



*Note: use vendor prefixing when using any of these values*
