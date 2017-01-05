# Animated SVG

This is a simple project I made to learn how to use Scalable Vector Graphics (SVGs) and animate them through CSS.

## Accessible DOM

The image itself is embedded inline in the html file. This means that every aspect of the image can be grabbed through the DOM, if tagged appropriately. For example, I can use the Chrome developer tools to inspect the airplane flying through:

![airplane]
[airplane]: ./assets/airplane-select.png

The airplane is actually just a group tag with an id of "airplane" ```<g id="airplane">``` that encapsulates the group of paths that draws the plane.

Adding animations is easy when the image components can be accessed this way. Simply select the component and add an animation property.

```CSS
#airplane {
  animation-name: flying;
  animation-duration: 10s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
```
