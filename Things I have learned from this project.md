# "*" : The CSS Universal Selector
 
The universal selector (*) selects all HTML elements on the page.
 

<br>
<br>

# Margin 0, padding 0: 
    inside universal selector will remove browser default style. 

<br>
<br>

# Box-sizing property:

The box-sizing property allows us to include the padding and border in an element's total width and height.
 

https://www.w3schools.com/css/css_boxmodel.asp
https://www.w3schools.com/css/css3_box-sizing.asp

<br>
<br>

# CSS background-size Property

The background-size property specifies the size of the background images. 

## auto
    Default value. The background image is displayed in its original size

## cover	
    Resize the background image to cover the entire container, even if it has to stretch the image or cut a little bit off one of the edges	

## contain
	Resize the background image to make sure the image is fully visible

https://www.w3schools.com/cssref/css3_pr_background-size.asp

<br>
<br>

# Backface visibility

The backface-visibility property defines whether or not the back face of an element should be visible when facing the user.
 

https://www.w3schools.com/cssref/css3_pr_backface-visibility.asp


<br>
<br>

# CSS box-shadow Property

 
The box-shadow property attaches one or more shadows to an element.
 

+ **h-offset**
	Required. The horizontal offset of the shadow. A positive value puts the shadow on the right side of the box, a negative value puts the shadow on the left side of the box	

+ **v-offset**	
    Required. The vertical offset of the shadow. A positive value puts the shadow below the box, a negative value puts the shadow above the box	
+ **blur**	
    Optional. The blur radius. The higher the number, the more blurred the shadow will be



<Br>
<Br>


# CSS Pseudo Elements

## CSS ::after Selector 

 
The ::after selector inserts something after the content of each selected element(s).

Use the content property to specify the content to insert.
 

```CSS
p::after {
  content: " - Remember this";
  background-color: yellow;
  color: red;
  font-weight: bold;
}

```

## CSS ::before Selector 

 
The ::before selector inserts something before the content of each selected element(s).

Use the content property to specify the content to insert.
 

```CSS
p::before {
  content: " - Remember this";
  background-color: yellow;
  color: red;
  font-weight: bold;
}
```
<br>
<br>

# CSS @keyframes Rule

The @keyframes rule specifies the animation code.

The animation is created by gradually changing from one set of CSS styles to another.

During the animation, you can change the set of CSS styles many times.

Specify when the style change will happen in percent, or with the keywords "from" and "to", which is the same as 0% and 100%. 0% is the beginning of the animation, 100% is when the animation is complete.

Tip: For best browser support, you should always define both the 0% and the 100% selectors.

Note: Use the animation properties to control the appearance of the animation, and also to bind the animation to selectors.

**Note:** The !important rule is ignored in a keyframe (See last example on this page).



```css
@keyframes mymove {
  0%   {top: 0px; left: 0px; background: red;}
  25%  {top: 0px; left: 100px; background: blue;}
  50%  {top: 100px; left: 100px; background: yellow;}
  75%  {top: 100px; left: 0px; background: green;}
  100% {top: 0px; left: 0px; background: red;}
}
```
<br>
<br>


# CSS animation Property

The animation property is a shorthand property for:

+ animation-name
+ animation-duration
+ animation-timing-function
+ animation-delay
+ animation-iteration-count
+ animation-direction
+ animation-fill-mode
+ animation-play-state

**Note:** Always specify the animation-duration property, otherwise the duration is 0, and will never be played.


```css
div {
  animation-name: example;
  animation-duration: 5s;
  animation-timing-function: linear;
  animation-delay: 2s;
  animation-iteration-count: infinite;
  animation-direction: alternate;
}

div {
  animation: example 5s linear 2s infinite alternate;
}
```

## Specify the fill-mode For an Animation

CSS animations do not affect an element before the first keyframe is played or after the last keyframe is played. The animation-fill-mode property can override this behavior.

The animation-fill-mode property specifies a style for the target element when the animation is not playing (before it starts, after it ends, or both).



https://www.w3schools.com/css/css3_animations.asp


<br>
<br>

# CSS Transitions

CSS transitions allows you to change property values smoothly, over a given duration.

## Transitions properties:

+ transition
+ transition-delay
+ transition-duration
+ transition-property
+ transition-timing-function

To create a transition effect, you must specify two things:

+ the CSS property you want to add an effect to
+ the duration of the effect

**Note**: If the duration part is not specified, the transition will have no effect, because the default value is 0.

The following example shows a 100px * 100px red <div> element. The <div> element has also specified a transition effect for the width property, with a duration of 2 seconds:

```css
div {
  width: 100px;
  height: 100px;
  background: red;
  transition: width 2s;
}

```
The transition effect will start when the specified CSS property (width) changes value.

Now, let us specify a new value for the width property when a user mouses over the <div> element:

```css
div:hover {
  width: 300px;
}
```

## Specify the Speed Curve of the Transition
https://www.w3schools.com/css/css3_transitions.asp#:~:text=Specify%20the%20Speed%20Curve%20of%20the%20Transition



<br>
<br>

# CSS 2D Transforms

CSS transforms allow you to move, rotate, scale, and skew elements.

+ translate()
+ rotate()
+ scaleX()
+ scaleY()
+ scale()
+ skewX()
+ skewY()
+ skew()
+ matrix()

## The translate() Method

The translate() method moves an element from its current position (according to the parameters given for the X-axis and the Y-axis).

https://www.w3schools.com/css/css3_2dtransforms.asp


<br>
<br>
# The Clearfix 



<br>
<br>

# attribute selector 

+ all the class start with col : [class^="col-"]{}
+ all the class end with col : [class$="col-"]{}
+ all the class contain col : [class*="col-"]{}

