

# Read 08 Layout

### February 11th, 2020

### _Layout_
* All elements in the document (page) are treated like blocks, _unless_ we indicate the opositive.
* We can manipulate the margain, border and padding of each element.
* The float property moves elements to the left or right.
* Every HTML element is treated as abos, and each bos can be eiter block level block or inline level block.
* _Block level_: starts a new line, and acts like the main bilding block oj any layout. Block elements:
  * h1, p, ul, li
* _inline blocks_ flow between surranding text.
  * img, b, i
* If one block level element sits inside another block-level element, then the outher box is know as the containing or parent element.
* Options for controling the positions of the elements:
  * Normal flow (position : static)
  * Relative positioning (position : relative)
  * Absolutte positioning (position : absolute) _they act like it is not there_
  * Fixed positioning ((position : fixed) _type of absolute positionig that requires position fixed_
  * Floating elements. Alows lyouts to place boxes next to each other.
* Fixed width layouts designs do not change size as the user increase / decreases the side of their browser.
* Liquid layouts designs stretch and contract as the user increases or decreases the size of their browser window.