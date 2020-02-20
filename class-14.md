# Read 14 The CSS Transforms, Transitions, and Animations

### February 19th, 2020


### _Transforms_
* With CSS3 came new ways to position and alter elements: _*transform*_
* The transform property comes in two different settings:
  1. Two-dimensional: Work on the x and y axes, known as horizontal and vertical axes.  
  1. Three-dimensional: work on both the x and y axes, as well as the z axis.
* Rotate property: provides the ability to rotate an element from 0 to 360 degrees, clockwise.
* Scale property: allows you to change the appeared size of an element. 
* Translate property:  works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.
* Skew property: is used to distort elements on the horizontal axis, vertical axis, or both. 
* The perspective of an element can be set in two different ways. One way includes using the perspective value within the transform property on individual elements, while the other includes using the perspective property on the parent element residing over child elements being transformed.
* Combining propertyes is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same.
* With three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including rotateX, rotateY, and rotateZ.
* Elements may also be translated on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element. Using a positive value will pull an element closer on the z axis, resulting in a larger element.

### _Transitions & Animations_
* With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.
* Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. 
* Transition: can occur when he easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.
* Transitions styles is by using the :hover, :focus, :active, and :target pseudo-classes.
* Transtition duration: the value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). 
* Transition-timing-function property is used to set the speed in which a transition will move.
* Transition-delay property: the delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing. 
* Animation duration: able to set the number of times an animation repeats, you may also declare the direction an animation completes.
* Animation Play State: allows an animation to be played or paused using the running and paused keyword values respectively.
* Animation-fill-mode property: identifies how an element should be styled either before, after, or before and after an animation is run.

### _8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS_
1. Fade in: It’s a great way to emphasize functionality or draw attention to a call to action.
1. Change color: Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS.
1. Grow & Shrink: To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge. Set your div’s class to “grow” and then add this code to your style block.
1. Rotate elements: CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS.
1. Square to circle: A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.
1. 3D shadow: This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.
1. Swing: Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.
1. Inset border: using box sizing, box-shadow: inset 0 0 0 25px #53a7ea;