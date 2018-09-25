### The Flex Container Properties

- Flex-direction
  ```
  ul {
  flex-direction: row || column || row-reverse || column-reverse;
  }
  ```
  
- Flex-wrap
  ```
  ul {
  flex-wrap: wrap || nowrap || wrap-reverse;
  }
  ```
  
  If we add a ridiculous amount of flex-items to our parent element. I choose 10 more items. What happens??
  Again, the flex container adapts to fit all children in, even if I need to scroll my browser `horizontally`.
  This is the default behavior of every flex container. It keeps on accommodating more flex items on a single line
  because the `flex-wrap` property defaults to `nowrap`.
  
  Well, with that number of flex-items, you certainly want the flex-container to 'wrap' around these elements. i.e.
  When the available space can no longer support the flex-items, break unto multiple lines when needed,
  and with that comes the wrap value.
  
  ```
  ul {
	flex-wrap: wrap;
  }
  ```
  
  
- Flex-flow
  The `flex-flow` is a shorthand property which takes `flex-direction` and `Flex-wrap` values. Ever used the `border`
  shorthand property? `border: 1px solid red`. It's the same concept here. Multiple values declared in one line.
  Re-writing the code above would yield this:
  ```
  ul {
	flex-flow: row wrap; /*direction 'row' and yes, please wrap the items.*/
  }
  ```
  
- Justify-content
  Life's really good with the flexbox model! If you still doubt that, the `justify-content` property would convince you.
  It may take on any of these 5 values:
  ```
  ul {
	justify-content: flex-start || flex-end || center || space-between || space-around
  }
  ```
  
- Align-items
  
- Align-content
  
  
