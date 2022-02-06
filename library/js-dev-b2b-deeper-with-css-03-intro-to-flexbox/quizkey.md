**Deeper with CSS: Intro to flexbox**

1. What is the main purpose of using flexbox?

A. To create visually appealing borders around HTML containers.
B. To create space between HTML containers.
C. To style HTML text in interesting ways.
D. To create flexible web page layouts easily.

**Answer: D**

2. How do you apply flexbox properties to a container element?

A. `display: flex`
B. `display: block`
C. `display: flex-box`
D. `display: inline-block`

**Answer: A**

3. Select all statements that are TRUE about flexbox. 

A. The default value for `flex-direction` is `column`.
B. The default value for `flex-direction` is `row`.
C. Setting the `flex` property of all items within a flex container to `1` will cause them to display with the same width 
D. With flexbox, it is not possible to align items horizontally in reverse order using the `flex-direction` property

**Answer: B & C**

4. Given the following HTML snippet:
  
```html
<div class="container">
  <div class="item-1">Item 1 Content</div>
  <div class="item-2">Item 2 Content</div>
  <div class="item-3">Item 3 Content</div>
</div>
```
and the following CSS file:

```css
.container {
  display: flex;
}

.item-1 {
  flex: 1;
}

.item-2 {
  flex: 2;
}

.item-3 {
  flex: 3;
}
```

Which of the following statement(s) are TRUE? Select at least one answer.

A. `item-1` will occupy the entire width of the parent container 
B. `item-2` will occupy the entire width of the parent container
C. `item-3` will occupy half the width of the parent container
D. `item-3` is always three times as wide as `item-1`

**Answer: C & D**
