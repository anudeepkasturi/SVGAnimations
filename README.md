# Animated SVG

This is a simple project I made to learn how to use Scalable Vector Graphics (SVGs) and animate them through CSS. I wish to apply these skills to create interactive and responsive infographics.

## Accessible DOM

The image itself is embedded inline in the html file. This means that every aspect of the image can be grabbed through the DOM, if tagged appropriately. For example, I can use the Chrome developer tools to inspect the airplane flying through:

![airplane]
[airplane]: ./assets/airplane-select.png

The airplane is actually just a group tag with an id ```<g id="airplane">``` that encapsulates the group of paths that draws the plane.

Adding animations is easy when the image components can be accessed this way. Simply select the component and add an animation property.

```CSS
#airplane {
  animation: flying 10s linear infinite;
}
```
## Data Visualization

The next step to take this foundation and use this to visualize data in an engaging and appealing way. Imagine an interactive and responsive infographic that can show and hide extra information based on what the user wants while also looking pretty.
