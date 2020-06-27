# SMACSS and Responsive Web Design 
## Responsive 
**Responsive web design** is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.


## Flexible Layouts
**Flexible layouts**, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. 


## Media Queries
**Media queries** were built as an extension to media types commonly found when targeting and including styles. 


## Flexible Media
The final, equally important aspect to responsive web design involves **flexible media**. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.


## What is “Float”?
Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”. Here is an example of that.
## What are floats used for?
Floats can be used to create entire web layouts, also they are helpful for layout in smaller instances.
## Clearing the Float
Clear has four valid values as well. Both is most commonly used, which clears floats coming from either direction. Left and Right can be used to only clear the float from one direction respectively. None is the default, which is typically unnecessary unless removing a clear value from a cascade. Inherit would be the fifth. Clearing only the left or right float, while less commonly seen in the wild, definitely has its uses.
The Great Collapse
One of the more bewildering things about working with floats is how they can affect the element that contains them (their “parent” element). If this parent element contained nothing but floated elements, the height of it would literally collapse to nothing. This isn’t always obvious if the parent doesn’t contain any visually noticeable background. 
## Problems with Floats
- **Pushdown:** is a symptom of an element inside a floated item being wider than the float itself (typically an image). Most browsers will render the image outside the float, but not have the part sticking out affect other layout. IE will expand the float to contain the image, often drastically affecting layout. A common example is an image sticking out of the main content push the sidebar down below.
- **Double Margin Bug:** Another thing to remember when dealing with IE 6 is that if you apply a margin in the same direction as the float, it will double the margin. Quick fix: set display: inline on the float, and don’t worry it will remain a block-level element.
- **The 3px Jog:** is when text that is up next to a floated element is mysteriously kicked away by 3px like a weird forcefield around the float. Quick fix: set a width or height on the affected text.
- In IE 7, the **Bottom Margin Bug:** is when if a floated parent has floated children inside it, bottom margin on those children is ignored by the parent. Quick fix: using bottom padding on the parent instead.

## SMACSS 
**Scalable and Modular Architecture for CSS** is more style guide than rigid framework.SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS.